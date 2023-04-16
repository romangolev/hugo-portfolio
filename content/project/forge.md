---
title: "Making Autodesk web services more powerful"
description: "Model Analysys and Data Validation using Autodesk platform services - APS (formerly Forge)"
tags: ["web", "node-js", "javascript", "heroku", "autodesk"]
weight: 3
draft: false
#date: 2017-02-20T15:26:23-06:00
---

### Building web applications
Within the new era of cloud computing, many there now exist services for managing construction projects in the cloud. It is very important to store data in Autodesk Platform Services (APS). As an extend to Atodesk ACC(BIM360) it is possible to create different kind of web application that will be using ACC as a main frame or even possible to create a separate service that will work without it. It has a very detailed documentation [here](https://aps.autodesk.com/developer/documentation). Since in my work I mostly used BIM360 as a CDE there were no doubts that integrating Forge into a day-to-day pipeline may be very handy.

The application itself is very basic and mostly relies on ACC(BIM360) service in terms of user management and also uses it as a database. Here is a schematic representation of how does it work on a back-end:
![Diagram](../images/diagram_data.png)

The interface is simple but allows to select and open converted cloud models in browser. The purpose of right pane is to visualise element's values and output donut chart using [chart.js](https://www.chartjs.org/) You can select a property for the visualisation, it uses [jQuery](https://jquery.com/) to get near-instant responsiveness.
![Web application view 1](../images/data1.png)

It does show the chart of the element's values from the model. Here is an example of application I created for as an extend to ACC to get the information about models maturity.
![Web application view 2](../images/data2.png)
On top of that, APS API gives an ability to extend functions of the embedded model viewer and develop custom tools. Three buttons of the viewer on the image above has custom functions for model validation and data extraction.