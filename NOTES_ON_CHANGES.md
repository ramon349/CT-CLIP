
# Missing data_ifnerence_nii 
-  zeroshot.py: 15 attempts import of data_inference_nii which does not exist 
- replaced with reular data_inference 

# Incorrect requirements file 
- transformers==4.30.1
- one of the packages has the transformers package requirement removed. we need 4.30.1 to load weights properly 
