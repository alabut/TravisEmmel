---
layout: post

title: Weight Sensor Integration with Home Systems
subtitle: "Birth of a fancy blog"
cover_image: blog-cover.jpg

excerpt: "This is a project to integrate several different sensors to enhance the movie-watching experience."

author:
  name: Karri Saarinen
  twitter: karrisaarinen
  gplus: 100687498195339762535 
  bio: Co-founder, Design
  image: ks.png
---

The inspiration for this project came from wanting to accomplish something in-line with the following scenarios:

Bedroom Scenario #1:
When getting up in the middle of the night, a scene is triggered that brings the lights leading to the bathroom up to 20% brightness and when returning to bed, turns them off.  

Bedroom Scenario #2:
It’s morning and I was supposed to be out of bed at 6:00AM.  At 6:01AM, the system realizes I’m still in bed and starts to bring the lights up and/or open the blinds to further encourage my egress from the warm confines of my bedding.

Living Room Scenario #1:
Watching a movie and my beverage requires an untimely refill.  As I get up, the system realizes I’ve left the couch and, in response, pauses the movie I’m watching and turns the lights up to 40%.  With my return to the couch, the lights drop and the movie resumes.

Living Room Scenario #2:
As I settle into my favorite spot on the sofa to do a little after dinner reading, a small booklight over my right shoulder comes on, the stereo comes on to play some soothing music and the rest of the lights in the house dim down.

In order to make the above scenarios a reality, the only component I was missing was a weight sensor that would interface with my Z-wave network.  Unable to find a prepackaged setup in the weight range I required or any range, for that matter, I opted to make my own.  Not wanting to reinvent the wheel in terms of connectivity and Z-wave integration, I once again decided to utilize the Remotec ZFM-80 dry contact relay as the bridge between the network and my devices.  I installed the relay in a premade project box and added a power receptacle into the mix.  This way, the weight sensor could also turn a dedicated device on in addition to triggering a more involved scene.

Test fitting the ZFM-80 relay inside the project box.  Also shown are the two machined cut-outs for a power input and receptacle.

My vision for the project was to create a low profile puck with an integrated switch that would sit under one leg of the couch or bed and dummy pucks for the remaining legs.  When someone sat down or got into bed, the added weight would trip the switch within the puck and set off a scene or turn on/off whatever device was plugged into the attached receptacle.  I designed the puck as a two-piece assembly encompassing a roller ball switch and a heavy duty spring.  The goal was to make the complete assembly as low profile as possible and keep the overall travel to a minimum.


Machined dummy puck.


Two-piece puck that houses the spring and switch.  The donut shaped relief in the center provides a mounting feature for the spring and the switch mounts to the three vertical tabs which also allows for a bit of adjustment to tune the sensitivity of the switch.

I began sourcing components with the above requirements in mind.  The overall height of the device would be determined by the switch height, so I tried to obtain a switch with as small a body as I could find.  Once the switch dimensions were dictated, the next step was to find a spring that had an appropriate spring rate and travel.  Given that the static weight of the couch and bed were significantly different, I had to source a couple different options to meet the requirements of both setups.  I also tried a couple of different materials, namely extremely stiff elastomers and traditional, wound springs.  In the end, the traditional springs won out.


Four possible candidates for the spring component.  The two units on the left are high-density elastomers and the two on the right are more traditional coil springs.  The coil springs were found to be the best option.

With all of the components sourced, I began modeling the entire assembly in CAD, trying to make it fairly simple to manufacture.  Internally, I created a mounting point for the switch that would allow some adjustability should the switch sensitivity need to be tweaked via engagement point.  I also made a relief for the spring to allow for easier alignment and assembly.  Externally, I made the overall diameter large enough that it would work for the legs of most beds/couches and gave the top a cup-shape so that said legs would not be subject to slipping off.  The dummy pucks were designed to match the same profile.  

Spring and roller switch being test fit in the sensor puck.

With the CAD models finalized, it was on to machining.  While the CNC cut out the blanks for the switch and dummy pucks, I worked on the project box.  I milled out cutouts for the power input and 110V receptacle as well as cutouts for the LED indicator and pairing switch on the ZFM-80.  It was a tight fit, but mercifully it all went together without too much swearing.

Pic of the milled out project box.  The square mounting holes are for the power input/receptacle and the round hole on the floor allows access to the momentary button on the relay.


Power receptacle and power cable connection.

Once the machining had completed, I began to assemble the individual components, connect the appropriate wires and button everything up.  With everything in place, it was time to pair device to the network and test its operation.  The switch assembly paired without issue and showed up immediately in my Z-wave devices.


Fully assembled unit.

During initial testing, I found that the coil springs worked best and most consistently for activating the relay.  The lighter weight spring worked perfectly when used in conjunction with the couch and the heavier spring worked out well for the bed (the static weight of the bed would tend to activate the switch when the lighter spring was installed).


Additional Pics:

Underside of the switch puck base, showing the relief for the wire that runs to the ZFM-80 module in the project box.


Close-up of the assembled project box showing the installed power receptacle.

**Zoomable images**
<div class="full zoomable"><img src="{{ site.baseurl}}/images/incorporated.jpg"></div>
