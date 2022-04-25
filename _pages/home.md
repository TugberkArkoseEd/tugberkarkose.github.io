---
layout: archive
permalink: /
hidden: false
# header:
#   overlay_color: "#5e616c"
#   overlay_image: /assets/images/mm-home-page-feature.jpg
#   actions:
#     - label: "<i class='fas fa-download'></i> Install now"
#       url: "/docs/quick-start-guide/"
# excerpt: >
#   A flexible two-column Jekyll theme. Perfect for building personal sites, blogs, and portfolios.<br />
#   <small><a href="https://github.com/mmistakes/minimal-mistakes/releases/tag/4.24.0">Latest release v4.24.0</a></small>
# feature_row:
#   - image_path: /assets/images/mm-customizable-feature.png
#     alt: "customizable"
#     title: "Super customizable"
#     excerpt: "Everything from the menus, sidebars, comments, and more can be configured or set with YAML Front Matter."
#     url: "/docs/configuration/"
#     btn_class: "btn--primary"
#     btn_label: "Learn more"
#   - image_path: /assets/images/mm-responsive-feature.png
#     alt: "fully responsive"
#     title: "Responsive layouts"
#     excerpt: "Built with HTML5 + CSS3. All layouts are fully responsive with helpers to augment your content."
#     url: "/docs/layouts/"
#     btn_class: "btn--primary"
#     btn_label: "Learn more"
#   - image_path: /assets/images/mm-free-feature.png
#     alt: "100% free"
#     title: "100% free"
#     excerpt: "Free to use however you want under the MIT License. Clone it, fork it, customize it... whatever!"
#     url: "/docs/license/"
#     btn_class: "btn--primary"
#     btn_label: "Learn more"      
---

## About Me
Used to working in multinational and multidisciplinary environments, getting involved in all stages of software development processes. Fast and eager learner with a research background, supportive and reliable team player with strong bias towards software quality and customer satisfaction.
---
### Experience
- Senior Software Innovation Engineer@Aizon - Nov 2020 / Present
- Research Software Engineer@Clevernet - Oct 2018 / Nov 2020
- Research Scientist@Barcelona Supercomputer Centre - Jul 2016 / Oct 2018

### Skills
- Python
- Distributed Systems
- Machine Learning

<h3 class="archive__subtitle">{{ site.data.ui-text[site.locale].recent_posts | default: "Recent Posts" }}</h3>

{% if paginator %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.posts %}
{% endif %}

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in posts %}
    {% include archive-single.html type=entries_layout %}
  {% endfor %}
</div>

{% include paginator.html %}

{% include feature_row %}
