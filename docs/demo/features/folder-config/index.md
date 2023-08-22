# Folder config

EasyDocs lets you easily edit your directories' slug and label and order, in your files as in your directories. To edit the slug/label/order of a directory, you just need to create a JSON config file in it, like below.

```json
{
  "slug": "folder-demo",
  "label": "Folder config",
  "index": 1
}
```

!!! info Info
This is the config file of the current directory!
!!!

You can edit three options:

## slug
The slug is the URL-friendly version of the directory's label. This option allows you to edit it.

## label
By adding this option, you change the name the users will see in the navigation bar.

## index
The index let you change the order of the directory inside its parent. If the index is greater than the index of the index of the other directories, it will be placed after them in the navigation bar. On the opposite, if the index is smaller than the index of the other directories is will be placed before them.

# Index file
If you name a file `index.md`, the user will view it when he will navigate to the directory, instead of the list of all the directory childrens.

!!! info Info
And this is why you are currently viewing this file :)
!!!