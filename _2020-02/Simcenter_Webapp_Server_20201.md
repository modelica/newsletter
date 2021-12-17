---
title: Simcenter Webapp Server 2020.1 released
author: "Anthony Domi ([Siemens Digital Industries Software](https://www.sw.siemens.com/ ))"
category: "vendor"
---


[Siemens Digital Industries Software](https://www.sw.siemens.com/ ) is proud to announce the 
recent release of Simcenter Webapp Server 2020.1. The key new feature being **the support of FMU 
as simulation models**.  
Additional new capabilities include:  
* New plot formats (XY plot, bar charts, spider charts, polar plots)
* [Interface with Excel](https://www.youtube.com/watch?v=h1U5ED5sdnA) to run models directly from the server
* A simplified Docker-based installer

#### Support of FMU as simulation models.
Since its [first release](https://www.youtube.com/watch?v=yx3W0SG1JfQ) in October 2018 this 
server-client, web-based solution provides access to system simulation models coming from 
Simcenter Amesim. Those models are prepared by the models 
authors (by selecting proper parameters and variables for the Webapp and defining results layouts) 
in order to be easily re-usable for model consumers logged-in to Simcenter Webapp Server.  

With the 2020.1 release Simcenter Webapp Server is becoming **tool-agnostic**.
It supports not only Simcenter Amesim models but also FMU 2.0 standalone simulation models.
So even if you use other system simulation software (for example Modelica-based), 
as long as this tool supports FMU 2.0 standalone co-simulation export, you can use your models 
within Simcenter Webapp Server.    
As an example here is a model coming from the Modelica ["Buildings"](https://simulationresearch.lbl.gov/modelica/releases/latest/help/Buildings_Electrical_Examples.html#Buildings.Electrical.Examples.RenewableSources) library.

![Example using Modelica-based "Buildings" library](Simcenter_Webapp_Server_20201_Modelica_example.png 'Example using the Modelica-based "Buildings" library')

In order to allow selecting the parameters and variables for a FMU a new "edit model" capability has 
been implemented allowing to filter out only relevant parameters and variables
as well as being able to change their titles.  

For more information on Simcenter Webapp Server, please visit our [website](https://www.plm.automation.siemens.com/global/en/products/simcenter/simcenter-webapp-server.html ).
