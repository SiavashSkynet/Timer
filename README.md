# TimerEvent
TimerEvent provides an easy way to trigger functions every set time and is a non-blocking alternative to delay() function. TimerEvent is based on TimedAction 1.6 by Alexander Brevig (alexanderbrevig@gmail.com). It is updated to work with Arduino IDE 1.8.5. in this fork I did add a start function to help developers to use timer more easier .
for any commit and sugestion please send me an Email : (shojaee.skynet@gmail.com)


# Public functions

## set(unsigned long myPeriod,void (*myFunction)())
Used to setup the timer. Use this within setup(). myPeriod is the interval in milliseconds that the function myFunction will repeat.
For example: myTimer.set(1000, myFunction);

## set(unsigned long myTimer,unsigned long myPeriod,void (*myFunction)())
Similar to the one above, myTimer is the starting time in unsigned long, which will otherwise be 0 if not declared.

## reset()
Resets the timer.

## disable()
Disables the timer.

## enable()
Enable the timer.

## update()
update() goes inside loop(), which does the checks every clock cycle.

## start()
start timer

## setInterval( unsigned long myPeriod )
Used to change the interval after you had set it.
