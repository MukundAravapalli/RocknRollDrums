# Rock n Roll Drums
#### [Completed Project](https://raw.githack.com/MukundAravapalli/RocknRollDrums/main/MukundDrumKit/index.html "Project Link")
## About
The Rock n Roll Drumkit is a banner of drums that can be played by clicking on icons or pressing their assigned keys. 

## Functionality
This program was built using the principles of the Document Object Model which links HTML elements and JavaScript functions. 

By using DOM methods, JavaScript functions can target specific HTML elements in order to only manipulate those elemnts while leaving the rest unchanged. 

```javascript
    document.querySelectorAll(".drum")[i].addEventListener("click", function(){
        var buttonInnerHTML = this.innerHTML;
        makeSound(buttonInnerHTML); 
        buttonAnimation(buttonInnerHTML); 
    }); // document query selector

    document.addEventListener("keydown",function(event){
     makeSound(event.key);
     buttonAnimation(event.key);
    });// document key event 
```
The above code snippit shows an example of the DOM i action. In the first code block, we use the keyword `document.querySelectorAll(".drum")` to target all our HTMl elements with the class `.drum`. 

In the second code block, we use the keyword `document.addEventListener("keydown",function(event)` to tell the program to observe whenever a key is pressed in order to carry out a certain function. 

By using DOM methods, we are able to tell the drum icons to listen to mouse clicks and key presses in order to play a certain sound. 

## Origins
I first learnt how to put together a drum kit using DOM methods through Dr. Angela Yu's [Web Developement Bootcamp](https://www.udemy.com/course/the-complete-web-development-bootcamp/ "Web Developement Bootcamp"). 

After learning the basics, I modified the program by adding my own colors, changing the title, and adding a background. 