Pro PHP Debugger
=========

simple php debugger

usage
=========

 ```php
    fla($target_variable, $second_param);
```

`$second_param` can be a custom string or if `TRUE` it would exit atfer the output is made

 custom output
 
 ```php
    fla('_funcs');		// all user declared and available functions
    fla('_vars');		// all user defined variables
    fla('_trace');   	// backtrace
```

changelog
=========

    v0.1   - Foldable array elements
    v0.2   - Fixed multiline array display bug, array css styling, detect ajax call with $_SERVER['HTTP_X_REQUESTED_WITH'] and display result as json
    v0.3   - added object to array folding system (fixed error)
           - config zone (LIVE_MODE - viewable only for provided DEBUG_IP or localhost)
           - updated css rules
           - if the second parameter is FALSE, then it would die, otherwise it would print the text
           - on/off switch
           - IP filter
    v0.3.1 - fix css rule
           - change LIVE with VIEW_FILTER
           - added USER_AGENT_VAR filter 

todo
=========
    - [x] on/off switch
    - [x] IP filter
    - [ ] memory usage
    - [ ] cpu usage? (w/ exec if available or sys_getloadavg)
    - [ ] highlight_file('file.php')
    - [ ] php_uname (host OS), php_sapi_name (interface between web server and PHP)
    - [ ] PHP_VERSION
    - [ ] dockable option
    - [ ] optimize css include
    - [ ] features array for easy disabling (to increase performance)
    - [ ] array fold indicator

    uncommited changes
     - removed post, get, cookies, files, request, server -> redundant