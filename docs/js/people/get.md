---
title: Fetch basic information for a person
---
<div id="body">

If `person` is an instance of [`RunOrg.Person`](/docs/js/people/person.md), 
then `person.Load()` fills (or replaces) its non-`id` fields with 
data retrieved from the API.

Returns a [promise](/docs/js/concepts/promise.md) that will resolve to the
`person` object if it could be filled.  


<p class="caption">Example usage</p><pre class="js">
new RunOrg.Person("1ax69bfa335").Load().then(function(person) {     
  console.log("Fetched data for %s.", person.label)
})
</pre>

<p class="caption">Example usage, with error handling</p><pre class="js">
var person = new RunOrg.Person("1ax69bfa335");

person.Load().then(function() {     
  console.log("Fetched data for %s.", person.label)
}, function(error) {
  if (error.HTTP == 404) 
    console.log("Person %s not found.", person.id)
  else 
    console.log("An error happened: %o", error)
})
</pre>



# Errors

## Returns `404 Not Found`
- if the database does not exist,
- if person `{id}` does not exist in the database.

# Access restrictions

Anyone can view any person's basic information, if they have their identifier.


</div>
<nav><span class="active">Fetch basic information for a person</span></nav>