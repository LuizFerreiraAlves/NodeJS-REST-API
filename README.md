# NodeJS-REST-API

Creating basic REST APIs (GET, POST, PATCH and DELETE) using Node.js for scheduling services in a pet shop.<br>
You can use cURL or an API tool like POSTMAN to test the application.<br>
It stores the records in a MySQL database composed of a single table whose columns are:

- id int NOT NULL AUTO_INCREMENT PRIMARY KEY (not handled by user)<br>
- cliente varchar(50) NOT NULL<br>
- pet varchar(20)<br>
- servico varchar(20) NOT NULL<br>
- data datetime NOT NULL (not handled by user)<br>
- dataCriacao datetime NOT NULL<br>
- status varchar(20) NOT NULL<br>
- observacoes text<br>

1-)First of all you should open a cmd or shell editor, go to the main path and run "npm start" to start the application.

2-) Once it's running, you can test the following APIs:<br>
  2.1-) GET /atendimentos to retrieve all the records of the table.<br>
  2.2-) GET /atendimentos/id to retrieve a single record in the "id" position.<br>
  2.3-) POST /atendimentos to insert a record.<br>
  2.4-) PATCH /atendimentos/id to update the record in "id" position.<br>
  2.5-) DELETE /atendimentos/id to delete the record in "id" position.<br>
  
<b>Note that we can update and insert the information: cliente, pet (optional), servico, dataCriacao, status and observacoes (optional)
</b>
