##### June 10, 2021

### Learned:

#### Forms:

1. The contents of a form is within `<form></form>`. It has different attributes:
    * _action_: It points to where the data and values go to.
    * _get_: With the get method, the values from the form are added to the end of the URL specified in the action attribute.
    * _post_:With the post method the values are sent in what are known as HTTP headers.
2. `<input>` tag is used for many input options available in HTML. It has many useful attributes like:
    1. _type_: this specifies the many types of input option. Some are listed as:
        * _text_: for creating a simple textbox. It further has it's own attributes like _name_, _size_ and _maxlength_.
        Example: `<input type = "text" name = "username" size = "15" maxlength = "30" />`
        * _password_: for a textbox that inputs passwords. It further has it's own attributes like _name_(must be set __password__), _size_ and _maxlength_.
        Example: `<input type = "password" name = "password" size = "15" maxlength = "30" />`
        * _textarea_: creates a comment section. It further has it's own attributes like _name_(must be set __comments__). _rows_ and _cols_ specify the size.
        Example:
        `<textarea name = "comments" cols = "20" rows = "4">Enter your comments...</textarea>`
        * _radio_: for radio button. The further attributes are listed as:
            * _name_: What the value represents as a whole.
            * _value_: The actual value.
            * _checked_: set it __checked__ for preselecting an radio button
        Example:
        `<input type = "radio" name = "social media" value = "Twitter" checked = "checked" /> Twitter `
        * _checkbox_: for checkbox.
            * _name_: What the value represents as a whole.
            * _value_: The actual value.
        Example:
        `<input type = "checkbox" name = "nationality" value = "American">American<br>`
3. `<select>` is used to making drop-down list box. Each option is encompassed by `<option></option>`. The attributes are:
    * _name_: What the value represents as a whole.
    * _multiple_: If you want to show multiple options.
    * _size_: Used after _multiple_ to mention the number of options to show.
    * `<option>` is a tag used within `<select>`. It's attributes are:
    * _value_: The actual value.
    * _selected_: Must be set __selected__ if an option is made to be preselected.
    Example:
    `<select name = "Genre" multiple = "multiple" size = "3">`
        `<option value = "Jazz" selected = "selected">Jazz</option>`
        `<option value = "Rock">Rock</option>`
        `<option value = "Indie">Indie</option>`
        `<option value = "Sufi" selected = "selected">Sufi</option>`
    `</select>`
4. To make subrcibe with an email form:
    `<input type = "text" name = "email">`
    `<input type = "submit" name = "Subcribe" value = "Subcribe">`
The _name_ attribute must be set to _email_ as it will list all the emails when clicked on.
_submit_ makes a button creates a submit button whose _name_ and _value_ should be set _Subsribe_. 
5. Uploading a file can be done with:
    `<input type = "file" name = "file"><br>`
    `<input type = "submit" value="upload">`
__But first the form method must be set as Post__
6. To use image as input:
    `<input type = "image" src = "source" width = "" height = "">`
7. To use image as button:
    `<button><img src="images/Pencil-Drawings-Combined-With-Photographs-9.jpg" alt="add" width="10" height="10" /> Add</button>`
8. `<label>` simply provides label. 
9. `<fieldset>` encapsulates a form. `<legend>` within `<fieldset>` gives the caption or heading to the fieldset.
10. For form validation:
    `<form action = "https://twitter.com" method="post">`
        `<label for = "username">Username:</label>`
        `<input type = "text" required = "required"><br>`
        `<label for = "password">Password:</label>`
        `<input type = "password" required = "required">`
        `<input type = "submit" value = "Submit">`
    `</form>`
    * _required_: is to be set __required__ when the input is necessary.
11. To input date we do:
    ` <input type="date" name = "">` This creates a textbox with the date option.
12. To input url w do:
    `<input type = "url" name = "website">` This also creats a textbox but this one takes url input.
13. A searchbox is created with:
    `<input type = "search" name = "search">`

#### Extra Markup

1. _id_ attribute(CSS)
2. _class_ attribute(CSS)
3. `<div>` is used in grouping of many elements in a single entity. 
4. `<span class = ""></span>` (CSS)
5. `<iframe>` is used to insert a snippet of a webpage within a frame. Mainly used for inserting googlemaps.
    Example:
    `<iframe`
        `width="450"`
        `height="350"`
        `src="http://maps.google.co.uk/maps?q=moma+new+york`
        `&amp;output=embed">`
        `</iframe>`
6. `<meta>` elements are inside the `<head>` elements that gives the browser information about the page like: who created it, when it expires, etc.
    Example:
    `<head>`
        `<meta name="description" content="An Essay on Installation Art" />`
	    `<meta name="keywords" content="installation, art, opinion" />`
	    `<meta name="robots" content="nofollow" />`
	    `<meta http-equiv="author" content="Jon Duckett" />`
        `<meta http-equiv="pragma" content="no-cache" />`
        `<meta http-equiv="expires" content="Fri, 04 Apr 2014 23:59:59 GMT" />`
    `</head>`
7. [DOCTYPE, remark in HTML and Escape Characters](https://github.com/bkzzshzz/html-css-practice/blob/main/html/extra_html_info.md)




