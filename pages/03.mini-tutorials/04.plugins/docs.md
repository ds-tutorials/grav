---
title: Plugins
published: false
taxonomy:
    category:
        - docs
---

### Figuring out which plugins a theme supports

! This section involves interacting with the file system and looking at code. You will not have to interact directly with the code.

Good documentation is often the sign of code. However, you may find yourself in love with a theme that does not have very thorough documentation. In that case, figuring out which plugins it supports can be difficult. The most cumbersome method would be to install every plugin and see if it changes your website. A perhaps more thorough (and certainly less cumbersome) method would be looking through the various templates provided by the theme.

1. Open up your file system. If using Reclaim Hosting/OU Create, the File Manager can be found under the Files heading on your dashboard.
2. Go to your Grav install and find `users/themes/your-theme-name/templates`. You will see several files ending in .html.twig and probably at least one folder (which will hold more templates).
3. Open up the first file.
4. Search for `config.plugins`. This statement will generally show up in an if statement like so: `if config.plugins.plugin-name.enabled`, but it may not.
5. Note the names of any plugins that come up the search. These plugins are used by the theme if installed.
6. Repeat steps 4 and 5 for each of the files in the templates folder, and then for the files of each folder in the templates folder.

## Non-theme plugin

Information about understanding how to use:

When examining the Readme of a plugin, most likely the instructions for use will involve Twig/html, markdown, or yaml.

Twig and html (example from SimpleSearch):
```twig

{% extends 'partials/simplesearch_base.html.twig' %}

{% block content %}
    <div class="content-padding">
    <h1 class="search-header">Search Results</h1>
    <h3>Query: "{{ query }}" - Found {{ search_results.count }} {{ 'Item'|pluralize(search_results.count) }}</h3>

    {% for page in search_results %}
        {% include 'partials/simplesearch_item.html.twig' with {'page':page} %}
    {% endfor %}
    </div>
{% endblock %}
```
If you see this, you can ignore it. This is the code used in templating.

Markdown (example from Diagrams):
```md
[sequence]
A->B:Hi C for me !
B-->A:With pleasure
B->C:A says hello
[/sequence]
```
This can be included directly in the pages you write.

Yaml (example from Email):
```yaml
title: Custom form

form:
  name: custom_form
  fields:

    # Any fields you'd like to add to the form:
    # Their values may be referenced in email actions via '{{ form.value.FIELDNAME|e }}'

  process:
    email:
      subject: "[Custom form] {{ form.value.name|e }}"
      body: "{% include 'forms/data.txt.twig' %}"
      from: sender@example.com
      from_name: 'Custom sender name'
      to: recipient@example.com
      to_name: 'Custom recipient name'
      content_type: 'text/plain'
      process_markdown: true
```
This is the format that the frontmatter of each of your pages will be written in. In normal editing mode, the admin panel takes care of the frontmatter for you, but if you need to edit it directly in order to use a specific plugin, you can always switch to expert mode temporarily.

If the plugin has configurable options, those may also be shown using yaml. You can generally ignore those, as the admin panel will provide a user interface to interact with these options when you click on the plugin.