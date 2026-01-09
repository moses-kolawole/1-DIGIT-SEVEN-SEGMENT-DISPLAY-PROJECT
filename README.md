# 1-Digit Seven Segment Display – Arduino Project

## Overview

This project is about displaying numbers from 0 to 9 on a 1-digit seven segment display using an Arduino.
It helped me understand how to control multiple Arduino pins at the same time and how to show numbers visually.

## Project Description

This project basically helps to display numbers ranging from 0 to 9.
It is one of my beginner Arduino projects and focuses on multi-pin digital output, timing, and proper component connection.

## Components Used
- Arduino board
- 1-digit seven segment display (Common Cathode)
- Breadboard
- Jumper wires

## Connections
- Each segment of the display is connected to a digital pin on the Arduino
- All pins are set as OUTPUT in the setup() function
- To display a number, the program turns ON the required segments
- After a short delay, the next number is displayed, and the process repeats

### Note
- The delay between numbers can be adjusted depending on how fast you want the numbers to change.
- Each number requires specific segments to be ON. For example, to display "1," only segments B and C are turned on.

## Alternative Connection
- You could also make a seven segment display manually using separate LEDs for each segment.

- ⚠️ Important: This method requires more resistors, more jumper wires, and more digital pins.

- Using a ready-made 7-segment display is easier and cleaner.

## How It Works
- Each pin connected to a segment is set as OUTPUT
- The Arduino turns ON the required segments for each number
- A delay is added so the number can be seen
- Then the segments are turned OFF
- Another delay is added
- This repeats for numbers 0–9 continuously

## Code Structure
- In the setup() function, I set all the pins connected to the display as OUTPUT
- In the loop() function, the code:
   - Turns ON the required segments for a number
   - Waits (delay_time)
   - Turns OFF the segments
   - Waits again
   - This repeats from 0 to 9 continuously

## Challenges Faced

One major challenge was knowing the difference between Common Cathode and Common Anode seven segment displays.
After research and watching YouTube videos, I discovered my display was Common Cathode and adjusted the code accordingly.
I also had to make sure wiring was correct and no pins were shorted, and manage timing so the numbers changed smoothly.

## Results & Behaviour

## Circuit images / video: 

![Project Images](images/1digit_seven_segment_photo_1.jpg)

Demo video: [Click Here For the Video](video/1digit_seven_segment_display_video.mp4)

- The display counts correctly from 0 to 9 and repeats continuously.

## What This Project Taught Me

- This project helped me understand how to control multiple outputs at the same time using an Arduino.
- It also taught me how timing and delays work to show numbers, which is useful for projects like digital counters or countdowns.

## Code

The Arduino code for this project is [HERE](code/7_SEGMENT_DISPLAY_COUNTER.ino)

## Project Status

Completed ✅
