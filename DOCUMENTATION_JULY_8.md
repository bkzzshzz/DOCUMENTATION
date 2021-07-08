##### July 8

```
The thing is, breaking down problems into sub-problems. Deal with one at a time and everytime see if one works or not before jumping into another. Today too, it was a lesson. A lesson that goes without saying, one of the most important in my programming journey. One step at time is the best way to get things done. 
```

### Today, the response was okay and all. There were definite problems but, since the response was 200(which means there's no problem in finding the file or not finding the file), it took us a while to figure out what exactly was wrong. Then when we put the proper response if the files that were requested(with extensions like .eot, .tff, .js, etc) using `self.sendresponse(400)`. With this we got the gist of the problem. Then it was all about finding the files and putting them in the root directory. 

#### Learned:
1. __favicon.ico__ icon file should be kept in the root directory. 
```python
valid_extensions = ['.jpg', '.css', '.js', '.eot', '.tff', '.woff', '.woff2', '.ico']

        for extension in valid_extensions:
            if self.path.endswith(extension):
                get_file = True
                break
```
Before this, I compared every extension by using `self.path.endswith() or self.path.endswith(extension) or self.path.endswith(extension)` which is a tedious job. So, instead made a list and by using a for-loop the problem is solved.

