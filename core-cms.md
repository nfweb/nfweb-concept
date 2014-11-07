#Content Management System

##Implementation Variations
###Enhancement of current code base
i.e. building a custom web application without a major framework but with a head start

* would require big changes to the software architecture
* no community support

###Customizing an existing Content Management System
Overall structure is already existing, needs to be customised to meet the requirements
Example: Drupal 

###Building a custom web application
should be based on an existing Content Management Framework -> use building blocks to create the intended functionality in an efficient way
Examples: Symfony, Rails

##Features
* multilingual content
* easy content authoring
* device-agnostig design ("mobile-friendly")
* various content types
 * story
 * event
 * media (image, video, audio)
 * page (hierarchical)
 * micropost
  * reference to other content or external links
* several subsites/spaces (for each city, project etc.) integrated into a single web site
* fine-grained user management and grouping
* future proof, easily maintainable & extendable
* reliable, safe & secure
* webservice API
* social media integration
* content revisioning
* content syndication
* enhanced search feature (including facets, subsites, rich content)
* good usability & accessibility

##Platform

Ruby on Rails allows a rapid development of webapps based on a prooven and sofisticated framework, supported by a large open-source community.
Content management systems such as Drupal have a pre-defined structure of their data model, software architecture, information architecture and user guidance. It would require a lot of changes to the underlying software to tailor such a system to our specific needs.
Still it would hardy be possible do bend it all the way we want and it still includes many components and features we don't even need and never will.
So it seems preferable to build the content management system for our Nightfever website from scratch, based on a powerfull framework and supported by a vast amount of ready-to-use components, that just need to be put together to create a system that is specific to our purpose.
