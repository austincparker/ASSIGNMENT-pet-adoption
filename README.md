# Adoption Website

## Deployed App

https://github.com/katherinevfry/sorting-hat

## Overview of the Project

This was our first project where we rendered to the DOM. We were given an array of objects (pets) and asked to design an app that displayed those objects in bootstrap cards. We were also asked to add filtering functionality and delete functionality.

## Screenshot of Project

https://github.com/austincparker/ASSIGNMENT-pet-adoption/blob/main/pet-adoption-ss.jpg

## List of Features

- Populated cards of animals up for adoption complete with a photo, special skill, color, and name.
- Buttons to filter cards by animal type.
- Button to delete each card.


## Steps in Project

- Created all html css js files and linked them.
- Created div elements in html file and added appropriate ids.
- Created forEach loops to cycle through pets array and print to dom
- Did some styling to make sure the boxes displayed correctly.
- Created a function to add a "typeColor" to each object in the pets array depending on what type of animal it is. Called this function in init before the petBuilder function. This is how I got each card to display the right color at the bottom. 

Code Snippet: 

`const addTypeColor = (petsArray) => {
  petsArray.forEach((pet) => {
    if (pet.type === "cat") {
      pet.typeColorBkg = "lightblue";
      pet.typeColorTxt = "royalblue";
    } 
    if (pet.type === "dog") {
      pet.typeColorBkg = "lightgreen";
      pet.typeColorTxt = "forestgreen";
    } 
    if (pet.type === "dino") {
      pet.typeColorBkg = "lightyellow";
      pet.typeColorTxt = "goldenrod";
    } 

  });

};`

- Did some more styling to make it look pretty.
- Added a non-functional 'delete' button.
- Added filtering functionality to the top buttons. (yay, it worked)
- Added delete functionality using event.target.outerText to select the 'Delete' button.



## Loom: 

https://www.loom.com/share/a48ca13e425b4e73a177871aa7085bf3
