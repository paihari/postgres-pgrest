
Exposure of PostGres Database tables as REST API

(base) bantwal@Hariprasads-MacBook-Air ~ % curl http://localhost:3000/employee
[{"id":1,"name":"Mickex","age":12,"department":"QA"}]%                                                                           (base) bantwal@Hariprasads-MacBook-Air ~ % payload='{"name": "John Doe", "age": 30}'

(base) bantwal@Hariprasads-MacBook-Air ~ % curl -X POST -H "Content-Type: application/json" -d "$payload" http://localhost:3000/employee

(base) bantwal@Hariprasads-MacBook-Air ~ % curl http://localhost:3000/employee      
[{"id":1,"name":"Mickex","age":12,"department":"QA"}, 
 {"id":2,"name":"John Doe","age":30,"department":null}]%                  
 
