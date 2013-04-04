lulip
=====

Line-level profiler for code running in LuaJIT

Usage
-----

```Lua
local profiler = require 'lulip'
local p = profiler:new()
p:dont('some-module')
p:maxrows(25)
p:start()

-- execute code here

p:stop()
p:dump(output_file_name)
```
