# Sound-Board

This is apart of the 50 projects in 50 days challenge and is the ninth project.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)


## Overview

### The challenge

- To create various buttons that contain different sounds depending on the name of the button. The challenge involves HTML, CSS and Javascript.

### Screenshot

# Mobile Preview 

![screenshot](https://github.com/romila2003/Sound-Board/blob/main/Mobile%20preview.PNG)

# Desktop Preview 

![screenshot](https://github.com/romila2003/Sound-Board/blob/main/Desktop%20preview.PNG)


### Links

 - Source code: [https://github.com/romila2003/Sound-Board](https://github.com/romila2003/Sound-Board)
 - Live website: [https://sound-board-main.netlify.app/](https://sound-board-main.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- Plain CSS
- Vanilla Javascript
- Flexbox

### What I learned

I learned a new concept that allows you to play a sound when clicked and pause the current sound to allow another sound to played, when clicked on a different sound. This concept was very interesting and can provide many useful benefits for future projects that involve sounds.

Javascript - `.play` and `.pause`:

```javascript

sounds.forEach(sound => {
    const btn = document.createElement("button");
    btn.classList.add("btn");

    btn.innerText = sound;

    btn.addEventListener("click", () => {
        stopSongs();

        document.getElementById(sound).play();
    })

    document.getElementById("buttons").appendChild(btn);
})

function stopSongs() {
    sounds.forEach(sound => {
        const song = document.getElementById(sound);

        song.pause();
        song.currentTime = 0;
    })
}

```

### Continued development

For future developments, I should implement the features/concepts learned over the last few projects and future projects, into practical projects/challenges such as the frontendmentor.io projects.


## Author

- Twitter - [@romila003](https://www.twitter.com/romila003)
- Frontend Mentor - [@romila2003](https://www.frontendmentor.io/profile/romila2003)
