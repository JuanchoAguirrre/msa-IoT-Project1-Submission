# msa-IoT-Project1-Submission
My repository containing my submission for the MSA IoT workshop.


i. My submission's architecture has retained the majority of the initial project, with my additions extending it. In short, it follows the general structure of all the relevant functions being called from the project's "sendTruckTelemetry()" to maintain consistency when updating the truck's state. 

	My main addition to the project would be the ability to monitor and manipulate the 'driver's' state while in the process of delivering to a customer, ranging from "energized" at the beginning of being enroute to "fatigued", where they will no longer be able to continue driving. Here, another addition would be the command from the IoT device central view to order the driver to take a "rest". The status of the driver then changes to "rest" as the truck's state shifts to "parked". It then acts as a cooldown until it counts back down till the driver is ready and "energized".


ii. new telemetry data being generated and displayed in PowerBI would be the the driver's state/wellbeing, the total duration that they have been 'enroute' for a delivery, and the total amount of time they have 'rested' while doing so. This ultimately allows users to track their driver's wellbeing and 'simulates' caring for them while on the job.

iii.
	1. To connect my app.js file to my Azure IoT Central device, I used their provided connection string, primary key, and scope Id. Similarly, I used the Azure maps key to connect the file to that service.
	2. To connect my IoT Central device to the Azure Events hub, I had the data automatically exported through the former's 'Data Export' module with its provided connection string.
	3. To connect my IoT Central device to the Azure Blob storage, I had the data automatically exported through the former's 'Data Export' module with its provided connection string.
