---
title: "RACHEL: Project Description"
date: 2022-12-04T15:59:37-05:00
author: "Team RACHEL"
draft: false
---

Project R.A.C.H.E.L. is an enhancement to the original game of table tennis. Users will no longer need to keep track of their own score; using a contact microphone array, R.A.C.H.E.L. determines when the ball has bounced, which side of the table it bounced on, and thus, can detect erroneous bounces. In real-time, the score will be displayed on the table, using an overhead projector system. The users can interact with the system through a button matrix, to start and end games, change the scoring mode, and make other preferential modifications to customize the R.A.C.H.E.L. experience.

As a stretch goal, we intend to extend R.A.C.H.E.L. to incorporate a selection of minigames and display modes. Using a camera above the table, we intend to track the ball in real-time. This would allow for games that require the user to hit the ball onto specified parts of the table, highlighted by the projector. Or the user could display the ball’s motion trail to view their play patterns. Similarly, we intend to interface the camera to track hand gestures, which could also be used for user input to the game. Finally, we hope to determine, within a few inches, where the ball has bounced on the table, exclusively using the piezoelectric sensors.

### PSSCs

  1. (Hardware): An ability to handle 2-way communication between a microcontroller and a laptop through UART.
  2. (Hardware): An ability to read key presses from a 4x4 keypad matrix.
  3. (Hardware): An ability to amplify analog signals from contact microphones.
  4. (Software): An ability to interpret microphone inputs to infer the score.
  5. (Software): An ability to read multiple inputs through 1 ADC controller with a circular buffer.


### Stretch Goals

  1. (Hardware): An ability to accurately track the ball within a 6"x6" square, with a delay of under a second, using a microphone array.
  2. (Software): An ability to accurately track the ball within a 6"x6" square, with a delay of under a second, using an overhead camera.
  3. (Software): An ability to detect a paddle hovered over an area of the table to interact with a projected user interface.
  4. (Software): Offer an extra minigame that changes the table as the game is played, based on the ball bounce locations.
    - The table will be divided into a grid of 50 (5 x 10) cells, each with two possible states: fair and foul. Hitting the ball into a fair cell turns it foul, and hitting the ball into a foul cell will give your opponent a point. Each cell is reset to fair after each rally.
