#Project Brief Nightfever Web Site

* [Introduction](#introduction)
  * [Project Goals](#project-goals)
  * [Current Website](#current-website)
* [CMS requirements](#cms-requirements)
* [Users](#users)
  * [Public Users](#public-users)
  * [Editors](#editors)
* [Website Structure](#website-structure)
  * [Scopes](#scopes)
    * [Global Scope](#global-scope)
    * [City Scope](#city-scope)
    * [Project Scope](#project-scope)
  * [Content Types](#content-types)
    * [Page](#page)
    * [Story](#story)
    * [Event](#event)
    * [Micropost](#micropost)
    * [Venue](#venue)
* [Infrastructure & Environment](#infrastructure-environment)
* [Deployment](#deployment)


##Introduction
Nightfever is an international christian initiative in about 100 cities all around the world. In these cities Nightfever teams open churches during the night and invite passersby to a moment of tranquility and encounter.

###Project Goals
Due to the recent and continuing growth of Nightfever we need to focus our website on internationalisation and localizaion. The current software delivering our website is funcionally limited and faulty. It is not considered to provide a sound platform for these and any future demands.

The online services for nightfever are to be renewed in terms of design as well as the underlying software system. The most important goals and challenges are:

* internationalization and localization
* dynamic and multimedia content
* support for mobile and touch devices
* increased usability for viewers and editors
* reliable and extendable software platform
* webservice API (foundation for mobile apps, web apps and additional sites
)

The relaunced website is to be presented at the international Nightfever leaders convention at October 1st 2014.

###Current Website
Currently there are websites for some of the cities, mostly from german speaking regions, where local teams are able to publish dates, fotos, visitor statements and press references. These city websites run on the same content management system but there are hardly any interconnections besides a general city navigation list.

The website exsists in a hand full of languages, but the l10n features of the employed content management system are rather limited.

##CMS requirements

* support internationalization and multilingual content
* easy to use content authoring interface
* device-agnostig design ("mobile-friendly")
* support various content types
* several semi-independent subsites/spaces (for each city, project etc.) integrated into a single experience
* fine-grained user management and grouping
* future proof, easily maintainable & extendable
* reliable, safe & secure
* based on well proven open source software
* provide a webservice API (connect external services e.g. a future mobile app)
* social media integration
* content revisioning
* content syndication
* enhanced search features (including facets, subsites, rich content), probably a distinct search engine (perferably Elasticsearch)
* good usability & accessibility

##Users
###Public Users
####A user who looks for general information on nightfever
1. get a precise description of the idea and purpose of nightfever
2. be able to learn more about it
3. discover nightfever cities and countries
4. learn about nearby locations and dates

####A user who looks for information on a specific nightfever city
1. find upcoming events in that city
2. consume articles and media about previous events in that city
3. learn more about nightfever
4. discover nearby cities

####A regular user looking for updates on nightfever
1. get the latest news (articles, media, newsletters)
2. know about upcoming important events

####A regular user looking for updates on a specific nightfever city
1. find upcoming events in that city
2. read latest news from that city
3. learn about important news from other cities and global

####A user who wants to participate or start Nightfever in his city
1. get background information on nightfever
2. know how he can participate

####A media representative
1. find press announcements
2. get general information on nightfever

###Editors
Are usually unexperienced in terms of content authoring and website administration.
Work on a local level, each city and project beeing responsible for their content.

## Website Structure
Individual websites/landing pages and subsites:

* international landing page (multilingual): nightfever.org
* landing pages for cities (usually monolingual, some with 2 or more languages): ~100 cities atm (e.g. bamberg.nightfever.org)
* landing pages for specific projects, recurring events etc. (mono- or multilingual)
* landing pages for countries or regions (usually monolingual, some with 2 or more languages)

All these websites have some sub pages like articles, events and static pages.

The navigation concept should include

* switching between different localizations of the current page (if available)
* show related entities of a certain site (city -> country, event -> city)
* show the total amount of cities and projects
* nearby nightfever cities
* upcoming events in nearby cities

###Scopes
Each scope acts as an independent website and build their own distinguished domain, creating an individual hierarchy and containing content from all other content types.
User permissions are given on a scope domain.

The landing page of each scope should be customizabe using some common elements:

* news feed
* navigation
* teasers
* upcoming events
* media elements

####Global Scope
The general landing page ```nightfever.org``` represents the global scope.

This includes overviews over cities and regions, events etc.

####City Scope
Cities are in general equivalent to local Nightfever groups.

####Project Scope
Projects resemble generic Nightfever groups working on specific projects like common events and specials.

Examples: Nightfever Akademie, Nightfever Weekend, Nightfever Leiterwochenende, Katholikentag, Kongress Freude am Glauben

###Content Types

####Page
Static webpage

Fields: title, body

#### Story
Full-featured articles (blog posts).
Includes enhanced authoring features, teaser.

Fields: title, excerpt, image, body, author, tags, category

#### Event
Fields: title, date_begin, date_end, body, image, event_type, venue, tags

Several event types: Nightfever (evening), specials, team gathering, etc.

#### Micropost
A short text post with the ability to reference internal or external content (similar to a tweet or status update) including a preview of the referenced content.

* internal content from the parent or other sites (promote events, stories etc)
* external and 3rd party references to websites, files, media (image, video, audio, gallery, playlist)

####Venue
Venues represent the usually recurring event locations of Nightfever evenings, but also other events.

Fields: title, description, image, address

####Statement
Statements from visitors.

Fields: body, cited_person

## Infrastructure & Environment

* external media hosting provider (third party & self hosted)
* central user directory: We want to provide our users a single sign on solution for all our services (CMS backend, mail accounts, support desk, intranet etc.). This means a centralized user management including roles, permissions and user groups. Besides local authentication users should be able to authenticate by external identity providers (openID, Facebook connect etc.).
* Web Analytics: Measurement, collection, analysis and reporting of request data to understand and optimize user experience. Self-hosts, preferably Piwiki)
* Support plattform: Many users will be administering Nightfever content on a regular basis. We'll need a knowledge base (guidelines, frequent tasks, tools etc.) and a discussion/issue management platform to handle individual issues.
* Backup plan: Constant automatic backup task inklusing code and content

## Deployment
Continuity of important legacy components:

* Existing URLs still hold or redirect to their content ("Cool URIs don't change"
)
* Existing domain names continue to exists


