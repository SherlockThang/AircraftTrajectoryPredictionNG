# Fleet (aircraft type)

Airline fleet is defined by aircraft ICAO codes. With these codes, it is possible to access the corresponding BADA configuration / performance data.

For each aircraft type, the BADA parameters define:   
●	A maximum take-off length expressed in meters   
●	A maximum landing length expressed in meters   
These lengths must be compared to the airport configuration in order to ensure that the aircraft is able to select an adequate run-way to take-off or land.

# Fleet Definition   
These input parameters are defined in an EXCEL file with name "AirlineFleet.xls"

#  Field   Field Type  Comment    
●   Aircraft full name	| String	| Defines uniquely an aircraft type and allows to link it to BADA ICAO code   
●	Number of in service aircraft instances | Integer | Number of available aircrafts of the same type (same seat configuration?)   
●	Number of available seats | integer	| No seat configuration yet defined   
●	US Dollars flying costs per flight hour	| float	| Factor to be multiple by a flight leg duration (expressed in decimal hours)   


# Extended Fleet Definition
These outputs are created in an EXCEL file with name "AirlineFleetExtendedData.xls"   

#	Field		Field Type	Comment
●	Aircraft ICAO Code (BADA identifier)	String	Defines uniquely an aircraft in the BADA database   
●	Landing length in meters	Integer (meters)	Used to ensure that the aircraft is able to find an adequate runway in the departure or in the arrival airport   
●	Maximum Take Off length in meter for Maximum Take Off Weight 	Integer (meters)	Used to ensure that the aircraft is able to find an adequate runway in the departure or in the arrival airport   


# Example of an AirlineFleet.xls input file

Aircraft	In service	Orders	Passengers Delta One	Passengers First Class	Passengers Premium Select	Passengers Delta Confort Plus	Passengers Main Cabin	Passengers Total	Costs per flying hours dollars	Refs	Notes
Airbus A220-100	3	4		12		15	82	109	2540	[32]	
Airbus A220-300	4	41		12		30	88	130	2580	[33]	
Airbus A319-100	5			12		18	102	132	2780	[34]	
