THIS IS A CRUD API FOR MANAGING TO-DO LIST USING SWAGGER UI 
MADE WITH NODE+EXPRESS 


TO RUN CLONE THIS REPO FROM GITHUTB 
use 
git clone https://github.com/Devesh2126/task-api.git
   cd task-api

THEN TO INSTALL DEPENDENCIES AND START SERVER  
API WILL RUN AT LOCAL HOST
http://localhost:3000
 AND FOR SWAGGER UI INTERACTIVE DOCS 
http://localhost:3000/docs

Endpoints


GET         /           APIinfo
GET         /health     Health check
GET         /tasks      List all tasks
GET         /tasks/:id  Get a single task by id
POST        /tasks      Create a new task
PUT         /tasks/:id  Update a task
DELETE      /tasks/:id  Delete a task

EXAMPLE REQUEST 
$ curl -i -X POST http://localhost:3000/tasks -H "Content-Type: application/json" -d "{\"title\":\"Buy milk\"}"

HTTP/1.1 201 Created
X-Powered-By: Express
Content-Type: application/json; charset=utf-8
Content-Length: 40

{"id":4,"title":"Buy milk","done":false}

SWAGGER UI 
![Swagger UI example](<Screenshot 2026-07-16 181212.png>)
![Swagger ui alt example ](<Screenshot 2026-07-16 181319.png>)