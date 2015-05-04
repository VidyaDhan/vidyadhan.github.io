---
layout: default
title: Vidya Dhan
full_posts: 1
---
<div class="homepage">
<div class="row voffset">

  <div class="col-md-9">

<p>Vidya Dhan (the name means “gift of education”) is a small charity set up by family and friends, it has been in operation for three years. </p>

<p>Following a recent increase in income it was decided to register it as a company limited by guarantee, open a bank account and register with HMRC in order to reclaim tax on gift aid. Vidya Dhan's main area of operation is in India where it helps children, especially but not exclusively, girls from poor families. </p>

<p>Its main objectives are:- </p>

<ol>
  <li>Contribute fully or in part towards the school fees of children</li>
  <li>Contribute fully or in part towards costs of school uniforms, shoes and stationery</li>
  <li>Reimburse children's medical costs if parents are unable to afford such costs</li>
  <li>Counsel parents in order to provide a safe and nurturing home environment</li>
  <li>Provide after school tuition and help with homework where necessary Vidya Dhan has been fortunate to recruit two voluntary outreach workers in India who select children in need. </li>
</ol>

  </div>

  <div class="col-md-3">
    <img src="/images/thyagraj/Thyagraj_1-640.jpg" width="270" class="popup" />
    <img src="/images/thyagraj/Thyagraj_2-640.jpg" width="270" class="popup" />
  </div>

</div>

<div class="row voffset">

  <div class="col-md-4">
    <img src="/images/thyagraj/Thyagraj_3-640.jpg" width="270" class="popup" />
    <img src="/images/thyagraj/Thyagraj_4-640.jpg" width="270" class="popup" />
  </div>

  <div class="col-md-8">

<p>At present the charity operates in and around rural areas of Bangalore. If our income increases we hope to be able to widen our area of operation. As the presence of Vidya Dhan has become known the local villagers approach our outreach workers in order to obtain funding for their children's education. In addition the outreach workers visit local villages to seek out children from particularly poor families. </p>

<p>No preference is given to children on basis of religion or caste. Once children are enrolled into our programme we monitor their progress at school and provide them and their parents with assistance as required. </p>

<p>Children have benefitted greatly from our programme. These children would not have been able to afford even basic state education whereas they are now being educated in good English medium schools. For the 20014/15 academic year there were 12 children in our programme. </p>


  </div>

</div><!-- /row -->

<div class="row">
  <div class="col-md-12">

<p>Attached are brief details, further information can be provided. The selection process is underway for 2015/16 and we hope to sponsor the education of at least 15 children, mostly girls.</p>
  
  </div>
</div><!-- /row -->


{% for post in site.posts %}
{% if forloop.index <= page.full_posts %}
<div class='post'>
  <h2><a href='{{post.url}}'>{{post.title}}</a></h2>
  <p><span class='date'>{{post.date | date_to_string}}</span></p>
  <div class='body'>{{post.excerpt}}</div>
</div>
{% endif %}
{% endfor %}

<div class="postLinks">
  <h3>Older Posts</h3>
  <ul>
  {% for post in site.posts %}
  {% if forloop.index > page.full_posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endif %}
  {% endfor %}
  </ul>
</div>

</div>