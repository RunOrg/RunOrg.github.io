---
title: People
---
<div id="body">

A human **person** is a type of entity used throughout the RunOrg API 
for many  purposes, the most important being:  

- Message and email recipients are always people. All sending APIs
  expect either individuals or [groups](/docs/api/groups.md) of people 
  as their parameters.
- Everyone who logs in, using any method, is bound to a person. 
- Access restrictions are based on the [person who performs the
  action](/docs/api/auth.md).



# Person information

The type [`<person>`](/docs/api/people/person.md) contains basic information 
about a person, just enough to be able to display their identity : a 
human-readable name, a small picture and (if available) their gender. 

This type is returned when retrieving lists of people (because it uses
less bandwidth than fetching the entire profile) and in situations 
where obtaining a person's data is not the main purpose of the request
(for example, when fetching a list of messages, basic information
is provided about each author as a matter of convenience).    


<table class="files"><tr><td>
`type <person>`
</td><td><a href="/docs/api/people/person.md">Short information about a person</a></td></tr><tr><td>
`GET /db/{db}/people`
</td><td><a href="/docs/api/people/all.md">List all people in the database</a></td></tr><tr><td>
`GET /db/{db}/people/{id}`
</td><td><a href="/docs/api/people/get.md">Fetch basic information for a person</a></td></tr></table>


</div>
<nav><ul class="above"><li><a href="/docs/api/index.md">RunOrg documentation</a></li></ul><span class="active">People</span><ul class="below"><li><a href="/docs/api/people/person.md">Short information about a person</a></li></ul></nav>