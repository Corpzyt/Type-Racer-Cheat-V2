# Type-Racer-Cheat-V2
Go to Inspect Element, then go to console.
```js
var counter = -1;
var firstWord = document.getElementsByClassName("inputPanel")[0].querySelectorAll("span")[0].innerHTML + document.getElementsByClassName("inputPanel")[0].querySelectorAll("span")[1].innerHTML,
restOfText = document.getElementsByClassName("inputPanel")[0].querySelectorAll("span")[2].innerHTML;
var fullText = firstWord.concat(restOfText);
var inputBox = document.getElementsByClassName('txtInput');
(function getString() {
    setTimeout(function() {
        counter++;
        inputBox[0].value += fullText[counter];
        if(counter != fullText.length) {
            getString();
        }
        //adjust the 100 milliseconds for a faster wpm & be undetected by their new system.
    }, 100);
})()
```

# Run this code, and it will auto type.

This is a modified version of aeristhy, using a better counter.
