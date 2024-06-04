# nosql-challenge
Module 12 Challenge

![restaurant-front-beautiful-building-facade-with-awning-greenery_176411-5877](https://github.com/KrissinaW/nosql-challenge/assets/162597320/5510b993-f4d6-4a12-8f92-2f5e957dd0f2)


# **Overview**

The UK Food Standards Agency evaluates various establishments across the United Kingdom, assigning them food hygiene ratings. You have been contracted by Eat Safe, Love, a food magazine, to analyze these ratings to help their journalists and food critics decide where to focus future articles.

# **Part 1**: Database and Jupyter Notebook Set Up

- Use NoSQL_setup_starter.ipynb for this section.

- Import Data: From your Terminal, import the data provided in the establishments.json file.
Name the database uk_food and the collection establishments.

- Copy the text you used to import your data from your Terminal to a markdown cell in your notebook.
Setup:

- Import necessary libraries: PyMongo and Pretty Print (pprint).

- Create an instance of the Mongo Client.

- Confirm Setup:

- List the databases in MongoDB to confirm that uk_food is listed.
  
- List the collections in the uk_food database to ensure establishments is present.
  
- Use find_one to display one document from the establishments collection using pprint.
  
- Assign the establishments collection to a variable for future use.


# **Part 2**: Update the Database

- Continue using NoSQL_setup_starter.ipynb.

- Add New Restaurant: Insert information for a new halal restaurant in Greenwich into the database.

  *Update Restaurant:

- Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and update the new restaurant document with this ID.

  *Remove Establishments in Dover:

- Count and remove all documents with "Dover" as the LocalAuthorityName.

- Verify the documents have been removed by counting again.

  *Correct Data Types:

- Use update_many to convert latitude and longitude to decimal numbers.

- Convert RatingValue to integers.


#  **Part 3**: Exploratory Analysis

- Use NoSQL_analysis_starter.ipynb for this section.

  * Hygiene Score of 20:

- Find establishments with a hygiene score of 20.
  
- Count and display the number of documents.
  
- Convert the results to a Pandas DataFrame and display the first 10 rows.
  
- London Establishments with High Ratings:

- Find establishments in London with a RatingValue of 4 or more using the $regex operator.
  
- Count and display the number of documents.
  
- Convert the results to a Pandas DataFrame and display the first 10 rows.
  
  *Top 5 Establishments near "Penang Flavours":

- Find the top 5 establishments with a RatingValue of 5, sorted by the lowest hygiene score, near "Penang Flavours".
  
- Display the results and convert them to a Pandas DataFrame.
  
- Hygiene Score of 0 by Local Authority:

- Use an aggregation pipeline to find the number of establishments with a hygiene score of 0, grouped by LocalAuthorityName.
  
- Sort the results from highest to lowest and print the top ten local authority areas.
  
- Convert the results to a Pandas DataFrame and display the first 10 rows.


# **Requirements**

**Part 1:** Database and Jupyter Notebook Set Up

Include the mongoimport command text in a markdown cell.

Ensure the establishments.json is imported correctly.

Database and collection are named correctly.

Libraries imported and Mongo Client created.

Database and collection listed correctly.

find_one and pprint used to display one document.

establishments collection assigned to a variable.

**Part 2:** Update the Database

Insert "Penang Flavours" data correctly.

Query and update BusinessTypeID for the new restaurant.

Delete documents with "Dover" as LocalAuthorityName.

Perform count_documents before and after deletion.

Convert latitude, longitude, and RatingValue to correct data types.

**Part 3:** Exploratory Analysis

Correct queries and counts for each question.

Proper use of pprint and conversion to Pandas DataFrames.

Correct aggregation pipeline and sorting for the final question.

Deployment and Submission

Submit a link to a GitHub repository containing your files.

Use the command line to add files to the repository.

Include appropriate commit messages.
