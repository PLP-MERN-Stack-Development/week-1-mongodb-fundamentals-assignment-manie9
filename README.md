[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=19660871&assignment_repo_type=AssignmentRepo)
# MongoDB Fundamentals Assignment

This assignment focuses on learning MongoDB fundamentals including setup, CRUD operations, advanced queries, aggregation pipelines, and indexing.

## Assignment Overview

You will:
1. Set up a MongoDB database
2. Perform basic CRUD operations
3. Write advanced queries with filtering, projection, and sorting
4. Create aggregation pipelines for data analysis
5. Implement indexing for performance optimization

## Getting Started

1. Accept the GitHub Classroom assignment invitation
2. Clone your personal repository that was created by GitHub Classroom
3. Install MongoDB locally or set up a MongoDB Atlas account
4. Run the provided `insert_books.js` script to populate your database
5. Complete the tasks in the assignment document

## Files Included

- `Week1-Assignment.md`: Detailed assignment instructions
- `insert_books.js`: Script to populate your MongoDB database with sample book data

## Requirements

- Node.js (v18 or higher)
- MongoDB (local installation or Atlas account)
- MongoDB Shell (mongosh) or MongoDB Compass

## Submission

Your work will be automatically submitted when you push to your GitHub Classroom repository. Make sure to:

1. Complete all tasks in the assignment
2. Add your `queries.js` file with all required MongoDB queries
3. Include a screenshot of your MongoDB database
4. Update the README.md with your specific setup instructions

## Resources

- [MongoDB Documentation](https://docs.mongodb.com/)
- [MongoDB University](https://university.mongodb.com/)
- [MongoDB Node.js Driver](https://mongodb.github.io/node-mongodb-native/) 




## 🛠️ Setup Instructions

I used MongoDB Atlas for this assignment.
Ensure you have a MongoDB Atlas account and a cluster set up.
Replace the connection string in insert_books.js with your MongoDB Atlas connection string:

const uri = 'mongodb+srv://<username>:<password>@cluster.mongodb.net/';


## Importing Data
Create a books.json File:
I created a books.json file in VS Code containing the sample book data.
Example content of books.json:
[
  {
    "title": "To Kill a Mockingbird",
    "author": "Harper Lee",
    "genre": "Fiction",
    "published_year": 1960,
    "price": 12.99,
    "in_stock": true,
    "pages": 336,
    "publisher": "J. B. Lippincott & Co."
  },
  {
    "title": "1984",
    "author": "George Orwell",
    "genre": "Dystopian",
    "published_year": 1949,
    "price": 10.99,
    "in_stock": true,
    "pages": 328,
    "publisher": "Secker & Warburg"
  }
  // Add more books here
]

## Import Data into MongoDB Compass:

Open MongoDB Compass and connect to your MongoDB Atlas cluster.
Navigate to the plp_bookstore database and create a books collection.
Click on Add Data > Import File.
Select the books.json file and import the data into the books collection.

## Running Queries
Open MongoDB Compass or MongoDB Shell (mongosh).
Navigate to the plp_bookstore database and select the books collection.
Run the queries provided in queries.js:

Example query, Update the price of a specific book
db.books.updateOne({ title: "1984" }, { $set: { price: 9.99 } });

## Verification
Open MongoDB Compass and verify that the books collection contains the sample data.
Take a screenshot of the books collection and include it in your submission. 


