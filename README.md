# NoSQL challenge

Analyze food hygiene ratings data from the UK Food Standards Agency. Goal is to load this data into a NoSQL database (MongoDB), so it can be used to help journalists and food critics from the magazine Eat Safe, Love decide which establishments to focus on for future articles.

NoSQL_setup:
Part 1: Database and Jupyter Notebook setup
# Import data from terminal
# Import dependencies
# Create an instance of MongoClient
# Confirm the new database was created
# List the database
# Assign the uk_food database to a variable name
# Review the collections in our new database
# Review a document in the establishments collection
# Assign the collection to a variable
Part 2: Update the Database
# Create a dictionary for the new restaurant data
# Insert the new restaurant into the collection
# Check that the new restaurant was inserted
# Find the businessTypeID "Restaurant/cafe/Canteen" and return only the BusinessTypeID and BusinessType fields
# Update the new restaurant with the BusinessTypeID
# Confirm that the new restaurant was updated
# Find how many documents have LocalAuthorityName as "Dover"
# Delete all documents where LocalAuthorityName is "Dover"
# Check if any remaining documents include Dover
# Check that other documents remain with 'find_one'
# Change the data type from String to Decimal for longitude and latitude
# Check that the latitude and longitude fields are now decimals
# Set non 1-5 Rating Values to Null
# Change the data type from String to Integer for RatingValue
# Check that the RatingValue field is now an integer
# Check that the coordinates and rating value are now numbers

NoSQL_analysis:
Notebook set up
# Import dependencies
# Create an instance of MongoClient
# assign the uk_food database to a variable name
# review the collections in our database
# assign the collection to a variable
Part 3: Exploratory Aanalysis
1. Which establishments have a hygiene score equal to 20?
# Find the establishments with a hygiene score of 20
# Use count_documents to display the number of documents in the result
# Display the first document in the results using pprint
# Convert the result to a Pandas DataFrame
# Display the number of rows in the DataFrame
# Display the first 10 rows of the DataFrame
2. Which establishments in London have RatingValue greater than or equal to 4?
# Find the establishments with London as the Local Authority and has a RatingValue greater than or equal to 4.
# Use count_documents to display the number of documents in the result
# Display the first document in the results using pprint
# Convert the result to a Pandas DataFrame
# Display the number of rows in the DataFrame
# Display the first 10 rows of the DataFrame
3. What are the top 5 establishments with RatingValue rating value of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
# Search within 0.01 degree on either side of the latitude and longitude.
# Rating value must equal 5
# Sort by hygiene score
# Define the limit for top 5 results
# Perform the query and retrieve the results
# Print the results
# Convert result to Pandas DataFrame
# Display the DataFrame
4. How many establishments in each Local Authority area have a hygiene score of 10?
# Create a pipeline that:
 # 1. Matches establishments with a hygiene score of 0
 # 2. Groups the matches by Local Authority
 # 3. Sorts the matches from highest to lowest
# Run the pipeline
# Print the number of documents in the result
# Print the first 10 results
# Convert the result to a Pandas DataFrame
# Display the number of rows in the DataFrame
# Display the first 10 rows of the DataFrame
