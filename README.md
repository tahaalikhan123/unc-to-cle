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

Missing Values
Here are the columns with missing values:

transaction: 104 missing values
status: 1 missing value
floor: 45 missing values
furnishing: 340 missing values
facing: 589 missing values
description: 1,371 missing values
price_per_sqft: 368 missing values
Handling Missing Values
We will handle missing values using the following strategies:

Drop columns with excessive missing data: For description, we might consider dropping it due to high variability and large number of missing values.
Fill with most frequent or default values: For categorical columns like transaction, status, floor, furnishing, and facing.
Drop rows with missing values in critical columns: Columns like price and square_feet are critical for analysis.