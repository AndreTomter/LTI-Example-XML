# LTI-Example-XML
A simple example to understand how Learning Tool Integrations (LTI) work in your Learning Management System (LMS)

It is a simple “Hello Library” example which does the following:

* Places a button in the course navigation menu
* Displays a library home page (or any other page) listed between the <blti:launch_url></blti:launch_url> tags

##Extend it

* Upload the launch.html page to your web server (or create your own launch page). You can update it to be a custom page for those visiting from within the LTI
* Update the <blti:launch_url></blti:launch_url> tag to point to the page
* This is your “Launch Page”
* Make sure it is hosted on https (since will be displayed within an iframe in an https page

## Beware of nested sites
Before you go ahead and just display your standard website within the LTI frame, think about if you really want to display a website inside of a website inside of a website. Is that really the user experience you are going for?
