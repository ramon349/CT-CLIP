
# Missing data_ifnerence_nii 
-  zeroshot.py: 15 attempts import of data_inference_nii which does not exist 
- replaced with reular data_inference 

# Incorrect requirements file 
- transformers==4.30.1
- one of the packages has the transformers package requirement removed. we need 4.30.1 to load weights properly 


# ignoring some of the preprocessing 
- i am using monai transforms instead for simplicity and we do not have storage for the entire datasets 
-  Intensity clipping  has uncesseary steps 
-  clip images to be [-100,200].  Scale that intensity to be -1 to 1 
- the permuations end up producing the same orientation as your original volume so i'm keeping that the same. 
- i may need to change from RAS to some other orientation