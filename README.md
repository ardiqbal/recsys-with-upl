# recsys-with-upl

In recommendation system research, some authors leverage the use of the user preference list (UPL) in their datasets.
Basically, the UPL denotes how many rated items, exactly, every user should have.
For example, a UPL 5 means that every user should have 5 rated items. Therefore, if there are 100 users, then there should be 500 rating from those users, regardless how many items in space.

This repository contains program to generate the UPL from rating dataset (Here, I use MovieLens dataset).
From the dataset information, each user had rated at least 20 movies.
The program will randomly select n item ratings, where n is the UPL size, for each user.
Therefore, the final UPL dataset will have (number of user) * (UPL size) ratings.
I use 10, 20, 30, 40, and 50 as the UPL size.
