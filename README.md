# Leetcode-userapi
get info on leetcode profiles via graphql python

requires python3 requests


example code: 

```python

from leetmodel import *

username = ...
password = ....
model = leetmodel(username, password)


userData = model.getUserData(rr)
user = userData["username"]
realname = userData["profile"]["realName"]

if realname != "":
  print("hello %s(%s)!"%(realname, user))
else:
  print("hello %s!"%(user))
```
