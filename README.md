# unc-to-cle
Preprocessing and analyzing a dataset found on kaggle.
# Summary of the dataset
The dataset contains 4,525 entries and 11 columns, all of which are of type object. Here's a detailed summary:

property_name: Name and type of the property (4,525 unique entries).
areaWithType: Type of area measurement (e.g., Super Area, Carpet Area).
square_feet: Area of the property in square feet, with values in the format of xxx sqft.
transaction: Type of transaction (e.g., Resale, New Property). This column has 4421 non-null entries, indicating some missing values.
status: Status of the property (e.g., Ready to Move). It has 4524 non-null entries.
floor: Information about the floor, with entries like 5 out of 10. This column has some missing values as well.
furnishing: Furnishing status of the property (e.g., Unfurnished, Semi-Furnished). Contains some missing values.
facing: Direction the property faces (e.g., East, West). Missing values are present here.
description: Descriptions of the properties, which are highly variable and text-heavy.
price_per_sqft: Price per square foot, with values in the format of ₹xxxx per sqft. This column also contains missing values.
price: Total price of the property, with various formats including ₹xx Lac and Call for Price.