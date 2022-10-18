# API-TODO
Project CRUD, API Rest Node with Express and MongoDB Atlas.<br>



Deployed in Heroku, URL for test online > https://dashboard.heroku.com/apps/todo-app-nodejs-tiago-play <br>

If you prefer you can dowload the project in your computer, in both cases it's necessary use an API clients like Insomnia or Postman<br>
Script to run the project: <b>npm run dev</b>

<b>Dependencies used at this project:</b> Cors, Dotenv, Express, Mongoose<br> 
<b>Dev Dependencies:</b> Nodemon

<b>You can test the follow routes:</b> <br><br>

<b>Create and login User:</b> /session<br>
<b>Method:</b> Post <br>
It's necessary to create the user and copy the <b>user_id</b><br>
<b>Requisition body (type json):</b><br>
{"username": "user@gmail.com"}<br>

Now for the next routes we simulated like the user are logged in. <br>
Only the user_id who created the todo can execute the methods.<br>

<b>Create todo: </b> /todo/:user_id<br>
<b>Method:</b> Post<br>
<b>Example of requisition body</b>
{
	"description": "test",
	"done": true
}

<b>Get todo:</b> /todo/:user_id<br>
<b>Method:</b> Get<br>
Hans't body

<b>Update todo: </b> /todo/:user_id<br>
<b>Method:</b> Patch <br>
<b>Example of requisition body: </b> { "description": "write the readme file", "done": false }

<b>Delete todo</b>
/todo/:user_id/:todo_id<br>
<b>Method:</b> Delete <br>
Hans't body
