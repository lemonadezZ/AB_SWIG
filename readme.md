```
/root/swig-3.0.12/swig -python example.i
```
```
yum install python-devel
```

```
gcc -fPIC -c example.c example_wrap.c -I/usr/include/python2.7/
```

```
ld -shared example.o example_wrap.o -o _example.so
```
