Recruitement project
================

Minature Pricing Server(MPS)

Introduction
------------

This is a sample project for Regentmarket Markets Group company recruitement process.

This application calculates a price based on the formula below:
	F = S * e ^ (r*t)

where,
F : Future Contract price
S : Current spot price, which will be received from a third party provider.
t : The time in year to which the future price is to be calculated.
r : Annualized Interest rate.

Requirements
------------
	* PHP v5 or newer.
	* working lampp or Xampp or Mammp
	

Description
-----------
This application is created to calculated the future contract using the provided data in the data.xml file

in case if the above given data is not in XML it uses the below formula to calculate the rate of interest.

Intrapolation formula:
					  (y3 - y1)
	y2 = y1+ (x2 - x1)*--------- 
					  (x3 - x1)
where x1 < x2 < x3 and y1 < y2 < y3



UI
---------

The startup page contains three input fields:
	- Amount
	- Time(in days)
	- Rate of interested (autopopulated)
	
Entering the Time and moving to other field will trigger the data into Rate of interest field	
Clicking on the "Calculate" button would display the "Future Contract price".
