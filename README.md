#Intro

The database `mongo_esc` is an extremely simple database.

##The Basics:

###Connecting

```
>>> from database_store import DB
>>> db = DB()
>>> db.connect()
```

###Putting Data In && Getting Data Out

```
>>> from database_store import DB
>>> db = DB()
>>> db.connect()
>>> db.change_db("eric")
>>> db.get_data("schles",document={"answer to everything":42})
[{u'answer to everything': 42}]
>>> db.get_data("schles",keys=["answer to everything"])
[{u'answer to everything': 42}]
>>> db.get_data("schles",values=[42])
[{u'answer to everything': 42}]
```




