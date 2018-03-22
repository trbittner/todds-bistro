---
---

{% include header.html %}
  <div class="paper">
    <div class="lines">
    <div class="cookbook-title">
      Todd's Bistro
    </div>
      <div class="text">
        <div class="section-title">
          Pasta
        </div>
        {% for recipe in site.recipes %}
        <a class="block-link" href="{{ site.baseurl }}{{ recipe.url }}">{{ recipe.recipe-title }}</a>
        {% endfor %}
      </div>      
    </div>
    <div class="holes hole-top"></div>
    <div class="holes hole-middle"></div>
    <div class="holes hole-bottom"></div>    
  </div>
{% include footer.html %}
