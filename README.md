COMPANY NAME : CODTECH IT SOLUTIONS

NAME : S NIVILA

INTERN ID : CT04DF2638

DOMAIN : JAVA

DURATION : 4 WEEKS

MENTOR : NEELA SANTHOSH

🎯 Task 4: Recommendation System

This task focuses on building a simple recommendation system using **Apache Mahout** and Java. It uses collaborative filtering to suggest items to users based on historical preferences. Key components:

- Sample user-item rating dataset
- Apache Mahout’s `DataModel` and `Recommender` classes
- Console output showing item recommendations per user

This project introduces machine learning basics through a hands-on recommendation engine and external library integration.

# AI-Based Recommendation System using Java & Apache Mahout

## Overview

This project demonstrates a Java-based recommendation system built using Apache Mahout, an open-source machine learning library. The system recommends products or content to users based on their preferences using User-Based Collaborative Filtering (UBCF).

The core functionality is built around analyzing user-item interaction data and suggesting items that similar users have shown interest in. It uses Pearson Correlation to measure similarity between users and the k-Nearest Neighbors (kNN) algorithm to determine which users are most similar to each other.

The project is ideal for beginners and intermediate-level developers who want to understand how collaborative filtering works in practice, and how to use Java and Apache Mahout to implement machine learning features.

## Objective

The objective of this project is to:

- Build a working recommendation system using Java.
- Learn and apply collaborative filtering techniques.
- Suggest products or content to users based on user-user similarity.
- Output top-N recommendations with estimated preference values.
- Provide a clean and modular Java codebase that can be extended or integrated with other applications.

## Technologies Used

The core technologies used in this project are:

- Java (JDK 8 or higher) for programming the system logic
- Apache Mahout for recommendation engine components
- CSV file as input dataset containing user-item-rating data
- A terminal or console for running and interacting with the program
- Optional: IntelliJ IDEA, Eclipse, or VS Code as Java IDEs

## How It Works

The system works by reading a dataset containing user ratings of items. It calculates how similar one user is to another using Pearson Correlation. Once the most similar users (neighbors) are found, it recommends items to the target user that their neighbors have rated highly.

Here's the step-by-step process:

1. Load the user-item-rating dataset from a file called `data.csv`.
2. Build a `DataModel` using Apache Mahout’s `FileDataModel`.
3. Compute user similarity using `PearsonCorrelationSimilarity`.
4. Use `NearestNUserNeighborhood` to select the closest 2 users to the target user.
5. Use `GenericUserBasedRecommender` to generate top 3 recommendations.
6. Display the recommended item IDs along with estimated preference scores in the console.

## Project Structure

The main components of the project are:

- `App.java`: The main Java file containing the recommendation logic.
- `data.csv`: The input file containing userId, itemId, and rating.
- `/libs`: A folder (optional) where Mahout JAR files can be stored.
- `README.md`: This documentation.

## Input Data Format

The input data file `data.csv` should be in comma-separated format with each line containing:

Example:

1,101,4.5
1,102,3.0
2,101,4.0
2,103,5.0
3,102,2.5

Each line indicates that a particular user has rated a specific item with a given rating (on a scale such as 1.0 to 5.0). You can expand this dataset with more users and items to experiment with recommendation accuracy.

## Setup and Execution

### Prerequisites

Before running the project, ensure the following are installed:

- Java Development Kit (JDK) 8 or higher
- Apache Mahout core JAR files (add to your classpath)
- A Java IDE (like IntelliJ or Eclipse) or command-line compiler
- `data.csv` file placed in the project directory

### Steps to Run

1. Clone or download the project.
2. Open the project in your IDE or terminal.
3. Ensure `App.java` and `data.csv` are in the same directory.
4. Add Mahout libraries to your classpath.
5. Compile the Java program:

   On macOS/Linux:
   ```bash
   javac -cp .:mahout-core-x.x.x.jar App.java
   
### Learning Outcomes

• By working on this project, you will:

• Understand collaborative filtering concepts and user similarity

• Learn how to use Apache Mahout’s recommender APIs

• Gain experience with Java file I/O and data structures

• Build the foundation for more advanced ML-based systems

•Be equipped to integrate ML models into production applications
