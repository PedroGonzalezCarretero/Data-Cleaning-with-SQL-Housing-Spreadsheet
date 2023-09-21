Data Cleaning with SQL - Housing Spreadsheet
Introduction

This repository contains SQL code for cleaning and transforming data from a housing spreadsheet. The code is aimed at improving the quality and usability of the dataset.
Author

    Pedro González Carretero

Instructions

The provided SQL code performs several data cleaning and transformation tasks on the housing spreadsheet.
Step 1: Date Conversion

The initial code attempts to convert the 'SaleDate' column to a proper date format. However, it mentions that this won't work and suggests using the 'ALTER TABLE' statement to create a new field 'SaleDateConverted' with the correct date format.
Step 2: Populating Missing Property Addresses

The code identifies missing property addresses and fills them in using available data. It first identifies records with missing addresses and then updates them by matching them with records that have the same 'ParcelID' but a different 'UniqueID'.
Step 3: Breaking Down Address into Individual Columns

The code splits the 'PropertyAddress' column into separate 'Address' and 'City' columns for better data organization.
Step 4: Breaking Down Owner Addresses into Individual Columns

Similarly, the code splits the 'OwnerAddress' column into 'Address,' 'City,' and 'State' columns to make it more structured.
Step 5: Changing 'Y' and 'N' to 'Yes' and 'No'

The code converts values in the 'SoldAsVacant' column from 'Y' to 'Yes' and from 'N' to 'No' for clarity.
Step 6: Removing Duplicates

The code removes duplicate records from the dataset based on specific criteria using a Common Table Expression (CTE).
Step 7: Deleting Unused Columns

Finally, the code deletes unused columns ('OwnerAddress,' 'TaxDistrict,' 'PropertyAddress') to streamline the dataset.
Usage

You can use this SQL code to clean and transform similar housing datasets. Make sure to adapt it to your specific dataset's structure and requirements.
