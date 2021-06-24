###### June 24

#### Learned

### Git
1. `git branch` lists the branches
2. `git branch <branch_name>` creates a new branch.
3. `git checkout <branch_name>` switches to the branch
4. `git pull origin master -f` pulls the updates from the remote repo to local repo
5. `find <filename> or <folder>` checks whether a file or a folder is inside a directory

### Python

1. To avoid getting errors when using double quotes inside a string, __use triple quotes ''' '''__ 
2. There is a grave difference between 
```python
variable = open("filename","mode")
``` 
and 
```python
variable = open("filename", "mode").read()
```
Without the _read()_ function appended, the variable stores the position of the file(**Not the file**). With _read()_, the variable stores the file as an string to variable. 
3. The following line is to be embedded into the {variable} part in html file. It has to be repeated the number of times the number of files are in the folder. The _list_of_links_ will concatenate all the link lines in a single string. The `file_title` will act as a variable for the title of the file.
```python
link_for_single_file = '''
            <li><a href="blog-posts/{file_name}">{file_title}</a></li>
            '''
list_of_links = '''
'''
```
4. In the for loop below, for every file in the list of files, the program will take one file name at a time and open the file. The content of file are converted to string with `file_content_str = file_handle.read()`. (The two lines can be written in a single line as `file_content_str = open("./blog-posts/" + name_of_file).read()`).

5. The logic to finding the title of the html file is to extract the text between `<title></title>`. To do that, search for <title> and </title> in the string. `.find("text")` finds the position of the place just before <title>. The starting postion is the postion at which <title> is found added to the number of characters in <title>. The ending postion is the postion of </title>. `title_from_file = file_content_str[starting_pos:ending_pos]` This stores the title of the file to the string title_from_file. `list_of_links = list_of_links + link_for_single_file.format(file_name = name_of_file, file_title = title_from_file)` is self explanatory. 
```python
for name_of_file in file_list:
    file_handle = open("./blog-posts/" + name_of_file)
    file_content_str = file_handle.read()
    temp_file = file_content_str
    temp_file = temp_file.lower()
    starting_pos = temp_file.find('<title>') + len('<title>')
    ending_pos = temp_file.find('</title>')
    title_from_file = file_content_str[starting_pos:ending_pos]
    list_of_links = list_of_links + link_for_single_file.format(file_name = name_of_file, file_title = title_from_file)
```

### Key takeways

The idea to solving the problem(or any future problems) is to take it step by step.

