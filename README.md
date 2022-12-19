# Hi Babes <3 Here is a virtual bowl of sweets for you!
## Grab your chocolate of the day and I hope that makes your day!

I actually do NOT know how to code but here is me trying :/

![](kiss.jpg)

//2) randomly select one of these sayings using floor() and random()
//3) display this saying both in the console and on the canvas using console.log() and text()

let fortunes = [
  "A cynic is only a frustrated optimist.",
  "We don't know the future, but here's a cookie.",
  "The road to riches is paved with homework.",
  "He who laughs at himself never runs out of things to laugh at.",
  "Avoid taking unnecessary gambles. Lucky numbers: 12, 15, 23, 28, 37",
  "That wasn't chicken.",
  "All fortunes are wrong except this one.",
  "Don't forget you are always on our minds.",
  "Don't eat the paper.",
  "You have rice in your teeth.",
  "Ask your mom instead of a cookie.",
  "This cookie contains 117 calories.",
  "You think it's a secret, but they know.",
  "Do not mistake temptation for opportunity."
];
let choice = 0;
let displayFortune;

function setup() {
  createCanvas(400, 400);
  //choice = floor(random(0, 16));
  displayFortune = fortuneGen();
}

function draw() {
  background(220);

  console.log(displayFortune);

  textAlign(CENTER);
  text('Your fortune is:', width / 2, 25);
  text(displayFortune, width / 2, height / 2);
  text('refresh for a new fortune!', width / 2, height - 25);
}

function fortuneGen() {
  choice = floor(random(0, 16));
  return fortunes[choice];
}
