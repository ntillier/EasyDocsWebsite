---
label: 'Configuration'
slug: 'configuration'
---

# Configuration
Tailoring the global attributes of your documentation is achievable through the docs.config.json file.

```json
{
  "title": "Your Documentation Title",
  "favicon": "/favicon.ico",
  "header": {
    "title": "Your Documentation Title",
    "icon": "/icon.svg",
    "links": [
      {
        "label": "Custom Label",
        "link": "https://example.com"
      }
    ]
  }
}
```

**Here's what each component represents:**

* `title`: This sets the title displayed in the browser's tab.
* `favicon`: Refers to the icon visible in the browser's tab.
* `header`: Contains information pertaining to the page header.

**In the header section, you can further customize:**
* `title`: The title showcased in the header.
* `icon`: An icon associated with the header.
* `links`: An array of links, each with a label (text) and corresponding link (URL).

!!! success Congratulation
Congratulations on successfully creating and setting up your project! Enjoy a virtual 🍪 :)
!!!