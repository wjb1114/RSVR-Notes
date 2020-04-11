# RSVR-Notes

## SpatialOS / Photon - Networking options
### Photon is more p2p, matchmaking esque - think Halo or Call Of Duty matches
### SpatialOS - Full cloud hosting solution with dedicated server, network, and client layers - More closely matches existing OSRS architecture, but may be more expensive in production
	
## Tick System
### Server ticks act as clock for mechanics - ex. entity spawns, farming growth status
### Most interaction is done real time and client side - Movement, combat, skilling interactions
#### Use server ticks to dictate packet send rates - get player status and send to server every tick
		
## Engine
### Most seem more comfortable with Unity
#### Unity can use both Photon and SpatialOS
### Many others prefer Unreal
#### SpatialOS or own netcode
		
## Interactions
### Combat
#### Start with melee only, basic collision detection for detecting hits
### Movement
#### Basic point and click navigation and thumbstick movement for headsets that are compatible
#### Object interactions using combat mechanics - ex. slashing webs, hitting levers
### Physics
#### Object throwing
##### Basic physics should be enough, we shouldn't need realistic trajectoriess, bounciness, etc. - at least not yet
			
## Skills
### Basic skill interaction - ex. fishing, woodcutting, mining, based on a recognizable location and its skill spots
#### Ex. Lumbridge Courtyard, includes base combat, woodcutting, smithing
		
## VR Specifics
### None of the programming leads currently has a headset :(
### Should be able to start as a standard first person game with mappable inputs
### I plan on getting a headset in the next few months
#### Which one will be based on availability and what other members of teh team may already own
		
## Todo
### Base network application
#### Simple scene with movement, each player has a single model to control
#### Text and/or voice chat? - Unity has some APIs for this
### Environment setup
#### Code repository
##### Public or private will depend on team size and project requirements - talk to Soup about this
### Task List
#### Create Trello board
##### Base tasks include repo setup, work on base networking application
##### Once we decide on starting location, will add tasks for mechanics specific to that location
