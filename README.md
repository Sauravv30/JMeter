# JMeter
This is Jmeter repo for jmeter load testing

After you are ready with .jmx file that contains the test scenarios, Saved from Junit UI:

Use this command to run the load testing in non interactive mode
  # jmeter -n -t "<.jmx-file-path>" -l "<results-file-path>.csv" 
	
Steps to create a dashboard file:
1.Add 'Summary Report', 'Simple Data Writer' from Listeners.
2.Set location to generated csv
3.open reportgenerator.properties from "apache-jmeter-5.6.3\bin\" copy all content from it
4.Open user.properties from same bin folder
5.Append all from reportgenerator.properties to user.properties and save
6.Now run the your Test script
7.open cmd and enter
  # jmeter -g "<results-file-path>.csv"v -o E:\Workspace\HRS

Go to E:\Workspace\HR and open index.html and you can check your test result
