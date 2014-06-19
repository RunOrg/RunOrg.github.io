---
title: Fetch basic information for a person
---
<div id="body">

Returns a [`<person>`](/docs/api/people/person.md) representation of the person with
identifier `{id}` in database `{db}`. 


<p class="caption">Example request</p><pre class="api">
GET /db/0Et4X0016om/people/0Et9j0026rO
</pre>

<p class="caption">Example response</p><pre class="api">
200 OK 
Content-Type: application/json

{ "id" : "0Et9j0026rO",
  "label" : "Victor Nicollet",
  "gender" : "M", 
  "pic" : "https://www.gravatar.com/avatar/648e25e4372728b2d3e0c0b2b6e26f4e" }
</pre>



# Errors

## Returns `404 Not Found`
- if the database does not exist,
- if person `{id}` does not exist in the database.

# Access restrictions

Anyone can view any person's basic information, if they have their identifier.


</div>
<nav><span class="active">Fetch basic information for a person</span></nav>