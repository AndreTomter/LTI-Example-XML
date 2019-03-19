# LTI-Example-XML
A simple example to understand how Learning Tool Integrations (LTI) work in your Learning Management System (LMS)

It is a simple “Hello Library” example which does the following:

* Places a button in the course navigation menu
* Displays a library home page (or any other page) listed between the <blti:launch_url></blti:launch_url> tags

## Install

To install you must have a course in your LMS as well as the ability to make course-level installs

* Go to your course settings
* Install the app. For example, in Canvas go to Apps then View App Configuration then Add App
* Choose Paste XML
* Give it a name (this only identifies it in your app list)
* Paste in the XML
* If you are hosting your own launch.php file, change the url between <blti:launch_url></blti:launch_url> and <lticm:property name="url"></lticm:property name="url"> to point to the location of your launch file
* Save and then you may need to refresh to get it to show up in the course navigation

## Extend it

* Upload the launch.php page to your web server. You can update it to be a custom page for those visiting from within the LTI
* Update the <blti:launch_url></blti:launch_url> tag to point to the page
* This is your “Launch Page”
* Make sure it is hosted on https (since will be displayed within an iframe in an https page
* Also make sure you can make POST requests to it (otherwise you'll get a 405 error)

## Beware of nested sites
Before you go ahead and just display your standard website within the LTI frame, think about if you really want to display a website inside of a website inside of a website. Is that really the user experience you are going for?

## Learn more
You can go to https://www.edu-apps.org/build_xml.html to build your own XML and learn more.

