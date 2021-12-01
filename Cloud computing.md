# Cloud computing

**Authors:**
Brian Hayes

**Pub info:**
https://dl.acm.org/doi/abs/10.1145/1364782.1364786

**Funding:**


**Citation**
```
@article{10.1145/1364782.1364786,
author = {Hayes, Brian},
title = {Cloud Computing},
year = {2008},
issue_date = {July 2008},
publisher = {Association for Computing Machinery},
address = {New York, NY, USA},
volume = {51},
number = {7},
issn = {0001-0782},
url = {https://doi.org/10.1145/1364782.1364786},
doi = {10.1145/1364782.1364786},
abstract = {As software migrates from local PCs to distant Internet servers, users and developers alike go along for the ride.},
journal = {Commun. ACM},
month = {jul},
pages = {9–11},
numpages = {3}
}
```


## Key Ideas and one paragraph abstraction
Overview of cloud computing in 2008.

### Abstruct
> THE GREEk MYTHS tell of creatures plucked from the surface of the Earth and enshrined as constellations in the night sky. Something
similar is happening today in the world of computing. Data and programs are being swept up from desktop PCs and corporate server rooms and installed in “the compute cloud.”
Whether it’s called cloud computing or ondemand computing, software as a service, or the Internet as platform, the common element is a shift in the geography of computation. When you create a spreadsheet with the Google Docs service, major components of the software reside on unseen computers, whereabouts unknown, possibly scatered across continents.

### Key ideas
- management of computing resource
- cost of managing and deveoping software
- provide high performance computation with enabling mobility


## Context

Migration from desktop and the cooporate server room to cloud.

## Historical sense

#### In 1950's: 

- service vureaus and time-sharing system
    - provide computing machinery for who lacked a mainframe in a glass-walled room
    - hub-and-spoke configuration
    - Users communicate to central over telephone line

#### In 1980's: 
- **Arrival of personal computers**
    - "liberating " programs and data from the central computing center.[1]
    - controlling their own computing environment
    - choosing software to suit their needs
    - customizing systems to their tastes
#### Currently (2008):
- **Cloud computing**: 
    - functions migrating outword to distant data centers reached through th Internet.
    - no hub (difference from hub-and-spoke topology) but **a core and a fringe**
    - client computer can communicate with many servers at the same time
    - some servers also exchange information among themselves

## Why this change is happening?
- For the individual
    - total control comes at a price
        - software update
        - OS, low-level utilities
        - subsequent revisions to other programs
    - mobility
    - collaboration
- For software vendors
    - similar to individual
    - software required to cope with a baffling variety of environment
        - In contrast, Internet-based software service can developed, tested, and run on a platform vendor's choosing.


## Architecture / A core and a fringe 
- **Concentrate computation and storage in the core**
    - high performance machines are linked by high-bandwidth connections
    - all of these resources are carefully maganed
- **A Fringe as end users**
    - making the requrests that initiate computations and who reseive the results

## Future direction
- **Wordstar for the WEB**
    - software application like google spreadsheet, adobe photoshop as online service
- **Enterprise computing in the cloud** 
- **Cloudy infrastructure**
    - e.g. AWS
- **The cloud OS**
    - eyeOS system, all the desktop functionality live in the browser window. (icons for files, folders, application)

## Operation issues
- **Scalability**
    - Handling hundreds or thousands of requests per second.
    - Coordination of information coming from multiple sources even from difference organization.
    - many-to-many communication 
        - sever talking to multiple clients
        - each client invoking programs on multiple servers
- **browser-based UI**
    - duplicating conventional computer's functionality inside WEB browser
    - choise developing tools for WEB based software is limited
        - languages, code libraries, and application frameworks
- **Master multiple languages and operating environment**
    - back-end process relis on a relational database (SQL)
    - client-side, JavaScript within HTML
    - Standing between them: Script language(PHP, Java, Python, ...)
## Technical Terms
- **XX**
  > AA

## Related papers / repo


## Next paper
- [A view of cloud computing](https://dl.acm.org/doi/10.1145/1721654.1721672)

<!-- Refs -->


---

## Reference

- [1]Computer lib: Dream machines
```
@book{nelson1987computer,
  title={Computer lib: Dream machines},
  author={Nelson, Theodor H and Nelson, Theodor H},
  year={1987},
  publisher={Tempus Books of Microsoft Press Redmond, WA}
}
```
