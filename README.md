# mermaid component
This is an example on how you can create a component in [CradleCMS](https://cradlecms.com) that loads a library.
The mermaid library is large, about `~900KB`, so it's only loaded when content has been tagged with `mermaid`.

### Example
 ```mermaid
 pie title NETFLIX
         "Time spent looking for movie" : 90
         "Time spent watching it" : 10
```

Link to [more mermaid examples](https://mermaid.ai/open-source/syntax/examples.html)


## How to
Add the `mermaid.liquid` file into your theme `components` folder.

Enter `{% component 'mermaid' %}` in your theme layout, after the `</body>` tag.

To create a mermaid diagram you need to use the markdown `MD` editor.

Create a new `page` or blog `article` using `MD`.


Set `mermaid` tag on the `page` or `article` and the mermaid library gets loaded.

### Override CSS
If your theme contains special styling for `<pre>` or `<code>` you might need to reset css stylings.
Below is an example how you can set `background-color: transparent` on the `pre` block containing the `mermaid` diagram.
```
pre:has(.language-mermaid) {
    background-color: transparent;
}
```

