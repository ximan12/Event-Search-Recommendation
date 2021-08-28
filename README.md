# Introduction
Event Search and Recommendation Engine is a full stack project powered by TicketMaster, whose purpose is to recommend events based on logged in user's current geo-location.(userid:1111 pwd:2222).

## Recommendation Algorithm(content-based)
1. Fetch all the events (ids) this user has visited. 
2. Given all these events, fetch the categories of these events. 
3. Given these categories, find what are the events that belong to them. 
4. Filter events that this user has visited. 
5. Sort the recommendation list on ascending order of distance between recommended events's locations and user's location.

## Requirements
* Apache Tomat v9.0
* Eclipse JEE
* JAVA 8
* MySQL

## Installation
Clone the GitHub repository and then import Event-Search-Recommendation-Engine.war into your eclipse.

```
git clone https://github.com/weijian2/Event-Search-Recommendation-Engine
```
To import WAR file into Eclipse JEE, click on File -> Import. Select Web -> WAR File.
* **WAR** file: Provide the full pathname of the WAR file on your computer.
* **Web project**: This will pre-fill based on the WAR file name. You can change it, which is handy if
you’re experimenting.
* **Target runtime**: You will need to select “Apache Tomcat 9.0”. The first time you import a WAR
file (or create new “Dynamic Web Project”) you will need to declare the new runtime environment. Do this by clicking on “New” and filling in the form as follows:
	* **Apache Tomat v9.0**, then click “Next”
	* Provide the Tomcat installation directory by giving the full pathname of the directory
containing your unzipped version of Tomcat 9.0.
	* Click “Finished”.
* Click "Finished".

Run the imported project by “right-clicking” on the new project and selecting “Run As -> Run on Server. <br>

## Usage/Quick Start
Login using demo account and password(1111/2222)

## Deployment
Deployment Environment: Amazon EC2 <br>
[demo link](http://54.202.63.63/Event-Search-Recommendation-Engine/) <br>

