# Image-Classification-Labeling-Project-Excel-file
Manually labeled images into categories like Dog, Cat, Car, and Bike using annotation tools. Saved annotations in Excel format for model training use. Improved skills in image recognition, attention to detail, and data labeling.

import pandas as pd

# Create a sample image classification dataset description again after code state reset
data = {
    "Image Name": [
        "dog_001.jpg", "dog_002.jpg", "cat_001.jpg", "cat_002.jpg", 
        "car_001.jpg", "car_002.jpg", "bike_001.jpg", "bike_002.jpg"
    ],
    "Class Label": [
        "Dog", "Dog", "Cat", "Cat", 
        "Car", "Car", "Bike", "Bike"
    ],
    "Annotated By": [
        "YourName" for _ in range(8)
    ],
    "Notes": [
        "Clear image", "Side view", "Sitting cat", "Close-up",
        "Front view", "Back view", "Parked", "Moving"
    ]
}

# Create a DataFrame
df = pd.DataFrame(data)

# Save as Excel file
file_path = "/mnt/data/Image_Classification_Labeling_Project.xlsx"
df.to_excel(file_path, index=False)


