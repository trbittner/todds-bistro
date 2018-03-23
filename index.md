---
---

{% include header.html %}
  <div class="paper">
    <div class="lines">
    <div class="cookbook-title">
      Todd's Bistro
    </div>
      <div class="text">
      <div class="section-title">Mains</div>
        {% assign recipes = site.recipes | where:'category','mains' %}
        {% for recipe in recipes %}
        <a class="block-link" href="{{ site.baseurl }}{{ recipe.url }}">{{ recipe.recipe-title }}</a>
        {% endfor %}
        <div class="section-title">Pasta</div>
        {% assign recipes = site.recipes | where:'category','pasta' %}
        {% for recipe in recipes %}
        <a class="block-link" href="{{ site.baseurl }}{{ recipe.url }}">{{ recipe.recipe-title }}</a>
        {% endfor %}
        <div class="section-title">Pizza</div>
        {% assign recipes = site.recipes | where:'category','pizza' %}
        {% for recipe in recipes %}
        <a class="block-link" href="{{ site.baseurl }}{{ recipe.url }}">{{ recipe.recipe-title }}</a>
        {% endfor %}
      </div>      
    </div>
    <div class="holes hole-top"></div>
    <div class="holes hole-middle"></div>
    <div class="holes hole-bottom"></div>    
  </div>
{% include footer.html %}
