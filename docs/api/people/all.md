---
title: List all people in the database
---
<div id="body">

Returns all the people in the database, in an unspecified but consistent
order, with [pagination](/docs/api/concepts/pagination.md). 


<p class="caption">Example request</p><pre class="api">
GET /db/0SNQc00211H/people?limit=3&offset=213
</pre>

<p class="caption">Example response</p><pre class="api">
200 OK
Content-Type: application/json 
  
{ "list" : [ 
  { "id" : "0SNQe00311H",
    "name" : "test@runorg.com",
    "gender" : null,
    "pic" : "https://www.gravatar.com/avatar/1ed54d253636f5b33eff32c2d5573f70" },
  { "id" : "0SNQg00511H",
    "name" : "vnicollet@runorg.com",
    "gender" : null,
    "pic" : "https://www.gravatar.com/avatar/5a31b00f649489a9a24d3dc3e8b28060"} ],
  "count" : 215 }
</pre>



# Errors

## Returns `401 Unauthorized` 
- if the provided token and requester do not match. 

## Returns `403 Forbidden` 
- if the requester is not a database administrator

## Returns `404 Not Found`
- if the database does not exist

# Access restrictions

Only [database administrators](/docs/api/groups/admin.md) may list all people
in the database. 

Note that [viewing individuals](/docs/api/people/get.js) is open to anyone.


</div>
<nav><span class="active">List all people in the database</span></nav>