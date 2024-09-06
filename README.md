# NoSQL

# Database and Jupyter Notebook Set Up
1. Created a databse named `uk_food` and a collection `establishments` by importing the data provided in `establishments.json.`

2. Imported the PyMongo and Pretty Print libraries and subsequently created an instance of the Mongo Client.

3. Confirmed that both the database `uk_food` was created and that the data for the `establishments` collection was loaded properly.

4. Used pprint to display one document of the `establishments` collection.

5. Assigned to `establishments` collection to the variable 'establishments'

## Update the Database
1. Inserted supplied data for "Penang Flavours" restaurant into the `establishments` collection.

2. Performed a query to find the "Restaurant/Cafe/Canteen" 'BusinessTypeID', returning only the 'BusinessTypeID' and the 'BusinessType'.

3. Performed queries to delete all documents where the 'LocalAuthorityName' is "Dover" then checked make sure they were, if fact, deleted - using the count_documents() method.

4. Converted the latitude and longitude fields from strings to decimal numbers and the 'RatingValue' to integers - both using the update_many() method. 

## Exploratory Analysis
* Question 1
1. Created a query to find the establishments with a hygience score of 20.

2. Listed the number of documents in the query using the count_documents() method.

3. Printed the first result - using pprint.

4. Converted the results to a Pandas DataFrame, displaying only the first 10 rows.

* Question 2
1. Created a query to find the establishments in London with a RatingValue >= 4.

2. Used the '$regex' operator to obtain the London establishments and the count_documents() method to list the number of documents.
 
3. Printed the first result - using pprint.

4. Converted the results to a Pandas DataFrame, displaying only the first 10 rows.

* Question 3
1. Created a query to find the establishments within 0.01 degree of "Penang Flavours" and with a RatingValue of 5.

2. Sorted the values in ascending order on the hygiene score using the sort() method. 

3. Used the limit() method to limit the results to 5.

4. Printed the first five results - using pprint.

5. Converted the results to a Pandas DataFrame.

* Question 4
1. Worked with a tutor to create an aggregation pipeline to include a match, query, and sort.

2. Set the match query to include documents with a hygience score of zero.

3. Set the group step to group on the 'LocalAuthorityName' and count the number of documents.

4. Set the sort step to sort the count of the documents in descending order.

5. Used the aggregate() method and cast the aggregation query as a list saved to the "results" variable.

6. Printed the first 10 results - using pprint.

7. Converted the results to a Pandas DataFrame, displaying only the first 10 rows.