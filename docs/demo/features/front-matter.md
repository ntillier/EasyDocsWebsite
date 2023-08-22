---
slug: 'front-demo'
label: 'File config'
index: 2
---

# File config

This file demonstrate the config possibilities available in the front matter of the files.

The file name is `front-matter.md`, but the front-matter can overhidde the doc slug and label:
```yaml
slug: 'front-demo'
label: 'File config'
```

So the label of this file is becomes `File config`, and its slug `front-demo`.

!!! info Note on the front matter
EasyDocs uses [gray-matter](https://www.npmjs.com/package/gray-matter) to parse the [YAML](https://yaml.org/) front matters of the files.
Thus the front matter should be in the YAML format and wrapped between two `---`, as below:
```
\-\-\-
hello: 'Hello world!'
\-\-\-
```
!!!