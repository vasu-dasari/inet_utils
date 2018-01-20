inet_utils
=====

A collection utility functions that could be used in conjunction with inet to make software more modular.
 
Build
-----
    $ rebar3 compile

Testing
-----

    $ rebar3 eunit

API
---

|API|Description|
|-----:|:-----------|
|convert_mac/2|Convert MAC Address from -> to |
|convert_ip/2|Convert IP Address from -> to |

Conversions allowed are in between following types:
to_string | to_binstring | to_integer | to_binary | to_list | to_tuple

    1> inet_utils:convert_mac(to_binstring, <<1,2,3,4,5,6>>).
    <<"01:02:03:04:05:06">>
    2> inet_utils:convert_ip(to_binary, 16#01020304).
    <<1,2,3,4>>
    
TODO
---
Will keep updating this library with more APIs as needed