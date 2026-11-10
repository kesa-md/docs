---
layout: page
title: Kesa extensions
---

Documentation and privacy policies for Kesa browser extensions.

{% for ext in site.extensions %}
## [{{ ext.name }}]({{ ext.path | relative_url }})

{{ ext.summary }}

[Documentation]({{ ext.path | relative_url }}) · [Privacy policy]({{ ext.path | append: 'privacy/' | relative_url }})
{% endfor %}

## Questions

Open an issue in the [kesa-md/docs](https://github.com/kesa-md/docs/issues) repository.
