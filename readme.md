import numpy as np
import cv2

#img=cv2.imread('/home/satish/Desktop/apple.png',cv2.IMREAD_GRAYSCALE)
#cv2.imshow('image',img)
#cv2.waitKey(0)
#cv2.destroyAllWindows()

img=cv2.imread('/home/satish/Desktop/apple.png',cv2.IMREAD_GRAYSCALE)
cv2.imshow('image',img)
k=cv2.waitKey(0)
print(k)
if k==27:
	cv2.destroyAllWindows()
elif k==ord('s'):
	cv2.imwrite('save.png',img)
	cv2.destroyAllWindows()

