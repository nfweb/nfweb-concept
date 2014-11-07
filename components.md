# Core Components

##Content Management System

* Platform: PHP, Ruby
* Three Implementation proposals:
 * Enhancement of current code base
 * Customizing an existing Content Management System: Drupal 
 * Building a custom web application (based on a Content Management Framework): Symfony, Ruby on Rails

[CMS Concept](/core-cms.md)

##Webserver Platform
* platform for CMS
* production, staging and development environments
* automated deployment

Webhosting, Cloud or VPS?

Hosting location: Germany?, EU?, US? -> privacy policies

Proposals: Digital Ocean, DomainFactory, hetzner, uberspace, filoo, netcup, do.de

##Media Hosting
* Media files require large amounts of storage and are mostly static ressources
* Should not be hosted on webserver but on a dedicated file/media storage
* Some hosting services provide additional features besides simple file storage

Proposals:

* Video: Youtube, Vimeo
* Audio: Soundcloud
* Images: Flickr 
* Generic Files:

##Domain Registration & Domain Name Server
* Domains: [domains-list.md](/domains-list.md)
* SSL Certificate

##SSL Certification
* strongly recommended to ensure secure login process & administration
* Should have a wildcard certificate to include all subdomains (*.nightfever.org)

##Mail Server (MTA/MDA)
* mailboxes for users
* ```:site@nightfever.org```
* ```:firstname.:lastname@(:site.)nightfever.org```

Self hosting vs. external hosting?

##User Authentication & Management
* Single Sign On for all services provided by nightfever
* Support for external identity providers (openID etc.)
* Basic user directory

# Auxiliary Components
not initially necessary, but highly recommended to support future developments

##Search Engine
* dedicated search engine to provide distinct search and analysis features for our webservices
* better performance and custom features than on-line full-text search on the content database
* requires a destinct search engine and index

Proposals: Elasticsearch, Solr

##Web Analytics
Measurement, collection, analysis and reporting of request data to understand and optimize user experience.

Proposals: Piwik

##Support Desk
Many users will be administering Nightfever content on a regular basis. We'll need a knowledge base (guidelines, frequent tasks, tools etc.) and a support platform to handle individual issues concerning our website, website adminstration and other topics both IT-related and others.

Proposals: Discourse, Tickeding, Github, Open Atrium

##Development Blog
Informs stakeholders about development progress.
[Nightfever Web Dev](http://nfweb.github.io)
[@nfwebdev](http://twitter.com/nfwebdev)

##Data Backup
Constant data duplication to a backup site. In case anything goes wrong.

Proposals: Amazon Glacier

# Optional Components

##Dedicated Mail Delivery Agent
* massively sending mails has a performance impact
* should not be conducted on the webserver
* mail load: user notifications, automatic newsletters

Proposals: Mandrill, Mailjet, Sendgrid

##URL Shortener
* shortens urls for easy sharing (micorblogging, f2f meet)
* CMS integration assists brand recognition (in contrast to a generic shortner like bit.ly

**Suggestions:** ```n8fvr.it```, ```n8fvr.io```, ```nght.fr``` or the like

##Content Delivery Network
* increases page speed and availability
* delivers static ressources (styles, scripts, images)
* caches dynamic content

Proposals: Cloud Flare, Google App Engine, Amazon Cloudfront, Fastly

#Non-software Components

## Documentation & Guidelines
* explain usage of nightfever software systems
* enforcement of a unique content strategy
* guidance and help for web based services
* also applicable beyond the web

@See [nf-guidelines](https://github.com/nfweb/nf-guidelines)

##Support Desk 
* offers help where general information is not sufficent
* administrative tasks (admin actions) e.g. user right management, site creation

##Development Documentation
* document our proceedings and results as best as we can to make it easy to follow up
* explain reasons for decisions and how they were translated into practice
* don't leave anybody behind
