# zEM

![GitHub top language](https://img.shields.io/github/languages/top/pak-center/zem?style=plastic)
![Lines of code](https://img.shields.io/tokei/lines/github/pak-center/zem?label=total%20lines%20of%20code&style=plastic)
![GitHub](https://img.shields.io/github/license/pak-center/zem?style=plastic)

**zEM** - **z/arch Enterprise Monitor** sends z/VM *MONITOR events in real time to Android app users on mobile or watch devices. 
## Table of contents

* [General info](#general-info)
* [Technologies](#technologies)
* [Usage](#usage)
* [Features](#features)
* [Roadmap](#roadmap)
* [TODO](#todo)
* [Installation](#installation)
* [Run the Project](#run-the-project)
* [License](#license)

## General Info

**z/arch Enterprise Monitor** AKA **zEM** is open source software that sends system events in real time to users hooked up to it via an Android cell phone or an Android watch. 

### Supervisors in constant contact such as:

* System Operators,
* System Admins
* Security Stuff
* Others with such a requirement and with assigned access.

Software works under z/Linux inside z/VM supervisor installed in LPAR or other z/VM. Connects with /dev/monreader assigned to Saved Sagment MONDCSS of z/VM memory area.

### Two operational modes quite like CP *MONITOR service:
* Event
* Sample

### Available approaches related to data gathering:
* just in real time sending msgs to connected clients via TCP/IP with no archive on DASD disks
* as above but with MINIMUM Event archive inside PostgreSQL database (remotly or on site)
* as above but with FULL Event & Sample archive inside PostgreSQL database (remotly or on site)
* Separate database for Event & Sample records (every record type inside their own table)

## Technologies

* IBM mainframe
* z/VM 
* z/Linux
* PostgreSQL database
* REST
* Rust (Actix Web, Tokio)

## Usage

## Features

| Feature | % Progress | Status |
| :---    | :---       | :---:  |
| z/VM V7.3 Event Records | # | Ongoing  |
| z/VM V7.3 Sample Records |  | Awaits |
| Config file handling | ## | Ongoing |
| non-blocking READ | ## | Ongoing |
| TCP/IP server |  | Awaits |
| RESTfull |  | Awaits  |
| PostgreSQL database | ## | Ongoing |
| Log | # | Ongoing |
| Authorization |  | Awaits |
| Beautify code | | Awaits |

## Roadmap

- [x] Add README
- [ ] Add DOCS & Graphs
- [ ] Add source code to Github
- [ ] Estabilish records for z/VM V7.3

## TODO

## Installation

## Run the Project

## License

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
