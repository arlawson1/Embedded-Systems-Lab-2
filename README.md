# Embedded-Systems-Lab-2
Using a SPST toggle switch to change between states in a finite-state machine. Switch toggles LEDS and 7-segment display


Lab document below:

ECE 487/587 Spring 2020
Laboratory 2 – Introduction to Digital Input/Output

1.	Introduction
This particular laboratory exercise is to familiarize you with using digital inputs via switches and various types of LED outputs.  

2.	Requirements
In addition to your Arduino platform, IDE, and computer, you will also need the following for this lab:
•	Solderless breadboard
•	1k ohm resistors (other resistor values will also work)
•	LED
•	Wires for use with breadboard
•	Toggle switch
•	Seven-segment display (common anode or common cathode types can be used)

3.	Laboratory Tasks
You are to create a new application that will execute on your Arduino platform based upon the Blink example that is available in the Arduino Examples folder that you downloaded as part of the IDE. 

Your application will use a toggle switch to interface with the user.  The application will operate by controlling the LEDs based upon the position of the toggle switch.  If the user moves the toggle switch to the “on” setting, your application will continuously blink LEDs until new user input is provided.  When the user moves the toggle switch to the “off” setting, the application should stop blinking the LEDs (i.e. turn off both LEDS) until new user input is provided.  It is acceptable for the current state of the LEDs to “complete” before they are turned off.  However, care must be taken to avoid switch bouncing. 

Your application must blink the onboard LED connected to PIN 13 such that the LED is on for 1 second and off for 1 second.  Also, you will construct a circuit on your breadboard that blinks an external (off-board) LED exactly out-of-phase with the onboard LED.  That is, the LED on your breadboard should be off for 1 second (while the onboard LED is on) and on for 1 second (while the onboard LED is off). You are free to use any of the I/O pins available to you for your circuit.  This is basically the same functionality as developed in Lab 1.  The only difference is that instead of controlling the LEDs with user input from the keyboard, now you are controlling them with user input from a toggle switch. 

Your program should count the number of different user inputs (switch changes) and output this count to be displayed using the serial monitor.  This output should only be updated when the switch setting is changed (i.e. there should not be an endless loop of count values printed to the screen).  The output value should be displayed in both decimal and hexadecimal in the following format:
				count = (decimal) 10   (hex) A

Finally, you must add to your circuit a 7-segment display to display the count value in hexadecimal (0 – F).  Your circuit should continuously display the count value using the 7-segment display, and this value should match the output to the serial monitor.  

4.	Grading
Due Date:  02/14/2020 (time determined by TA’s grading times)
No late assignments will be accepted.  

All students must demo/explain their project in the lab (SERC 2005) to the TA, Ben Sawyer, by the deadline.  The assignment will be graded at the time of the demo.  There will be no re-submissions (for each lab attempt), so all debugging is the responsibility of the student (the TA doesn’t have time to help you debug your code!).  Each student will have to sign up for a grading/demo time, and the assigned time is the grading/demo time! No exceptions. Arrive a few minutes early to get set up and get ready for your demo time to begin. We want to stay on schedule, so be ready to go when your time starts. If you miss your demo time, you will receive a grade of zero for the lab attempt, and you will have to resubmit. The signup sheet will be posted in SERC 2005 the week before the lab is due. The TA will schedule all grading activities according to the signup sheet. The TA is not able to schedule independent times outside of those posted on the signup sheet. 

You must turn in a hardcopy of your program during your demo with the grading sheet attached as page 1.  The hardcopy of your code should match the code that is being executed!  If it does not match, your grade for the lab will be zero.  Your code should have a header comment indicating your name, CWID, lab assignment, and other pertinent info. I encourage you to print your code from the Arduino IDE to preserve your formatting, which will be considered as part of the “programming practices” grade.  

I encourage all students to PLAN AHEAD regarding deadlines.  Deadlines are LIMITS not GOALS! All students should plan to get their assignments done with time to spare to avoid missing the deadline and to get a demo time.  You may need to be flexible when trying to get a demo time. Deadlines are judged based upon when the assignment is demoed (i.e. graded), not when a student says he/she is finished.  If the assignment is not graded by the deadline, it will not be accepted and the student will receive a zero for that lab attempt.  

Grading Guidelines that will be used for Lab #2:
Good Programming Practices:
1)	Comments
2)	Indentation
3)	Good/meaningful variable names
4)	Minimum/wise usage of global variables; unnecessary use of variables
5)	Inefficient code

Grade Breakdown:
30 pts – Good programming practices
70 pts – functionality/description of code (ability to explain how your system works)
