# Restructuring some things

"pictures" should be renamed to "posts" to reflect a more generic data structure. Below is a plan for a general file strucutre.

NOTE: I should also write notes and commments on what each of these `.js` files do.

```
- public
+-- js
  +-- components
    +-- addbox.js
    +-- editable-text.js
    +-- image-data.js
    +-- pagebox.js
    +-- searchbox.js
    +-- sidebar-tags.js
    +-- thumbnail.js
  +-- index.js
  +-- search.js
  +-- upload.js
  +-- view.js
+-- lib
  +-- vue-router.js
  +-- vue.vs
  +-- vue.min.js
  +-- vue2-autocomplete.js
+-- css
  +-- style.css
  +-- theme.css
  +-- vue2-autocomplete.css
+-- database
  +-- posts.json
  +-- tags.json
+-- posts
  +-- img
  +-- gif
  +-- video
  +-- audio
  +-- markdown
+-- index.html
```


# posts.JSON structure
Refer to `posts.ods` for a spreadsheet view of how the posts.json file should be organized.

```json

```