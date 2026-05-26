# mermaid component
This component is an example on how you can create a component that dynamically loads a large library.
The mermaid library is `~900KB` and it's loaded only when content has the tag `mermaid`.

## How to
Add the `mermaid.liquid` file into your theme `components` folder.

Enter `{% component 'mermaid' %}` in your theme layout, after the `</body>` tag.

To create a mermaid diagram you need to use the markdown `MD` editor.

Create a new `page` or blog `article` using `MD`.

### Example
 ```mermaid
 pie title NETFLIX
         "Time spent looking for movie" : 90
         "Time spent watching it" : 10
```

Set `mermaid` tag on the `page` or `article` and the mermaid library gets loaded.
