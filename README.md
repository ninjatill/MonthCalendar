# MonthCalendar
A daily gold star system, one month at a time. Inspired by the [Every Day Calendar](https://www.kickstarter.com/projects/simonegiertz/the-every-day-calendar), this is a compact version that has 48 total touch pads.

I saw the Every Day Calendar (EDC) referenced on the Particle forums. It sounded like a great idea and I needed way to track if I took my daily allergy pill. However, the EDC is very large and therefore expensive to manufacture. I also thought the functionality could be expanded beyond just turning an LED on to indicate completion. By the time I got around to designing my own version, the Kickstarter campain had closed and there were no resouces made available via open source yet. So I designed it all from scratch.

My Design Criteria:
- Should be small enough to fit inside a medicine cabinet or mounted on limited wall space in a bathroom.
- Should still be able to track every day of the year.
- Should record and track progress and report it to the cloud for review.
- Should be able to track multiple users (like a husband and wife pair).
- Should use capacitive touch (seems more robust and it's something new to learn).
- Should have colored LEDs that shine up through the PCB (similar to the static LED color on the EDC). Color can be used for:
-- Indicating missed days with red (or some alternative) color.
-- Showing fancy animations to entice interaction/completion.
-- Indicating separate users and tasks via differing color schemes.

Additional considerations (some after starting the design):
- There's no need to have the LEDs on all the time. Perhaps some sort of human presense detector can be incorporated to only turn on the LEDs when someone is near the system.
- If this is in a bathroom, where most people start their day, it would be benificial to act as a calendar to indicate what is the current day.
- Because of the modularity, the top touch plate (described below) could be swapped out for different configurations or locales. It might be a benifit (or neccessary) to add non-volitile storage to the touch plate to identify hardware revisions, serial numbers, locales, layout changes, etc.
- To minimize light bleed between indicators I will fabricate a 3D-printed light collimator.

The initial design uses 2 PCBs connected via pin headers. The bottom PCB contains all the controller hardware and LEDs. The Top PCB is merely a touch plate containing all the capacitive touch pads. The microcontroller is inserted on the back-side of the controller PCB as well as the power entry ports. The PCBs will be mounted in a 3D printed case. 
