# NodeJS-REST-API

Creating basic REST APIs (GET, POST, PATCH and DELETE) using Node.js for scheduling services in a pet shop.
You can use cURL or an API tool like POSTMAN to test the application. 
It stores the records in a MySQL database composed of a single table whose columns are:

- id int NOT NULL AUTO_INCREMENT PRIMARY KEY (not handled by user)
- cliente varchar(50) NOT NULL
- pet varchar(20)
- servico varchar(20) NOT NULL
- data datetime NOT NULL (not handled by user)
- dataCriacao datetime NOT NULL
- status varchar(20) NOT NULL
- observacoes text

1-)First of all you should open a cmd or shell editor, go to the main path and run "npm start" to start the application.

2-) Once it's running, you can test the following APIs:
  2.1-) GET /atendimentos to retrieve all the records of the table.
  2.2-) GET /atendimentos/id to retrieve a single record in the "id" position.
  2.3-) POST /atendimentos to insert a record.
  2.4-) PATCH /atendimentos/id to update the record in "id" position.
  2.5-) DELETE /atendimentos/id to delete the record in "id" position.
  
<b>Note that we can update and insert the information: cliente, pet (optional), servico, dataCriacao, status and observacoes (optional)
</b>
