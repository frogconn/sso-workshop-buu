Configuring the authentication source

```
touch modules/exampleauth/enable
```

Configuration on authsources.php
```
'example-userpass' => array(
        'exampleauth:UserPass',
        'student:studentpass' => array(
            'uid' => array('student'),
        ),
        'employee:employeepass' => array(
            'uid' => array('employee'),
        ),
    ),
```