Easily find out what version of python pipx is running. I could not find a
better package that already does this.

## usage

``` bash
# what version of python does the global pipx use?
pipx run --spec git+https://github.com/waylonwalker/pyvers pyvers

# what version of python does the local pipx use?
python -m pipx run --spec git+https://github.com/waylonwalker/pyvers pyvers
```

## alternative

I later realized that I can achieve the same solution without creating a new
package, but installing ipython or another repl that allows me to pass in a
python string.

```
pipx run ipython -c "import sys;print(sys.version)"
```
