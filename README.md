Airbnb
Project description

Related Projects
https://github.com/teamName/repo
https://github.com/teamName/repo
https://github.com/teamName/repo
https://github.com/teamName/repo
Table of Contents
Usage
Requirements
Development
Usage
Some usage instructions:

- npm install
- npm start
- npm run react-dev
- from database dir run node createTables.js to initailize DB with mock data.

Requirements:
An nvmrc file is included if using nvm.

Node 6.13.0
etc
Development:
App: StayKay
Page: Location info page
Service: Availability micro service
Developers: Jacob Knudsen
Design Overview:
The Availability service is designed to allow users to check availability and book dates to reserve locations.
This service uses MySQL, because the data associated with a location is relational, and MySQL provides guaranteed referential integrity for relational datasets with minimal development overhead.
REST API’s:
GET /availability/:locationname =>retrieves all dates that are unavailable for this location as JSON.
Example response: ‘[03/10/2020, 03/11/2020]’
POST/availability/:locationname => adds new dates that will be booked for the location with the name declared in the “/:locationname” parameter.
Schema:
