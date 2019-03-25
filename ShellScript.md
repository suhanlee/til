# ShellScript


#### expr
```
$ NUMBER=5
$ expr $NUMBER * 5
10
```

#### Return code
- Retrun value 0 is success, otehr is fail
```
$ echo "Hello"
Hello
$ echo $?
0
```
#### test
```
$ test 5 -lt 3
$ echo $?
1
```

#### test []
```
$ [ 5 -lt 3 ]
$ echo $?
1
```

#### if
```
#!/bin/sh

if [ `whoami` = "root" ] 
then
  echo "super user"
fi
```
