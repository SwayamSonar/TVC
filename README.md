# TVC
Thrust Vector Control Model Rocket.slx is a simulink simulation of the rocket attempting to maintain an upright position during flight and can track horizontal velocity due to the TVC

Tune.slx is for tuning PID values as simulink fails some of the time when using Thrust Vector Control Model Rocket.slx

Main.cpp is an implementation in arduino for the bluepill (stm32f103c8t6).It should work with arduinos, just copy paste the contents into the arduino ide or whichever you prefer

# Recommended Watching

[BPS.space](https://www.youtube.com/channel/UCILl8ozWuxnFYXIe2svjHhg)

[Brian Douglas](https://www.youtube.com/user/ControlLectures/videos)

[Understanding PID Control, Part 1: What is PID Control?](https://youtu.be/wkfEZmsQqiA)

[How to read values from mpu6050](https://www.youtube.com/watch?v=ImctYI8hgq4)

# Recommended Reading
[The Fundamentals of Control Theory](https://www.patreon.com/posts/book-is-now-free-28313078)

[Books Joe Barnard (BPS.space) recommends](https://www.youtube.com/watch?v=BcKL4M5Xod)

https://folk.ntnu.no/skoge/prost/proceedings/ecc-2013/data/papers/0927.pdf

https://ntrs.nasa.gov/archive/nasa/casi.ntrs.nasa.gov/20120014565.pdf

http://ardupilot.org/dev/docs/apmcopter-programming-attitude-control-2.html


http://ardupilot.org/dev/docs/ekf2-estimation-system.html?highlight=quaternion

Instead of trying to estimate the quaternion orientation directly, it estimates an error rotation vector and applies the correction to the quaternion from the inertial navigation equations. This is better when there are large angle errors as it avoids errors associated with linearising quaternions across large angle changes.

    See “Rotation Vector in Attitude Estimation”, Mark E. Pittelkau, Journal of Guidance, Control, and Dynamics, 2003” for details on this approach.

