
CnOpts - A connection options object, used for passing extended options to the Connection

```python
from pysftp import CnOpts, Connection
connection_opts = CnOpts()
connection_opts.hostkeys = None
conn = Connection(
        host="<hostname>",
        username="<user>",
        password="",
        #private_key=private_key_object,
        cnopts=connection_opts,
    )
```