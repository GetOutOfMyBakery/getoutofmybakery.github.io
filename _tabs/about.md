---
# the default layout is 'page'
icon: fas fa-info-circle
order: 4
---

Hey!

{% if jekyll.environment == 'development' %}
  👇 This is only shown in "development mode":
  > Add Markdown syntax content to file `_tabs/about.md`{: .filepath } and it will show up on this page.
  {: .prompt-tip}

  Let's see some prompt's in action:
  > prompt-tip
  {: .prompt-tip}

  > prompt-info
  {: .prompt-info}

  > prompt-warning
  {: .prompt-warning}

  > prompt-danger
  {: .prompt-danger}
{% endif %}
