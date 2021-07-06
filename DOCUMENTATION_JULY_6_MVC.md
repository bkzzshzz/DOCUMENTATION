##### July 6

#### About User Management System and MVC

Any site/blog may require a User Management System to engage with the subscribers/users, to keep track of their number, information and activites within the site. The need for this type of interaction between the users and the server hence justifies the user management system. It is based in MVC(Model-View-Controller) structure. Irrespective of the structure, there is always a _client_ that seeks/saves information, a _database_ that stores the information and a _server_ that acts as a middleman between client and database. For better understanding and genralising, this interaction between these three parties is called MVC where

Model --> Database

View --> HTML/CSS pages that client sees

Controller --> Server

1. **Model**: It is simply the database where the information is stored and is retrieved from when need be by the controller. MySQL, MongoDB are the languages for creating models. The main thing to note is that it __only interacts with the controller__. 

2. **View**: It is a fancy way of saying HTML pages and is what the client sees. WE can say that it is the output of the combined work of controller and model. It also __only interacts with the controller__. 

3. **Controller**: This is the part which interacts with the user. Just like a waiter takes orders and serves, this takes instructions/information from the user and gives the desired processed information back. It is the middleman between view and model. 

```
Point to note:
There should be no interaction between view and model. All the interaction between them must be done through the controller, 
```

#### Plans for Login/Signup

1. [This](https://colorlib.com/wp/template/colorlib-regform-7/) bootstrap supported template is the one that shall be used for login and signup page. 

2. The login/signup button will be on the right side of the navbar before More.... 

3. The login/signup pages are stored in a separate folder called views. 

4. The functionalities of the pages will include whatever is present in the template. 

4. GET /login and /signup will reference to the login and signup pages resp.

#### About CSV

1. CSV stands for comma separated values. It is mainly used for storing data and is easily accessible.

Python has a csv library that eases accessing CSV files.

```python
import csv

with open('employee_birthday.txt') as csv_file:
    csv_reader = csv.reader(csv_file, delimiter=',')
    line_count = 0
    for row in csv_reader:
        if line_count == 0:
            print(f'Column names are {", ".join(row)}')
            line_count += 1
        else:
            print(f'\t{row[0]} works in the {row[1]} department, and was born in {row[2]}.')
            line_count += 1
    print(f'Processed {line_count} lines.')
```
`csv_reader = csv.reader(csv_file, delimiter=',')` csv_reader stores an address of the csv file's data converted into a list. The `delimited` removes the commas. 

```python
import csv

with open('employee_birthday.txt', mode='r') as csv_file:
    csv_reader = csv.DictReader(csv_file)
    line_count = 0
    for row in csv_reader:
        if line_count == 0:
            print(f'Column names are {", ".join(row)}')
            line_count += 1
        print(f'\t{row["name"]} works in the {row["department"]} department, and was born in {row["birthday month"]}.')
        line_count += 1
    print(f'Processed {line_count} lines.')
```

Here, the `DictReader` converts the csv_file data into a dictionary and the memoery address is passed to csv_reader. 


#### Reference Links

1. [CSV Reference](https://realpython.com/python-csv/)
2. [About MVC](https://www.youtube.com/watch?v=1IsL6g2ixak)

