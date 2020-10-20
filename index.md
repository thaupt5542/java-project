## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/thaupt5542/java-project/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

# musical-pancake
Web Development Class Project 1

<html lang="en">
<body style="background-color:lightgray;">
  
 <h1>User Problem:</h1>
 <p>I want to address the problem many pet owners have when it comes to handling their pets. There is no readily accessible site or app that allows pet owners to easily keep track of pet medical records or determine what kind of food is good or bad for the pet. It can include a place for setting reminders on taking the pet in for check-ups, connected to local pet stores via maps, and allow for categorizing the type of pet. This site would provide training plans for dogs and any additional information people may look for when considering getting a pet.</p>
 
 <h1>Users:</h1>
 <p>The users are any people who own pets or are looking into getting one.</p>
 
 <h1>Comparison:</h1>
 <p>The more popular pet stores, such as Pet Smart, have their own sites for displaying some ofthis information and for booking appointments. However, this idea is very different from what is currently out there while taking ideas from other, similar sites.</p>

<h1 style="text-align:center;">Pet&Co</h1>
<p style="text-align:center; border: 2px solid DodgerBlue;"><strong>Petting Zoo</strong></p>

<p style="font-family:courier;">
<span style='font-size:width:42px;height42px;'>&#128512;</span>
</p>

<p style="text-align:center;">
<iframe src="https://giphy.com/embed/gpXfKa9xLAR56" width="480" height="320" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/cheezburger-applause-gpXfKa9xLAR56"></a> 


<p><button type="button"
onclick="document.getElementById('demo').innerHTML = Date()">
Click me to display Date and Time.</button>
<p id="demo"></p>


<address>
Theresa Haupt<br> 
Visit us at:<br>
Haverford College<br>
USA
</address>
<p> <span style="font-size:500%;color:red;">&hearts;</span> </p>


</body>

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](https://www.petsmart.com/) and ![Image](src)
```

For more details see [Pet Smart Home Page](https://www.petsmart.com/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/thaupt5542/java-project/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.


</head>
<meta charset="utf-8">

    <title>Number guessing game</title>

    <style>
      html {
        font-family: sans-serif;
      }

      body {
        width: 50%;
        max-width: 800px;
        min-width: 480px;
        margin: 0 auto;
      }

      .lastResult {
        color: white;
        padding: 3px;
      }
    </style>
  </head>

  <body>
    <h1>Number guessing game</h1>

    <p>We have selected a random number between 1 and 100. See if you can guess it in 10 turns or fewer. We'll tell you if your guess was too high or too low.</p>

    <div class="form">
      <label for="guessField">Enter a guess: </label>
      <input type="text" id="guessField" class="guessField">
      <input type="submit" value="Submit guess" class="guessSubmit">
    </div>

    <div class="resultParas">
      <p class="guesses"></p>
      <p class="lastResult"></p>
      <p class="lowOrHi"></p>
    </div>

    <script>

      let randomNumber = Math.floor(Math.random() * 100) + 1;

const guesses = document.querySelector('.guesses');
const lastResult = document.querySelector('.lastResult');
const lowOrHi = document.querySelector('.lowOrHi');

const guessSubmit = document.querySelector('.guessSubmit');
const guessField = document.querySelector('.guessField');

let guessCount = 1;
let resetButton;
<div class="resultParas">
  <p class="guesses"></p>
  <p class="lastResult"></p>
  <p class="lowOrHi"></p>
</div>
<label for="guessField">Enter a guess: </label><input type="text" id="guessField" class="guessField">
<input type="submit" value="Submit guess" class="guessSubmit">

}function checkGuess() {
  let userGuess = Number(guessField.value);
  if (guessCount === 1) {
    guesses.textContent = 'Previous guesses: ';
  }
  guesses.textContent += userGuess + ' ';
 
  if (userGuess === randomNumber) {
    lastResult.textContent = 'Congratulations! You got it right!';
    lastResult.style.backgroundColor = 'green';
    lowOrHi.textContent = '';
    setGameOver();
  } else if (guessCount === 10) {
    lastResult.textContent = '!!!GAME OVER!!!';
    setGameOver();
  } else {
    lastResult.textContent = 'Wrong!';
    lastResult.style.backgroundColor = 'red';
    if(userGuess < randomNumber) {
      lowOrHi.textContent = 'Last guess was too low!';
    } else if(userGuess > randomNumber) {
      lowOrHi.textContent = 'Last guess was too high!';
    }
  }
 
  guessCount++;
  guessField.value = '';
  guessField.focus();
}
guessSubmit.addEventListener('click', checkGuess);

    </script>
  </body>
<body>
<h1>Hello World</h1>
<p>I'm learning how to use GitHub Pages.</p>
</body>
</html>
