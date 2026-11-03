# CampusEats Catalogue — Assignment 8

Name - Prerna
Roll No. - 20251651072

Service chosen: CampusEats Catalogue / Menu service

Routes:
- GET /items — list all menu items
- GET /items/:id — fetch one item by ID
- POST /items — create a new menu item

Status codes used:
- 200 OK — successful GET on /items and GET /items/:id
- 201 Created — successful creation through POST /items
- 404 Not Found — item id does not exist in GET /items/:id
- 422 Unprocessable Entity — missing required name field in POST /items

How req.params and req.body are used:
- req.params is used in GET /items/:id to read the id from the URL, for example /items/2.
- req.body is used in POST /items to read the JSON payload sent by the client, such as { "name": "Burger", "price": 120 }.
- POST needs express.json() so Express can parse JSON data from the request body before we read it.

Run locally:
1. npm install
2. node server.js
3. Open http://localhost:3000

Google Drive / screenshots:
- Add the demonstration video link here.
- Add the before/after screenshots here.

This project follows the CampusEats Catalogue tutorial pattern and exposes a simple REST API with a front-end page that reads and writes menu data.
