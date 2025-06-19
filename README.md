import cv2 img = cv2.imread("DFS.png",0) print(img) cv2.imshow("Output", img) cv2.waitKey(0) cv2.destroyAllWindows() # Import OpenCV Package
# Read as Grey Image
# prints the matrix of the pixel
## Show the output image
# Need to Manually Close the window
# Destroy all the windows of cv2 object
2. Reading a colour image
import cv2 img = cv2.imread("lena.jpg",1) print(img) cv2.imshow("Output", img) cv2.waitKey(3000) cv2.destroyAllWindows() 3. Read as a unchanged image
mport cv2 img = cv2.imread("lena.jpg",-1) print(img) cv2.imshow("Output", img) cv2.waitKey(3000) cv2.destroyAllWindows() 4. Writing images
import cv2
img = cv2.imread("lena.jpg",-1)
print(img)
cv2.imshow("Output", img)
cv2.waitKey(5000)
# Import OpenCV Package
# Read as Color Image
# prints the matrix of the pixel
## Show the output image
# Output will wait for 3 seconds
# Destroy all the windows of cv2 object
# Import OpenCV Package
# Read as Unchanged Image
# prints the matrix of the pixel
## Show the output image
# Output will wait for 3 seconds
# Destroy all the windows of cv2 object
cv2.destroyAllWindows()
cv2.imwrite("New-Lena.png",img) #create new image file from img object
import cv2
img = cv2.imread("lena.jpg",-1)
print(img)
cv2.imshow("Output", img)
k = cv2.waitKey(0) & 0xFF
if k==27: cv2.destroyAllWindows()
# If Escape is pressed, it destroy all window
elif k==ord('s'):
cv2.imwrite("New-Lena.png",img) ## If "s" is pressed, it create new image
cv2.destroyAllWindows()
5. Changing the colour space of the image
import cv2 # Import Opencv Package
img = cv2.imread("Car.jpeg",-1) # Read as Unchaged Image
grey = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY) # Convert BGR to Gray
cv2.imshow("Output", grey) ## Show the output image
cv2.waitKey(0) # Output will wait for 3 seconds
cv2.destroyAllWindows() # Destroy all the windows of cv2 object
import cv2 # Import Opencv Package
img = cv2.imread("Car.jpeg") # Read Image
gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY) # Convert BGR to Gray
cv2.imshow("Output", gray) ## Show the output image
BGR1 = cv2.cvtColor(gray, cv2.COLOR_GRAY2RGB)
cv2.imshow("Output1", BGR1)
cv2.waitKey(0) cv2.destroyAllWindows() # Output will wait for 3 seconds
# Destroy all the windows of cv2 obj
