# 1-Digit Seven Segment Display – Arduino Project

## Overview
This project demonstrates how to control a single-digit 7-segment display using an Arduino to show numbers 0–9 sequentially.

## Objective
- Learn how to control multiple Arduino digital pins simultaneously
- Understand the working of a 7-segment display
- Practice sequencing numbers with timing functions
- Gain hands-on experience with multi-pin circuits

## Components Used
- Arduino Uno
- 1-Digit 7-Segment Display (Common Cathode)
- Breadboard
- Jumper wires

## Circuit Diagram
![Circuit Diagrams](images/)

## How It Works
1. Each segment of the 7-segment display is connected to a separate Arduino digital pin through a 220Ω resistor.
2. The Arduino sets each pin as an OUTPUT using `pinMode()`.
3. To display a number, the program turns ON the required segments by writing HIGH to their respective pins.
4. After a short delay, the next number is displayed in sequence.
5. This process repeats continuously inside the `loop()` function.

## Code
The Arduino sketch for this project is located in the [code/directory](code/7_SEGMENT_DISPLAY_COUNTER.ino) directory.

## Demo Video
A demonstration video showing the working project is included in this repository.

📹 **Project Demonstration:**  
[Click here to watch/download the demo video](video/1digit_seven_segment_display_video.mp4)

*(If the video does not preview directly on GitHub, please download it using the link above.)*

## Reflection (What I Learned)
- How to control multiple outputs simultaneously
- How 7-segment displays operate
- Improved understanding of Arduino sketch structure for multi-component circuits

## Challenges Faced
- Ensuring correct segment-to-pin mapping
- Wiring multiple pins without short circuits
- Managing timing for smooth number transitions

## Possible Improvements
- Add a push button to increment numbers manually
- Extend to a 2-digit display for counting beyond 9
- Use arrays or functions to simplify segment control

## Project Status
Completed
