---
label: 'Project Organization'
slug: 'organization'
---

# Organizing your project
EasyDocs leverages markdown files within the `/docs` directory to generate your website. This guide offers a comprehensive overview of how you can efficiently structure your documentation.

# Documentation Structure
The directory layout of EasyDocs has been meticulously crafted to ensure your content remains orderly and easily manageable. Here's a breakdown:

```lua
EasyDocs/
|-- docs/
|   |-- index.md
|   |-- about.md
|   |-- guide/
|       |-- guide-first-part.md
|       |-- guide-second-part.md
|-- public/
|   |-- logo.png
|   |-- background.jpg
|-- .static/
|   |-- tree.json
|-- .build/
|   |-- index.html
|   |-- index.min.js
|-- docs.config.json
```

## `/docs` Directory
The `/docs` directory serves as the repository for your markdown document files. Each markdown file signifies a distinct webpage. For instance:

* `/index.md`: Your main landing page.
* `/about.md`: The About Us page.
* `/guide`: A subdirectory housing individual markdown files for a guide.

!!! info File Extensions
EasyDocs will exclusively process files in `/docs` ending with `.md`. Other files will be omitted, with exceptions for special files.
!!!

## `/public` Directory
The `/public` directory is designed for storing images and other files utilized in your website. By separating images from content, you maintain an organized structure.

## Configuration
The docs.config.json file contains crucial configuration settings for your website. We'll delve into this in later sections.

# Advanced Usage
EasyDocs introduces advanced functionalities for customizing your documentation.

## Front Matter
You can incorporate front matter at the outset of a file. This entails data stored in YAML format, encapsulated by `---` at the file's commencement.

Three options are available:

* `label`: Document name.
* `slug`: URL-friendly version of directory label.
* `index`: File's position within its directory.

!!! info Index Handling
The index grants you control over directory order within its parent. A higher index places the directory after others in the navigation bar, while a lower index precedes them.
!!!

## Configuration Files
EasyDocs simplifies slug, label, and order customization for directories, both in files and within directories. To modify a directory's slug, label, or index, create a JSON config file named config.json within the directory, as demonstrated below:

```json
{
  "slug": "folder-demo",
  "label": "Folder Configuration",
  "index": 1
}
```

!!! hint Efficient Editing
These three options parallel the functions of the [front matter](#front-matter) attributes.
!!!