#Series 1
***
Project Robotnics, AS 2013, Alexander Rüedlinger

##Question
```
1. Explain how the robot behavior works by analyzing the code.
2. What do you think the line emit forward speed stands for?
3. What represents speed in this line of code and how can it be reused?
```

###Question 1
First off, each e-puck implements a so called robot controller. Such a controller implements different event handlers which handle a specific type of event. So if a e-puck receives an event it will execute the corresponding event handler.  
The selection of the appropriate event handler is called dispatching and is performed by the aseba framework.  
Besides receiving and responding to events, e-pucks can also send events.  
In this exercise the e-puck 1 acts as a control unit. It sends different events which are received by the other e-pucks. 

###Question 2
The emit statement specifies that a given robot should send an event of a certain type with zero or more arguments.
So the statement "emit forward speed" can be understood as follows:

- send a event of type forward
- with argument speed

If the event handler is defined then such an event will trigger the execution of the corresponding block of code.

###Question 3
The expression speed represents an argument in the "emit forward speed". It can be reused in the corresponding event handler using the variable args[0].
With the speed argument we can change the behaviour of the e-puck. In the exercises we've used the speed argument to change the speed and direction of the e-pucks.

