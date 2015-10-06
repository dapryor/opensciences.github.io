---
title: <form class="form-horizontal" action="http://formspree.io/openscience.content@gmail.com" method="POST"><fieldset><legend><h1>Donate your dataset (one per submission)</h1></legend><div class="form-group"><div class="col-md-12"><input id="suggest-name" name="suggest-name" type="text" placeholder="Name of Dataset" class="form-control input-md"></div></div>

layout: repo-dataset
category: contribute
---
<div class="control-group"><div class="controls"><select id="category" name="category" class="form-control input-xlarge" required><option></option>{% for category in site.datacategories %}<option>{{category.title}}</option>{% endfor %}</select></div></div>

#URL

* <div class="form-group"><div class="col-md-6"><input placeholder="All links to data sets" id="link-to-dataset" name="link-to-dataset"   type="text" class="form-control input-md" required></div></br>
* <div class="form-group"><div class="col-md-6"><input id="paper-link" name="paper-link" type="text" placeholder="Paper in ACM/IEEE Digital Library" class="form-control input-md" required></div></br></br>

#Change Log

Who | When
---- | ----
<div class="form-group row"><label class="col-md-2 control-label" for="suggest-name">Donated by</label><div class="col-md-3"><input id="donators-name" name="donators-name" type="text" placeholder="Donator's Name" class="form-control input-md"></div><div class="col-md-3"><input id="donators-email" name="donators-email" type="text" placeholder="Donator's Email" class="form-control input-md"></div> |  <div class="form-group col-md-4"><input id="date" name="date" type="text" placeholder="Date" class="form-control input-md"></div></div>

#Reference

Studies who have been using the data (in any form) are required to include the following reference:


<!-- Textarea -->
<div class="form-group">
  <div class="col-md-12">
    <textarea placeholder="BibTex" class="form-control" id="bibtex" name="bibtex"></textarea>
  </div>
</div>


#About the Data

###Overview of Data

<!-- Textarea -->
<div class="form-group">
  <div class="col-md-12">
    <textarea placeholder="Provide background info here" class="form-control" id="overview" name="overview" required></textarea>
  </div>
</div>


###Attribute Information

<!-- Textarea -->
<div class="form-group">
  <div class="col-md-12">
    <textarea placeholder="Give us some context about the attributes, if applicable." class="form-control" id="authors" name="authors"></textarea>
  </div>
</div>


###Paper Abstract
<!-- Textarea -->
<div class="form-group">
  <div class="col-md-12">
    <textarea placeholder="Provide the paper's abstract here" class="form-control" id="abstract" name="abstract"></textarea>
  </div>
</div>



<!-- Button -->
<div class="form-group col-md-4">
    <button id="send-button" name="send-button" class="btn btn-primary" type="submit">Donate!</button>
</div>

<!-- Formspree hidden fields -->
<input type="hidden" name="_next" value="/repo/contribute/thanks.html" />
<input type="hidden" name="_subject" value="New submission from tera-PROMISE donation form" />
<input type="text" name="_gotcha" style="display:none" />







</fieldset>
</form>

