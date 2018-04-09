---
layout: main
stylesheet: frontpage.css
title: Todd's Bistro
---
<div class="text">
  {% assign recipe_groups = site.recipes | group_by: 'category' | sort: 'name' %}
    {% for recipe_group in recipe_groups %}
      <div class="section-title">{{ recipe_group.name | capitalize }}</div>
      {% assign recipes = recipe_group.items | sort: 'recipe-title' %}
        {% for recipe in recipes %}
          <div>
            <a href="{{ site.baseurl }}{{ recipe.url }}">{{ recipe.recipe-title }}</a>
          </div>
        {% endfor %}
    {% endfor %}   
</div>
