# SQL-Data-Cleaning-Exploratory-Data-Analysis

# The project involves cleaning property sales data for further analysis using SQL
# The first step involves changing dates saved in DATETIME format to DATE format using CONVERT command. This is done to enhance readability, remove unnecessary information from the column and save space.
# Thereafter I identify the existence of null values in PropertyAddress field. However, these null values can be populated with data given elsewhere for same properties. I use SELF JOIN technique along with ISNULL command to populate the null values.
# I then move to splitting city and state data from PropertyAddress and OwnerAddress fields into separate columns. For PropertyAddress I utilise SUBSTRING and CHARINDEX. For OwnerAddress I utilise PARSENAME command.
# The SoldAsVacant column recorded affirmations as both 'Y' and 'Yes' and negations as both 'N' and 'No'. For consistency, 'Y' and 'N' are changed to 'Yes' and 'No' using UPDATE & CASE commands.
# Thereafter, I move to identifying duplicate rows using CTE, PARTITION BY, WHERE & ORDER BY commands. These rows are then deleted using the DELETE command.
# Lastly, I drop unnecessary columns using DROP command.
