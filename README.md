# buck-linker-flag-issue

Buck should be able to link a precompiled library using `linker_flags`. This project can be used to check different versions of Buck.  

To create `libfoo`:

```bash=
clang++ -c foo.cpp -o foo
ar -rv libfoo.a foo.o
```

To build the app:

```bash=
buck build :app
```
