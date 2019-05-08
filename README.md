# Activity-with-Factory-pattern-Student-Orientation

Run following command when inside Gautam_Beri_Pragya_Vishalakshi folder:

ant -buildfile campusTour/src/build.xml clean
ant -buildfile campusTour/src/build.xml all
ant -buildfile campusTour/src/build.xml run

command to generate javadoc:
ant -buildfile campusTour/src/build.xml javadoc

The javadoc generated is stored in "doc" folder at src level. The "index.html" is the file which takes from first page of Javadoc.

-----------------------------------------------------------------------

Enums Used:
1. Activity of visiting buildings:
	- ByFoot: visit buildings by foot.
	- BusRide: visit buildings by bus.
	
2. Activity of Picking Gift:
	- UniversityUnion: Pick gift from University Union
	- EventCenter: Pick gift from Event center
	
3. Activity of Having Lunch:
	- MountainViewOnline: Order lunch online
	- AtCIW: Get lunch at queue at CIW
	
4. Activity of attending lecture:
	- CS240: Attend in-class lecture
	- CS350: Attend online streaming of lecture


Example orientation pattern provided:

PickGiftPlaces.UniversityUnion: 80.00 kg of CO2, $0.00, 10min, 200cal
LunchPlaces.AtCIW: 180 kg of CO2, $50.00, 35min, 250cal
LecturePreference.CS350: 60 kg of CO2, $20.00, 30min, 120cal
CollegeBuilding.BusRide: 50 kg of CO2, $1.00, 5min, 80cal

Total:
CarbonFootprint : 370.0kg of CO2
Duration : 80.0min
Cost : $71.0
Calories : 650.0cal


Algorithm:
The enum of each activity is provided to student while creating the constructor of Student.java. The ActivityBuilder.java is used to build the orientation activity provided.

Result.java is used to display the total efforts for the activities provided for the orientation.
