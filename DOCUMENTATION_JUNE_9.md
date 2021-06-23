##### June 9, 2021

## Created a repo

### Learned:

1. Created a repository named _html-css-practice_ and added files.
2. `git add origin <ssh-link>` was the one i did not do. 
3. The branch was set __main__ as default. 
4. `git reset --hard` is a dangerous method of restoring back to the previous commit.

### Key things to remember:

1. An empty directory won't be pushed.
2. Must `git add` files individually as it is the proper way.
3. Keep the repo _well_ organised.

## HTML

### Learned:

#### Structures:

1. There are six headings: **h(1-6)**
2. `<blockquote>` adds an indent to the lines within open and close tags.
3. `<abbr title = "text">(abbreviation)</abbr>` shows the full form when the cursor is hovered over (abbreviation).
4. `<address>`
    `<p>`
    `<a href="mailto:floydianbkes@gmail.com">floydianbkes@gmail.com</a>`
    `</p>`
    `<p>Bode, Bhaktapur.</p>`
    `</address>`

    `<a>` tag does the same work but here the text inside i.e. Bode, Bhaktapur is emphasised.

    `mailto:` is a must when adding an email-reference.
5. `<del>` and `<s>` does the same function of strikethrough and `<ins>` underlines the text.

#### Lists:

1. Ordered lists `<ol>`, unordered list `<ul>`, `<li>` list item that encloses each item in the list.
2. Definition list `<dl>` is used when the list has a term to be explained and the explanation is written after the definition term `<dt>`. `<dd>` contains the definition. 

#### Links:

1. `<a>` tag does the linking. `<a href = "file address or url">` can be read a reference to the link.
2. Use __id__ inside `<a>` to set a name for a certain part. For example: `<p id = "top"></p>` sets the paragraph as top.
3. To link within the file, use the __#__ symbol. Like: `<a href = "#top">Go to top</a>`

#### Images:

1. `<img src = "filename of url>` the `<img>` tag is used to add images to the page and _src_ stands for source - which could be a filename or a url.
2. `<img>` tag has attributes like:
    * _alt_: to display a text when the image is not displayed `<img src = "filename" alt = "text">` 
    * _title_: displays the text when the cursor is hovered over the image
    * _width_ and _height_ does as they mean
3. `<figure>` is helpful for giving `<figcaption>` for a image within the `<figure>` tag. 

#### Tables:

1. A table starts with `<table>` and ends with `</table>`.
2. `<tr>` stands for __table row__ and then follows `<th>` _table heading_ to bold the table element or `<td>` _table data_ just to type normal element. 
3. `<th scope = "row" or "col">` _row_ and _col_ specify whether the heading contains defines the row data or column data. 
4. `<th or td rowspan or colspan>` _rowspan_ and _colspan_ merges the rows or columns.
5. For empty cell type `<td></td> or <th></th>`.
6. `<thead><tbody><tfoot>` is used for giving different properties to the top, body and bottom part of the table elements. 

