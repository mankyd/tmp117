# tmp117
Python Module for Interacting with Sparfun's TMP117 Module.

This is very much a WIP at the moment, but the basic functionality is there.

Example:

```
from tmp117 import Tmp117

t = Tmp117()

print("Initing")
t.init()

t.oneShotMode()
print("Temp in celsius:", t.readTempC())

config = t.getConfigurationRegister()
print("Config bits: {:016b}".format(config))
```