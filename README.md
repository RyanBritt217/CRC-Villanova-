<table>
<td><img src="https://raw.githubusercontent.com/RyanBritt217/CRC-Villanova-/main/CRC%20Image2.png?token=GHSAT0AAAAAACXEP6XRNFXAE3OSJ67HNCPWZXAEEMQ"  width=500 /></td>
<td><p><h1>CRC Wing Design & Manufacturing</h1></p>
<p> Design methods and process to construct a new wing for the CRC drone.</p>
</table>

## Motivation

The satellite industry is experiencing unprecedented growth, with new companies launching record numbers of satellites transforming global communication, providing near real-time images of our planet, and even enabling commercial space tourism.

As more and more satellites are added to low Earth orbit, the probability of collisions between satellites and orbital debris continues to rise.  This is compounded by the fact that any collisions that do occur (either between operational satellites and debris or two pieces of debris) create more space debris on impact.  Satellites and orbital debris travel at orbital speeds greater than 17,500 mph (7825 m/s) in low earth orbit.  At these speeds, even relatively small orbital debris can cause substantial to catastrophic damage to a satellite or a spacecraft if a collision occurs.

In [March 2021, a Chinese military satellite launched in September 2019 collided](https://www.space.com/space-junk-collision-chinese-satellite-yunhai-1-02) with a 10-50 cm piece of debris from the Russian Zenit-2 rocket that launched Russia’s Tselina-2 satellite in September 1996.  This collision resulted in 37 additional, trackable debris objects, and likely many more smaller pieces that remain untracked.

According to the [NASA Orbital Debris Program Office](https://www.orbitaldebris.jsc.nasa.gov/faq/#), there are approximately 23,000 pieces of debris larger than 10 cm orbiting the Earth. There are half a million pieces of debris between 1 and 10 cm, and approximately 100 million pieces of debris 1 mm or larger.  The United States Space Command (USSPACECOM) Space Surveillance Network (SSN) sensors catalog and track approximately 27,000 pieces of orbital debris in near-Earth orbit (larger than 10 cm).  This information can be obtained from [Space-track.org](https://www.space-track.org/).

Historically, satellite operators predict and manually maneuver spacecraft to avoid conjunctions with other spacecraft and cataloged space debris.  The SSN, for example, analyses known orbital debris trajectories over time to identify upcoming potential close encounters with the International Space Station.  If large debris is projected to pass within a few kilometers of the space station and probability of collision is greater than 1 in 10,000, a maneuver is scheduled to avoid conjunction.

The SpaceX Starlink constellation is the [first commercial application](https://spectrum.ieee.org/spacex-preps-selfdriving-satellites-for-launch) of an autonomous conjunction avoidance system.

## Project Description

Work with the [Aerospace Toolbox](https://www.mathworks.com/products/aerospace-toolbox.html) and [Aerospace Blockset™](https://www.mathworks.com/products/aerospace-blockset.html) products to identify potential satellite-debris conjunctions, and develop and analyze an automated algorithm for satellites to avoid space debris over time while maintaining orbital requirements.  Test and validate your algorithm.

Suggested steps:
1.	Review [Comparison of Orbit Propagators](https://www.mathworks.com/help/aerotbx/ug/comparison-of-orbit-propagators.html) and Constellation Modeling with the [Orbit Propagator Block](https://www.mathworks.com/help/aeroblks/constellation-modeling-with-the-orbit-propagator-block.html) examples to learn how to propagate orbital trajectories using Two-Body-Keplerian, SGP4 and SDP4 propagators in Aerospace Toolbox and Aerospace Blockset.  
2.	Run additional examples listed in the Background Material section below.
3.	Download space debris states from [Space-track.org](https://www.space-track.org/).
4.	Propagate the debris trajectories using SGP4 propagation algorithm.
5.	Define a satellite mission with specific orbit definition and requirements. e.g.: earth imaging or broadband communications.
6.	Propagate the satellite’s states over time, along with the space debris.
7.	Identify potential conjunctions during the analysis window [5,6].
	-	Determine close contacts by distance criteria.

Extended project work:
1.	Plan avoidance maneuver for upcoming conjunction with debris.
	-	Maintain orbit requirements when possible.
2.	Simulate avoidance maneuver.
3.	Design and execute a test and validation method for your algorithm.  Consider using [Verification and Validation products](https://www.mathworks.com/solutions/verification-validation.html).
