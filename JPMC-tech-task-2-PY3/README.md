

Task Overview | Installation Instructions | Link to Module 2

Introduction
Experience Technology at JP Morgan Chase
Try out what real work is like in the technology team JP Morgan Chase. Fast track to the tech team with your work.

Module 2 Task Overview
Use JP Morgan Chase's frameworks and tools Implement JP Morgan Chase’s Perspective open source code in preparation for data visualization

Aim:Take an incomplete setup of Perspective, i.e. a graph that updates manually, and make it work with the code from Task 1 such that it now updates automatically by continuously requesting from the server application

Please clone this repository to start the task
[goal-a] In the client application, observe that when new data feed is retrieved whenever you click the 'Start Streaming Data' button, the previous entry is re-entered into the table. Update the application so that the table does not have duplicated entries
[goal-b] We also want the react app to keep continuosly requesting data from the python server. Currently, the data feed is called only once every time the 'Start Streaming' button is clicked. Change the application to continuously query the datafeed every 100ms when the 'Start Streaming' is clicked.
[goal-c] Currently, the Perspective element only shows the data in table view after the data loads. Add Perspective configurations so that when the data is loaded, it shows the historical data of ask_price ABC in the Y line chart.
Upload a git patch file as the submission to this task
Set up / Installation
In order to get the server and client application code working on your machine, follow the setup here

Note:This is the version of the JPM 2 exercise that uses Python 3. The Python 2.7 version is in this other repo

How to Run
Similar to Task 1, start the data feed server by running the python server.

Make sure your terminal / command line is in the repository first before doing any of this.

If you are using Windows, make sure to run your terminal/command prompt as administrator.

python datafeed/server3.py

If you encounter an issue with datautil.parser, run this command:

pip install python-dateutil
If you don't have pip, you can install it from: https://pip.pypa.io/en/stable/installing/

Run npm install && npm start to start the React application.

It's okay to have audit warnings when installing/running the app.

If you don't have npm (although you should if you followed the set up / installation part), you can install the recommended version alongside NodeJS from: https://nodejs.org/en/

The recommended version are node v11.0.0 and npm v6.4.1

Open http://localhost:3000 to view the app in the browser. The page will reload if you make edits.

How to fix the code to meet the objectives
To make the changes necessary to complete the objectives of this task, follow this guide.

How to submit your work
A patch file is what is required from you to submit. To create a patch file, follow this guide. Then submit the patch file in the JPM Module 2 Page.
