# Py LevelDB

A Cython wrapper for Mojang's modified LevelDB library.


## Install
`pip install pyleveldb`

## Use
```py
from leveldb import LevelDB

db = LevelDB("path/to/db", create_if_missing = True)
db.put(b"greetings", b"Hello world")
print(db.get(b"greetings"))
# b"Hello world"
```

See the [source code](src/leveldb/_leveldb.pyx) for full documentation.
