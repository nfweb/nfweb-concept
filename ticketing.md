#Ticketing System

First, we need an [issue tracking system](http://en.wikipedia.org/wiki/Issue_tracking_system) for software development process.

##Bugzilla
I would prefer Bugzilla 'cause we can use it as a bug tracking system. It is the best known and most widely used open source bug tracking system. Bugzilla is used, among others, by Mozilla Foundation, Wikimedia Foundation, NASA, GNOME, KDE, Apache, Red Hat and Novell. It can track bugs and code changes, communicate with teammates, submit and review patches and manage quality assurance (QA). Particularly interesting for the nightfever website development is Whining (Function for remembering forgotten problems via email). We can also use it as a Nightfever Help Desk.

System Requirements:
* compatible dbs (e.g.: MySQL, Oracle, SQLite)
* Perl 5
* assortment of Perl modules
* compatible web server (any web server that supports CGI)
* MTA or SMTP server

#Help Desk
We also need a Nightfever Help Desk (NHD) 

##osTicket

An other open source ticketing systems is osTicket. It is also widely-used and used a simple, easy-to-use, multi-user, web-based customer support platform. Maybe we can use it as NHD 'cause osTicket includes all features we need:
* Custom Fields 
* Ticket Filters
* Configurable help topics for web tickets
* Ticket locking mechanism (allow staff to lock tickets during response)
* Assign tickets to a staff or to a team
* Auto-Responder
* Internal Notes
* SLA (Service Level Agreements)
* Customer Portal (login via email and ticket ID without registration/user account)
* Dashboard Reports

System Requirements:
* PHP 5.3 (or better) 
* MySQL 5 (or better) 
* Web server
