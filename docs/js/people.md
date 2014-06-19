---
title: People
---
<div id="body">

A human **person** is a type of entity used throughout the RunOrg API 
for many  purposes, the most important being:  

- Message and email recipients are always people. All sending APIs
  expect either individuals or [groups](/docs/js/groups.md) of people 
  as their parameters.
- Everyone who logs in, using any method, is bound to a person. 
- Access restrictions are based on the [person who performs the
  action](/docs/js/auth.md).



# Class `Person`

The class [`RunOrg.Person`](/docs/js/people/person.md) contains basic 
information about a person, just enough to be able to display their 
identity : a human-readable name, a small picture and (if available) 
their gender. 

This class is used when retrieving lists of people (because it uses
less bandwidth than fetching the entire profile) and in situations 
where obtaining a person's data is not the main purpose of the request
(for example, when fetching a list of messages, basic information
is provided about each author as a matter of convenience).  


<table class="files"><tr><td>
`class RunOrg.Person`
</td><td><a href="/docs/js/people/person.md">Short information about a person</a></td></tr><tr><td>
`static RunOrg.Person.List`
</td><td><a href="/docs/js/people/all.md">List all people in the database</a></td></tr><tr><td>
`method RunOrg.Person.Load`
</td><td><a href="/docs/js/people/get.md">Fetch basic information for a person</a></td></tr></table>


# Class "Person.Profile"

The class [`RunOrg.Person.Profile`](/docs/js/people/profile.md) contains full 
information about a person. 



# Complete profile

The type [`<person:profile>`](/docs/js/people/profile.md) contains full 
information about a person. 



</div>
<nav><ul class="above"><li><a href="/docs/js/index.md">RunOrg documentation</a></li></ul><span class="active">People</span><ul class="below"><li><a href="/docs/js/people/person.md">Short information about a person</a></li></ul></nav>