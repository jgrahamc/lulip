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
p:accumulate_in(accumulate_file_name)
p:dump(output_file_name)
```
