# nosql-challenge
Repository for my module 12 MongoDB/noSQL challenge.

## Overview

For this challenge, I've been contracted by the editors of a food magazine to evaluate the UK Food Standards Agency Ratings Data for establishments to help decide where to focus future articles.

This challenge will be delivered in two parts:
    Deliverable 1: A Jupyter notebook containing code that imports the data and sets up and updates the uk_food database.
    Deliverable 2: A Jupyter notebook containing code that performs the exploratory analysis queries in the database.

# Deliverable 1

## Part One

For the first part of deliverable one, I focused on importing the data and setting up Pymongo in order to update the database. I did the following:
    Imported the establishments.json file from the terminal into a MongoDB database as 'uk_food' and a collection as 'establishments'
    Imported the necessary libraries
    Created an instance of Mongo Client
    Confirmed the database and collection were properly imported
    Assigned the 'establishments' collection to a variable


## Part Two

For the second part of deliverable one, I updated the Database with modifications requested by the magazine. I made the following changes:
    Added Penang Flavours document to the collection
    Found the BusinessTypeID for Restaurant/Cafe/Canteen and returned it
    Updated Penang Flavours with the found BusinessTypeID
    Removed all establishments in the Dover Local Authority
    Converted latitude and longitude values from a string to a double


# Deliverable Two

For deliverable two, I used the updated collection to answer the following questions for the magazine:
    Which establishments have a hygiene score equal to 20?
    Which establishments in London have a RatingValue greater than or equal to 4?
    What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygine score, nearest to the new restaurant added, "Penang Flavours"
    How many establishments in each Local Authority area have a hygiene score of 0 with the results sorted from highest to lowest.