Project: Event driven simulation of Garden Sprinkler System

--------------------------------------------------------------
Copyright (C) 2013 by Ruchira De and Debasish Das

PLEASE SEE LICENSE FILE FOR LICENSE RESTRICTIONS

Description:

Garden Sprinkler System is a software controller to control the
sprinklers which are installed in a user's garden.

User provides a list of weekly schedules where the sprinklers needs to
be turned ON/OFF with varying duration of time and rate of flow of
water.

Users can add/remove schedules and the schedules are serialized for
futures uses.

User can also force the sprinklers to turn ON/OFF.

A event driven simulator which extends SwingWorker is run as a background
process which generates data to analyze the water consumption by the
sprinklers.

Garden Sprinkler System shows the location of the sprinklers on a panel
and help the users to visualize the status of sprinklers during the simulation.

Screenshots of the application are provided in the folder screenshot. Right now
it shows two different analytics. It presents the weekly water consumption per
sprinkler and per day water consumption by all sprinklers.

The simulation log is provided in the folder log. It shows the status of all
sprinklers at each simulation time tick.

Code limitations:
Chart axis : We get a quantitative idea about water consumed per day but
does not show exact amount. We could not find a light weight java chart
utility for this. Next step would be use javascript plotting utilities.

To build:

A ant buildfile build.xml is provided in the repo. ant will build the
project in bin/

To run:

cd bin/
java gui.SprinklerSystemGUI

Questions/Comments:

For any question/comment related to the project send an email to the authors:

Ruchira De ruchira.de@gmail.com
Debasish Das debasish.das83@gmail.com
