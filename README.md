# nosql-challenge

**Eat Safe, Love - Food Hygiene Rating Analysis**


**Project Overview**

The Eat Safe, Love project is a comprehensive codebase designed to assist the editors of the renowned food magazine, Eat Safe, Love, in evaluating food hygiene ratings across the United Kingdom. This codebase empowers journalists and food critics by providing insightful data analysis, allowing them to make informed decisions about which establishments to focus on for future articles.



**Part 1: Database and Jupyter Notebook Setup**

This section of the codebase ensures a seamless setup for data analysis.

**Database Import:** The code imports the establishments data provided in the establishments.json file into a MongoDB database named "uk_food" and a collection named "establishments". This enables easy access and manipulation of the data within a powerful NoSQL database.

**Library Import:** The necessary libraries, PyMongo and Pretty Print (pprint), are imported to facilitate database operations and ensure visually appealing output.

**MongoDB Connection:** An instance of the Mongo Client is created to establish a connection with the MongoDB server. This connection is essential for retrieving and updating data in the database.

**Database Confirmation:** The code verifies the successful creation of the database and data import by listing the available databases and collections. It also displays one document from the "establishments" collection to confirm the data's presence and integrity.



**Part 2: Update the Database**

This section focuses on fulfilling the specific modifications requested by the editors to refine the database before conducting queries and analysis.

**Including a New Restaurant:** An exciting new halal restaurant in Greenwich is identified and needs to be included in the analysis. The code determines the BusinessTypeID for "Restaurant/Cafe/Canteen" and updates the new restaurant's information accordingly. This ensures comprehensive coverage of relevant establishments in the analysis.

**Excluding Establishments in Dover:** The editors express no interest in establishments located in Dover. To accommodate this request, the code checks the number of documents associated with the Dover Local Authority. It then removes these establishments from the database, ensuring that the resulting dataset aligns with the editors' preferences.

**Correcting Data Types:** Some numeric values in the database are stored as strings instead of their appropriate numeric data types. The code resolves this issue by employing update_many operations to convert the latitude and longitude fields to decimal numbers. Additionally, it ensures the RatingValue field is stored as integer numbers for seamless data analysis.



**Part 3: Exploratory Analysis**

This section unleashes the full potential of the Eat Safe, Love project by performing in-depth exploratory analysis on the food hygiene rating dataset.

**Analyzing Rating Values:** The code explores the RatingValue field, which represents the overall rating assigned by the Food Authority on a scale of 1 to 5. This analysis provides valuable insights into the quality and cleanliness of establishments.

**Location Selection and Avoidance:** Eat Safe, Love aims to identify locations that are worth visiting and those that should be avoided. The code addresses this by answering specific questions posed by the magazine. Through comprehensive analysis and data-driven decision-making, it provides guidance to journalists and food critics on the best establishments to focus on for future articles.


By leveraging this well-structured and meticulously maintained codebase, Eat Safe, Love's team of professionals can effectively navigate the realm of food hygiene ratings, ensuring captivating content that aligns with their editorial vision.


Throughout this project, I drew upon an array of reputable resources, including YouTube tutorials, w3schools, learnpython.com, geeksforgeeks.org, flexiple.com, and simplilearn.com. These sources bolstered my technical expertise and enriched the quality of my work.


If you have any further inquiries or would like to learn more about the Eat Safe, Love project, please feel free to reach out.
