---
title: List all people in the database
---
<div id="body">

`RunOrg.Person.List(limit, offset)` reads `limit` people from the 
database, starting at `offset`. The order is unspecified but 
consistent. 

Returns a [promise](/docs/js/concepts/promise.md) that will resolve to a 
list of filled `RunOrg.Person` instances. 


<p class="caption">Example usage</p><pre class="js">
RunOrg.Person.List(10, 0).then(function(list) {
  for (var i = 0; i < list.length; ++i) 
    console.log("Person %s is %s", list[i].id, list[i].label)    
})			 
</pre>



# Errors

## Returns `401 Unauthorized` 
- if the provided token and requester do not match. 

## Returns `403 Forbidden` 
- if the requester is not a database administrator

## Returns `404 Not Found`
- if the database does not exist

# Access restrictions

Only [database administrators](/docs/js/groups/admin.md) may list all people
in the database. 

Note that [viewing individuals](/docs/js/people/get.js) is open to anyone.


</div>
<nav><span class="active">List all people in the database</span></nav>