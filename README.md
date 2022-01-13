# MIT-things
Are you from MIT admissions and got directed to here? Great! If not, that's still cool, this is just a list of things that I've done, with some context.
<br>
<ul>
  <li><a href=https://github.com/GunnAeronautics/mower4.2.0>Rocket control code</a><br>This is the current version of the rocket control code. Mainly created at the end of my sophomore year of high school and further improved on throughout my junior year, the main advancements in this version were adding Inertial Measurement Unit (IMU) support (so we know what the rocket is doing past just altitude) and making the code much more generalized, so more of it could be reused from year to year. The current plan is to turn most of this into a standalone library, which would allow anyone to run any rocket project they want off of this code and not just our TARC mechanisms. The next itaration of the actual controls behind this is still somewhat under developement, but will be a lot fancier and be able to focus on the actual control theory aspect of flight rather than just piping data from sensors directly to actuators. This was still a necessary step along the way, though. (version number is entirely accidental)</li>
  <li><a href=https://github.com/GunnAeronautics/glider_control_demo>Glider control demo</a><br>Quick demo I threw together to see if I could actually process the data from the gyroscope into actuator outputs. TODO: I had a video of this working somewhere...</li>
  <li><a href=https://github.com/GunnAeronautics/GAA-quaternion>Quaternions</a>, <a href=https://github.com/GunnAeronautics/GAA_Quat_master>more quaternions</a>, and <a href=https://github.com/nmiliv/QuaternionsDemo>even more quaternions</a><br>Quaternions are still my one weird math flex. I originally learned how to use them to help to process gyroscope data for the rocket (first two libraries are for that, first version had bad syntax so I made a different one that is less bad, but the old version is still needed for the old code). Third library was my first try at using quaternions.</li>
	<li><a href=https://github.com/GunnAeronautics/GAA-Buzzer>Buzzer library</a><br>Personally, I think this is my biggest contribution to rocketry avionics. Although this library provides basic support for generating tones, beeping at intervals, and so on, the main addition is the support for morse code. Most off-the-shelf flight computers available these days use their own systems of beeps to report data and errors, which causes issues when you realize (a) every brand is going to have different, essentially meaningless error codes, and (b) nine beeps (signifying the digit nine) and ten beeps (signyfying the digit zero) are hard to tell apart but have very different meanings (800 feet is different from 899 feet). Morse code solves both of these problems beacause (a) errors can now have actual letters/words and (b) numbers in morse code were already designed to be easily differentiable. I didn't know morse code going into this project, and I still don't know most of it, but just learning the numbers and a couple letters has been so much easier than trying to decipher what other systems do.</li>
</ul>
