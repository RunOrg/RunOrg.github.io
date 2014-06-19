---
title: Short information about a person
---
<div id="body">

This object contains basic information about a person, just enough 
to be able to display their identity : 


<pre class="json">
{ "id": "1c39461xbF3",
  "label": "Victor Nicollet",
  "gender": "F",
  "pic": "https://www.gravatar.com/avatar/5a31b00f649489a9a24d3dc3e8b28060?d=identicon" }
</pre>

<table class="files"><tr><td>
`GET /db/{db}/people`
</td><td><a href="/docs/api/people/all.md">List all people in the database</a></td></tr><tr><td>
`GET /db/{db}/people/{id}`
</td><td><a href="/docs/api/people/get.md">Fetch basic information for a person</a></td></tr></table>


For privacy purposes, the short information will never include contact information,
such as a _full_ e-mail address or phone number. To ensure that this is the case, 
make sure you correctly classify any contact information as such. 

</div>
<nav><ul class="above"><li><a href="/docs/api/index.md">RunOrg documentation</a></li><li><a href="/docs/api/people.md">People</a></li></ul><span class="active">Short information about a person</span></nav>