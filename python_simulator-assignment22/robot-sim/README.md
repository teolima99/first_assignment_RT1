First assignment for Research track 1 
================================


### How to run the code  ###

To run the code, open the terminal shell, move to the `robot-sim` directory and run: 

$python2 run.py assignment.py



### Pseudocode ###

in the while loop:

if the list is full and contains all 12 items, all tokens are paired
	print("Game over bro..")
	the program ends and exit the loop

if silver is equal to True 
	the robot will search for the silver token
else if 
	the robot will search for the golden token

if no token is detected
	robot turn

else if the current distance to the token is less than 0.4 and the token is silver
	print("OKAY I FOUND IT!!")
	the robot grab the token
	token is added to the list
	robot backs away
	we modify the value of the variable silver

else if the current distance to the token is less than 0.6 and the token is gold
	print("Paired!")
	the robot release the silver token near the golden token
	the golden token is added to the list
	robot backs away
	we modify the value of the variable silver

else if the robot is well aligned with the token
	print("Wait...I'm coming")
	the robot go forward

else if the robot is not well aligned with the token
	print("Left a bit...") or print("Right a bit...")
	the robot turn to the left or to the right

### Possible improvements ###

One of the possible improvements could be: making sure that the robot always finds the token closest to it.

By making a 360-degree turn, the robot could store in a list all the distances to the tokens in the environment, so later it can direct itself to the nearest token and improve its execution time
