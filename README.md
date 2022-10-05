# API-TODO
Project CRUD, API Rest Node with Express and MongoDB Atlas.<br>
Depolyed in Heroku, URL for test > https://dashboard.heroku.com/apps/todo-app-nodejs-tiago-play <br>

<b>You can test the follow routes:</b> <br><br>

<b>Create and login User</b><br>
/session<br>
<b>Method:</b> Post

<b>Requisition body (type json):</b><br>
{"username": "user@gmail.com"}<br>

Now for the next routes we simulated like the user are logged in. <br>
Only the user_id who created the todo can execute the methods.<br>



<b>Create todo<br></b>
/todo/:user_id<br>
<b>Method:</b> Post<br>
<b>Example of requisition body</b>
{
	"description": "test",
	"done": true
}

<b>Get todo</b>
/todo/:user_id<br>
<b>Method:</b> Get<br>
Hans't body

<b>Update todo</b>
/todo/:user_id/:todo_id<br>
<b>Method:</b> Patch <br>
<b>Example of requisition body</b>
{
	"description": "write the readme file", "done": false
}

<b>Delete todo</b>
/todo/:user_id/:todo_id<br>
<b>Method:</b> Delete <br>
Hans't body
