Egen Coding Challenge – Level 2

Name: Sri Harsha Vardhan Reddi
Email: sreddi1@binghamton.edu

Description:
This project is used to consume data from the emulator and persist the metrics data in MongDB. Total six micro-services are provided in the following controllers.

MetricsController:
- create() : Used to insert the metrics data into DB.
- readAllMetrics() : Used to read all the metrics from DB.
- readMetricsByRange() : Used to read the metrics by the given range of timestamps.

AlertsController: 
- readAllAlerts() : Used to read all the alerts from DB.
- readAlertsByRange() : Used to read the alerts by the given range of timestamps. 


This project also has the following two Rules.
OverWeightRule: It is executed when the weight of the person shoots 10% over his base weight.
UnderWeightRule: It is executed when the weight of the person drops below 10% of his base weight.

Mongo DB details:
Installed MongoDB in your system.
Create a Database "sensordb".
Create collections "metrics" and "alerts".
Scripts:
> use sensordb
> db.createCollection("metrics");
> db.createCollection("alerts");

Steps to run:
1) Download the Zip and extract it.
2) Open Spring Tool Suite and import this extracted project as existing maven project.
3) Please change the base_weight value to your convinience in OverWeightRule and UnderWeightRule classes.
4) Then do Maven clean, Maven install.
5) Now Right click on egenSolution and follow Run As -> Spring Boot App.
6) The project will be ready to be used by Emulator.  