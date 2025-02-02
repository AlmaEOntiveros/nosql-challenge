# nosql-challenge

The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. You've been contracted by the editors of a food magazine, Eat Safe, Love, to evaluate some of the ratings data in order to help their journalists and food critics decide where to focus future articles.

Requirements
Part 1: Database and Jupyter Notebook Set Up (15 points)
To receive all points, your Jupyter notebook setup file must have all of the following:
Include the mongoimport command text you used to import establishments.json in a markdown cell at the beginning of your Jupyter notebook file (3 points)

The mongoimport command text correctly drops any existing establishments collection before importing establishments.json into MongoDB (2 points)

The database is named uk_food and the collection is named establishments (2 points)

Correctly imports PyMongo and Pretty Print (2 points)

An instance of the Mongo Client is created (1 point)

Lists the databases you have in Mongo, which includes uk_food (1 point)

Lists the collection(s) in the uk_food database, which includes establishments in the output (1 point)

Uses find_one() and pprint to display one document in the establishments collection (2 points)

The establishments collection is assigned to a variable (1 point)

Part 2: Update the Database (20 points)
To receive all points, your Jupyter notebook setup file must have all of the following:
The supplied data for the "Penang Flavours" restaurant is correctly inserted into the establishments collection (3 points)

A query is performed to find the BusinessTypeID for "Restaurant/Cafe/Canteen" and returns only the BusinessTypeID and BusinessType fields (3 points)

The "Penang Flavours" document is updated with the correct value for BusinessTypeID (3 points)

A query is correctly performed to delete all the documents in the collection where "Dover Local Authority" is the value for LocalAuthorityName (3 points)

A count_documents() check is performed before and after the removal of the Dover documents to ensure the documents were removed (4 points)

An update_many() query is performed to convert the latitude and longitude fields from strings to decimal numbers and RatingValue to integers (4 points)

Part 3: Exploratory Analysis (55 points)
To receive all points, your Jupyter notebook analysis file must have all of the following:
Question 1: Which establishments have a hygiene score equal to 20? (8 points)

A query is correctly performed to find the establishments with a hygiene score of 20 (2 points)

count_documents() is used to list the correct number of documents (answer: 41) (2 points)

The first result is printed using pprint (2 points)

The results are converted to a Pandas DataFrame and displays the first 10 rows (2 points)
