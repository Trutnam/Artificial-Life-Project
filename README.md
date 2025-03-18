# Artificial-Life-Project

This file, entitled final.py, contains the python script for my final submission for this class. I have greatly enjoyed expirimenting with difftaichi in this course, and each lab has brought unique and fun challenges to be solved. My favorite lab to work on was lab 4, which involved implementing an open-loop system in difftaichi. For this project, I have continued along those lines, and worked with different parameters and robot shapes from the previous labs to increase the amount of interesting behavior exhibited.

My project was built off of the mpm implementatation example from difftaichi. I have built off of this, creating an open-loop control implementation with adjustable time dependent acutation patterns driving the motion of the soft-body. This approach has yielded interesting results, allowing me to see how different actuation patterns influence the movement of various shapes over time. 

The core of the open-loop control mechanism is  the compute_actuation() function, which defines actuation forces for each actuator as a sine wave. The function assigns a unique phase shift for each actuator, creating coordinated but independent oscillatory movement. 

The actuation force applied at each time step is given by:

a(t) = A * sin(2πft + φ)

Where A is the amplitude, f is the frequency, t is the time step, and φ is the phase shift specfic to each actuator. The actuation values are stored in a global actuation field, which is accessed by the individual particles during the particles-to-grid step.

This form of movement is easily applicable to robots of all different shapes, which allowed me to incorporate robots from past labs into this project, tying the course together elequently. I spent a few hours trying to implement a closed-loop system, but ultimately ran into issues that would require assistence from somebody with more knowledge in difftaichi. After looking at the available resources online I found that I was not able to solve the error I was getting in the timeframe I had left to complete the project.

I am sad to see this class end. I really had a blast playing around with the difftaichi language, and coming to class was always a fun and non-stressful opportunity to learn from Sam. I made sure to come to class every session, and I was grateful for the opportunity to learn from my peers. I hope to see everyone again, and I can't wait to see what everyone worked on!
