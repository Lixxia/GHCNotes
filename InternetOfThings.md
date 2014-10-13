# Novel and Innovative Applications for Internet of Things

### A software architecture for the management of Smart Buildings
### *Larissa Suzuki*
- managing a physical infrastructure in real time > smart buildings
- multiple proprietary building systems (access control, hvac control, fire alarm)
- smart building converged systems, integrated and real time collection of data
	Optimally, everything is interconnected to facilitate toe collection of real time data and the monitoring of the building health
- want an architecture that allows us to gather data, and share that data between different state holders 
- by 2020 everybody would have about 7 smart appliances. Take out the middle man, manufacturor would automatically know if something is not functioning properly
- intelligently adapt the environment based on the conditions outside
- automate all the things
- gather data from different systems, connect that data, intelligently understand what's happening inside the physical infrastrcture
- fragmented metric might lead to poor decisions
- want cohesive data sent to a system to make sure correct decisions are being made
- a platform in which we can integrate data and send it to emerging technologies
- use middleware which uses MQIT
- visualize then publish so different applications can consume data in an integrated manner
- smart buildings, proof of concept
	- goal: better equipped and more efficient maintenance repairs
	scenario: allow engineers to find and update assets using augmented reality applications - both point assets and linear assets
	actors: building eingneers 

	- data collection system
	- event and enrichment system
	- assets and work orders management system
	- data middleware
	- emerging technologies


**What would be the next step with software development process?**
> this is already implemented, we want to put in actual meters. We are moving to more advanced technologies. We can send machines instead of people to complete tasks. 

**How do you deal with false-positives?**
> We have to callibrate that specific piece of software to ensure it is a robust system. This serves as a framework to develop further applications. 

<hr>

### An Insider's Look at the IoT in a Railroad
### *Yujie Ying*
**Overview of railrodad sensor technology**
- thousands of sensors have been installed on and inside the tracks to detect derailment or failure
- infrared sensors are on the track to detect overheated bearings
- microphones to recognize audible defects
- ultrasonic sensors
- wheel profile lasers to take a crosssectional snapshot of the wheel to find defects
- strain gauges to identify lax spots in the wheels
- low air hose detector to prevent accidents

**Smart train inspection site**
- most inspections are performed manually
- smart train inspection: want to capture the full view of the train without having the train stop
	- inspection performed by automated or semi-autimated system
	- wheel detectors
	- use line scan cameras to provide a complete scan of the train
	- LIDAR scanners to create a 3d model of the train
	- the 2d and 3d sensors create a lot of data per minute, developing systems to focus on parts that require inspection
	- GUI application to be used by inspectors
	- all components are connected to the internal IP network
	- 3 full functional sites, want to have at least a dozen fully function sites
**Other R&D**
- researching on-train sensor networks 
- mote: an intelligent tag on the car with a number of sensors attached to it
- track evaluation vehicles: a car with several sensors used to measure the rails and forecast failures before they occur
- challenges
	- network coverage
	- sensor cost
	- batter life for motes
	- industry standardization
	- big data integration
	- security

**We live near a railroad switching yard, is ther instrumentation to detect extra riders?**
>This is one of the applications of the imaging site. next step: use an algorithm to identify humans on trains and devise an alert. 

**People crossing railroad tracks, there are several accidents so is there a way to detect this?**
>Safety is a priority, we have an alerting system. We are currently working on a project: Positive train control system: technology for anti-collision of trains and detecting any obsticals in front of trains. We're getting there.

<hr>

### PiDoorbell: Home Automation with RaspberryPi
### *Rupa Dachere*

- **problem:**
	1. wanted to know who was at my front door
	2. what day and time they came
	3. wanted to be notified when they arrived
	
	>ex. contractors, package delivery, neighbor, etc.
- **piDoorbell Flow**
	1. caller comes
	2. proximity sensor outputs changed signal to RaspberryPi
	3. RapsberryPi instructs webcam to take photo
	4. webcam sends photo to RaspberryPi
	5. RaspberryPi uploades photo and sends sms
- **steps**
	- walk in front of proximity sensor
	- see detection of foreign object
	- trigger camera to take a photo or start capturing video
	- save in file with timestamp
	- send sms
	
[code is open sourced: software, handout and tutorial](github.com/codechix-opensource)
