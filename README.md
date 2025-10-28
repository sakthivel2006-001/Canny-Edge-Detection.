# Canny-Edge-Detection.
# workshop-3 - Canny Edge Detection
# Name :sakthivel s
# reg no:212223220090
## AIM :
To implement the Canny Edge Detection algorithm on a digital image to accurately detect and highlight significant edges while minimizing noise and false detections.

## PROGRAM
```
import cv2
import matplotlib.pyplot as plt
# Read the image
img = cv2.imread('sakthivel.jpg',cv2.IMREAD_GRAYSCALE)
# Apply Gaussian blur to reduce noise
blurred =cv2.GaussianBlur(img, (5,5),0)
# Detect edges using Canny
edges = cv2.Canny(blurred, 50, 150) #Adjust threshold values as needed
# Plot the original image and the detected edges
plt.figure(figsize=(10,5))
plt.subplot(121),plt.imshow(img, cmap='gray')
plt.title('Original Image'), plt.axis('off')
plt.subplot(122),plt.imshow(edges, cmap='gray')
plt.title('Detected Edges'), plt.axis('off')
plt.show()
```
## OUTPUT
<img width="699" height="427" alt="download" src="https://github.com/user-attachments/assets/ffdf59fe-06b4-4cd9-aa4b-a58a28033f8f" />
