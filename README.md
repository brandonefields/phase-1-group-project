# Quizology
============

## Summary
Quizology is a trivia game which has fun & curious facts. No particular theme was chosen for the questions but some resounding themes are soccer and space. Players are presented with a trivia question on a card and multiple choice answers. After an answer is selected, the player is informed of whether their selection is right or wrong and given the option to move on to the next question or quit.

## Technologies

* [HTML5] (https://www.w3schools.com/html/) 
    ![HTML5 Logo](https://www.w3.org/html/logo/img/mark-word-icon.png)
* [JavaScript] (https://developer.mozilla.org/en-US/docs/Web/JavaScript)
    ![JavaScript Logo](https://upload.wikimedia.org/wikipedia/commons/6/6a/JavaScript-logo.png)
* [CSS3] (https://www.w3schools.com/css/) 
    ![CSS3 Logo](https://upload.wikimedia.org/wikipedia/commons/d/d5/CSS3_logo_and_wordmark.svg)

## Setup
Clone(`git clone`) this repo to your local machine. Navigate(`cd <subdirectory name>`) into the newly created directory. 

### Set up your backend
All of the questions/answers data is stored in the `db.json` file. To use this file, if you don't already have a JSON server, in your terminal run `npm install -g json-server`. Then run `json-server --watch db.json`. 

### Set up your front-end
Open another window in your terminal and navigate into the directory where the game files live, aka the newly crated directory after this repository was cloned. Run `lite-server`, the game should open in your browser.

## Features
* Flipping card animation revealing results of selection
    (Gif here)

* Keep tracks of points and updates with every question answered
    (Gif here)

* Players can add their own questions to the game for a more personalized experience
    (Gif here). 

## Code Snippets
Randomizes answers so they're not in the same position when the same question loads:
```javascript
function shuffleArray(arr) {
  let remainingIndices = arr.length;

  while (0 !== remainingIndices) {
    let randIndex = Math.floor(Math.random() * remainingIndices);
    remainingIndices -= 1;

    let tempArr = arr[remainingIndices];
    arr[remainingIndices] = arr[randIndex];
    arr[randIndex] = tempArr;
  }
  return arr;
}
```

## Expansions


## Status


## Contributors
* [Brandon](https://github.com/brandonefields)
* [Danny](https://github.com/dannyirwin)
* [Michael](https://github.com/stevemr77)



