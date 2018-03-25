---
layout: default
---
  <div class="paper">
    <div class="lines">
    <div class="cookbook-title">
      Todd's Bistro
    </div>
      <div class="text">
      {% assign recipe_groups = site.recipes | group_by: 'category' | sort: 'name' %}
      {% for recipe_group in recipe_groups %}
      <div class="section-title">{{ recipe_group.name | capitalize }}</div>
        {% assign recipes = recipe_group.items | sort: 'recipe-title' %}
        {% for recipe in recipes %}
        <a class="block-link" href="{{ site.baseurl }}{{ recipe.url }}">{{ recipe.recipe-title }}</a>
        {% endfor %}
      {% endfor %}  
      </div>      
    </div>
    <div class="holes hole-top"></div>
    <div class="holes hole-middle"></div>
    <div class="holes hole-bottom"></div>    
  </div>
