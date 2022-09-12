# Flexigy 

This is the dataset created for the evaluation of the Flexigy Porject

Contributors:
Tiago Fonseca, Luis Lino Ferreira, Paulo Baltarejo Sousa, Jorge Landeck, Lurian Klein

Description: 
This dataset contains appliance-level energy consumption, their flexibility and OMIE prices for a day.
User consumption flexibility is based on real-world data collected with the help of smart-energy meters for 50 different buildings. The testing data accounts for a total of 137 consumption FOs, in which 42 are fixed FOs corresponding to consumptions of computers and fridges, 71 are shiftable FOs characterizing the flexibility of appliances such as washing machines and dishwashers, and 24 are elastic FOs describing the flexibility of water heaters. 
Regarding energy self-production FOs, three different test scenarios were studied. 
3.	20% of the REC buildings have self-production; 
4.	40% of the REC buildings have self-production; 
5.	60% of the REC buildings have self-production.

# Dataset

The dataset files are organized as follows:

1. OMIE prices
	Files with the prices on a 15-minute basis of a day 

2. Test Case Scenario # //Folders have the corresponding test case scenario data

Each file (different formats) contains all the information during a day for the respective house and is structured:

Line 1 -> UserID, Buyer Profile, Supplier Profile 

Line 2 - X -> This section initiates in --Devices-- and specifies the devices characteristcs for that buiding. All lines are structured like: DeviceID, Name, Type. Lines with Thermal Elastic Devices (HVAC and Thermalacuumulators) must specify more characteristics

Line X - Y -> The rest of the file contains the energy values for each device as well as the information related to the FO that it relates to. The format is: DeviceID, FOID, ES, LS, FOType, FOName, Time,Unix, Energy

Line Y - End -> The usual consumption of elastic devices can appear just for comparison and results purposes


