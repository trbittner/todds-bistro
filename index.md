---
layout: default
stylesheet: paper.css
---
<div class="row">
  <div class="col-md-1"></div>
  <div class="paper col-12 col-md-10">
    <!-- It appears that because the "lines" class isn't a row, it breaks the bootstrap flow and the associated
         padding.  As a result, we have to re-declare the "container" class. -->
    <div class="lines container">
      <div class="row">
        <div class="col-md-1"></div>
        <div class="col-6 col-md-5">
          <div class="cookbook-title">Todd's Bistro</div>
        </div>
        <div class="col-6 col-md-5">
        <div class="backpage-title float-right"><a class="backpage-link" href="#">Cooking Tips</a></div>
        </div>
        <div class="col-md-1"></div>
      </div>
      
      <div class="row">
        <div class="col-md-1"></div>
        <div class="col-12 col-md-11">
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
      </div>
    </div>
    <div class="holes hole-top"></div>
    <div class="holes hole-middle"></div>
    <div class="holes hole-bottom"></div>    
  </div>
  <div class="col-md-1"></div>
</div>
