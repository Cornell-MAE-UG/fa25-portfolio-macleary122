---
layout: project
title: Wind Turbine Blade Design 
description: Design and Validation Group Project
technologies: [Fusion 360, Matlab]
image: /assets/images/radio-machine-cad.jpg
---

Project Overview: 
In this project we were asked to design the blades for a wind turbine in a given wind velocity probability distribution operating at a constant rotation rate in a wind tunnel. The goal was to use skills we had practiced in the previous labs to decide on the optimal design to maximize power extracted from the wind flow.    


Design Process: 
Our group first decided to optimize the design for a wind velocity of 4.8 m/s, which was the most probable wind speed based on the Weibull probability distribution. Then, we decided to consider which airfoil cross section to use to optimize the lift to drag ratio to maximize power extracted for low Reynolds number flow. Our criteria was to find an airfoil cross section commonly used in small scale wind turbines that was 3D printable with a high lift to drag coefficient, mantained for a wide range of angle of attacks. The S1223 airfoil met this criteria the best. We decided on a design rotation rate of 1500 RPM based on power curves from previous labs. We maximized length and chord based on provided constraints to maximize blade surface area. Using the design rotation rate and design wind speed, we varied pitch with radius to mantain an optimal angle of attack along the blade length. We developed Matlab code to model that our blade was safe from structural failure and to determine which taper to use. 
After deciding on our design, we made the CAD using Fusion 360:

![Photo of old radio]({{ "/assets/images/old-radio.jpg" | relative_url }}){: .inline-image-l}

Testing Summary: 
We validated our design by collecting power curves of rotation rate versus power at four different wind speeds, making sure to stay within safety limits. Pictured below are the power curves:

![Power Curves]({{ "/assets/images/powercurve.jpg" | relative_url }}){: .inline-image-l}

We found that maximum power extracted out of the speeds measured was 0.9 W at 5 m/s, close to the design wind speed of 4.8 m/s, which supports that the design performed best at the wind speed it was expected to. However, the power was maximized at 1153 RPM, a different rotation rate than the design rotation rate of 1500 RPM, and the modeled peak power was 1.6 W. Also, due to time constraints we are unable to test wind velocities higher than 5 m/s, so it's possible that the peak power for our blade design peaked at a higher wind velocity. Therefore, further testing is needed to verify power extracted at higher wind speeds. Here is the exponential fit we used looking at wind speed versus power, which predicts that power would further increase at higher wind speeds: 

![Wind Speed versus Power]({{ "/assets/images/windspeedpower.jpg" | relative_url }}){: .inline-image-l}



My Contribution: 
I contributed to finding and assesing possible airfoil cross sections. I also feasibility tested the S1223 airfoil by 3D printing a sample tip cross section to assess manufacturability since there were concerns about the thin trailing edge being difficult to manufacture. I also helped with modeling possible structural failure of the wind turbine blade and ensuring that parameters had a sufficient factor of safety against failure. I also helped in documenting each stage of the process to synthesize information for validation testing and the final report.  


