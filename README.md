# EvoArch
Evolutionary Archive of your solutions


### Concept

There was a need to track versions of software/databases/docker containers in solutions. Because of security, not all servers could be reached by the version tracking deployment server. Thus, the solution should be capable of self-scrapping data and of manually inserting the version of the solution to be tracked.

No such solution was found, appart from osquery or netbox, that are not quite there.

The software should allow users to add a resource, add some details, add tags (servers?), and the category.

The category is a nested system, where you can put a category in a category.

You could have Home servers -> multimedia -> server01

Osquerry could be used to get up-to-date data, NetBox could be used to get the device on which the solution is running.

The checking of the version could be done with modules, as in, a module for checking the docker image, a module to check the pip version, database.

The modules should be as easy as possible, so that they can be just copy pasted in the system and work, so that one can make its own module (useful?)

### To-do
- modular design for version tracking
- implement [osquerry](https://www.osquery.io/) to get up-to-date data from servers
- implement [NetBox](https://demo.netbox.dev/) to connect which devices have what
