# Google-Hashcode-2018-Solution-Online-Qualification-Round
This is an attempt at a solution for Google's Hashcode 2018 Online Qualification Round Problem (Self-driving rides)

## Usage

Most straightforward way to run this code on your machine would be :
* Go to your prefered Java IDE
* Create a project
* Add Java Classes of the same name as the one in the master branch
* Copy and paste the code into the corresponding Class
* Download input.txt and make appropriate changes to directory in World.java line 30
* Build and run project



# What each class does:
## World 
* Contains the bounds (for "city" grid and time steps), number of vehicles, and number of rides.
* Fills an array list with Ride objects. The fields are populated from the input text file. An id is also added to differentiate each ride.
* Fills an array list with Vehicle objects.
* A printList method is present to test the aforementioned functionalities are present.

## Vehicle
* Keeps record of current position of vehicle (on the grid).
* Is assigned a Route which it will follow (functionality yet to be completed).

## Ride
* Keeps record of all parameters of rides from input text file. Also has an id (as it is needed for output).

## Route
* Simply an array list of rides that will be passed to vehicles to follow. Has a boolean field that decides whether or not a new ride can be added to it.

## SortRide
* A class required for sorting an ArrayList of ride objects. Sorts rides be ascending order of **earliest start time**, if two rides can start at the same time, then it checks for **latest finish time**. Collections.sort() requires such a class to be defined.
