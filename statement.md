# Welcome!

This C# template lets you get started quickly with a simple one-page playground.

```C# runnable
// { autofold
using System;

class Hello 
{
  Click here to add your code snippet. private List<Circle> Snake = new List<Circle>(); 
        private Circle food = new Circle(); 
 
        public Form1() 
        { 
            InitializeComponent(); 
 
            //Set settings to default 
            new Settings(); 
 
            //Set game speed and start timer 
            gameTimer.Interval = 1000 / Settings.Speed; 
            gameTimer.Tick += UpdateScreen; 
            gameTimer.Start(); 
 
            //Start New game 
            StartGame(); 
        } 
 
        private void StartGame() 
        { 
            lblGameOver.Visible = false; 
 
            //Set settings to default 
            new Settings(); 
 
            //Create new player object 
            Snake.Clear(); 
             
            Circle head = new Circle(); 
            head.X = 10; 
            head.Y = 5; 
            Snake.Add(head); 
 
 
            lblScore.Text = Settings.Score.ToString(); 
            GenerateFood(); 
 
        } 
        }
```

# Advanced usage

If you want a more complex example (external libraries, viewers...), use the [Advanced C# template](https://tech.io/select-repo/386)
