# Test Plan


## Obstacle Detection:
### How: Our implementation for this step requires multiple steps :
#### Step 1: Find a distance value between each pair of sensors. To test the distance
value, we may use the numbers we see for the height and length, as well as the
Pythagorean Theorem.
####Step 2: Check the angle found between each pair of sensors using the distance value
initially found.
####Step 3: Using these values, determine what each angle should approximately be to
detect different types of obstacles.
####Step 4: Detect the obstacles.


## Output: As we had steps for each test, we will again make steps for the expected outputs:
#### Step 1: Compare the outputted (through serial) value for the hypotenuse to the
Pythagorean calculated value. We expect them to be the same.
####  Step 2: Using the same technique as step 1 except calculating the angle, we should
see the same value for this calculation as well.
#### Step 3 : The values and outputs for the “obstacle detected” will be constantly
checked and rechecked to make sure the angles determine the correct obstacle.
#### Step4 : Adding Audio to the Ultrasonic Sensors.

## High level test plan
| Test ID |           Description       |      Exp I/P    |    Exp O/P   |   Actual Out  |   Type Of Test |
| --------| --------------------------- | --------------- | ------------ | ------------- | -------------- |
|  H_01   |      High accuracy     |  Choice  |    Display   |   As Expected | Scenario based |
|  H_02   | Capable of measuring a distance of up to 400 cm | Choice  |  Display    |   As Expected | Requirement Based |
|  H_03   | Measuring time lapses between the sending and receiving of the ultrasonic pulse | Choice | Display   |   As Expected | Requirement Based |

## Low level test plan
| Test ID |           Description       |      Exp I/P    |    Exp O/P   |   Actual Out  |   Type Of Test |
| --------| --------------------------- | --------------- | ------------ | ------------- | -------------- |
|  L_01   | Detection of clear objects | Choice | Display  | As Expected   | Scenario based |
|  L_02   | Provide multiple range measurements per second | Choice | Display   | As Expected  | Requirement Based |
