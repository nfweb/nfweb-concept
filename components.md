#ToC
1. [Core Components](#core-components)
2. [Auxiliary Components](#auxiliary-components)
3. [Optional Components](#optional-components)
4. [Non-software Components](#non-software-components)

# Core Components

##Content Management System

* Platform: PHP, Ruby
* Three Implementation proposals:
 * Enhancement of current code base
 * Customizing an existing Content Management System: Drupal 
 * Building a custom web application (based on a Content Management Framework): Symfony, Rails

[CMS Concept](/core-cms.md)

##Webserver Platform
* Requirements: SSH, Git, software requirements

Webhosting, Cloud or VPS?

Hosting location: Germany?, EU?, US? -> privacy policies

Proposals: Digital Ocean, DomainFactory, hetzner, uberspace, filoo etc.

##Media Hosting
* Media files require large amounts of storage and are mostly static ressources
* Should not be hosted one webserver but on a dedicated service
* Some hosting services provide additional features besides simple file storage

Proposals:

* Video: Youtube, Vimeo
* Audio: Soundcloud
* Images: Flickr 
* Generic Files:

##Domain Registration & Domain Name Server
* Domains: nightfever.org
* SSL Certificate
* What about managing different domains? (nightfever-[:city].de)

##SSL Certification
* strongly recommended to ensure secure login process & administration
* Should have a wildcard certificate (*.nightfever.org)

##Mail Server (MTA/MDA)
* mailboxes for users
* ```:site@nightfever.org```
* ```:firstname.:lastname@(:site.)nightfever.org```

Self hosting vs. external hosting?

##User Authentication & Management
* Single Sign On for all services provided by nightfever
* Support for external identity providers (openID etc.)
* Basic user directory

This would also be a part of the Nightfever Intranet.

# Auxiliary Components
not initially necessary, but highly recommended to support future developments

##Search Engine
* A large content base is not applicable to an on-line full-text search on the content database 
* requires a destinct search engine and index

Proposals: Solr, Elasicsearch

##Web Analytics
Measurement, collection, analysis and reporting of request data to understand and optimize user experience.

Proposals: Piwik

##Support Desk
Many users will be administering Nightfever content on a regular basis. We'll need a knowledge base (guidelines, frequent tasks, tools etc.) and a support platform to handle individual issues.

This would also be a part of the Nightfever Intranet.

Proposals: Discourse, Tickeding, Github, Open Atrium

##Development Blog
Informs stakeholders about development progress.

Proposal: Simple blog 

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
