# Business Inventory Management
## Summary🖊️
### The dataset contains Inventory log of equipments with their respective details including Item code, Description, Category, Quantity, and so on... Some items are categorized into categories like A, B, C, or D, and their availability and other details are mentioned accordingly.

![Dataset](https://github.com/Shruti-Nagar/pictures/blob/main/Business%20Inventory%20Report/Pending.jpg)

The columns "Retail Price," "Below Min," "Reorder?," "Reorder Qty a," and "Reorder Qty b" contain the following information:
#### Retail Price: The price at which the item is sold to customers.
#### Below Min: Indicates whether the quantity of the item in stock is below the minimum threshold.
#### Reorder?: Indicates whether the item needs to be reordered.
#### Reorder Qty : The quantity to reorder if the item falls below the minimum threshold.

These are the formulas I used to calculate required fileds and I also used "Name Manager" (Formulas Tab < Create from Selection) for quick calculations.
![Section 1](https://github.com/Shruti-Nagar/pictures/blob/main/Business%20Inventory%20Report/Formula%201.jpg)
![Name Manager](https://github.com/Shruti-Nagar/pictures/blob/main/Business%20Inventory%20Report/Name_Manager.jpg)

These are few other data which are used for lookup functions to calculate various parameters like Postage, Reorder Quantity etc...
![Lookup Arrays](https://github.com/Shruti-Nagar/pictures/blob/main/Business%20Inventory%20Report/Lookup%20Data.jpg)

### This showcases a list of prospective items that have been ordered, including details such as item code, description, category, quantity ordered, cost per unit, postage per unit, and total cost.

![Section 2](https://github.com/Shruti-Nagar/pictures/blob/main/Business%20Inventory%20Report/Formulas%202.jpg)
#### Item No. - Using IF logical function
#### Item Code - Data Validation (Data Tab < Data Validation < List)
#### Details/ Description - VLookUp, it matches data in "Item Code" and looks into Inventory sheet for Detals.
#### Category - Data Validation(A,B,C&D)

![Section 3](https://github.com/Shruti-Nagar/pictures/blob/main/Business%20Inventory%20Report/Formulas%203.jpg)
#### Cost/Unit - VLookUp, It matches data in "Item code" and looks into "Retail Price" Column
#### Postage/Unit - Index to return value of a specific row and column of a range & Match searches for specified value in a relative position
#### Total Cost - (Cost + Postage) * Units


## Below are the Final Project Snippets
![Completed Inventory](https://github.com/Shruti-Nagar/pictures/blob/main/Business%20Inventory%20Report/Inventory%20Log.jpg)
![Quotes](https://github.com/Shruti-Nagar/pictures/blob/main/Business%20Inventory%20Report/Prospective%20Orders.jpg)
