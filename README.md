TOML
====

See also https://github.com/mojombo/toml

Python module which parses and emits TOML.

Released under the MIT license.

Current Version of the Specification
------------------------------------

https://github.com/mojombo/toml/blob/e3656ad493400895f4460f1244a25f8f8e31a32a/README.md

TO DO
-----

- Make sure the parser keeps up with the spec as it evolves.

QUICK GUIDE
-----------


```
pip install toml
```


toml.dumps --- takes a string to be parsed as toml and returns the corresponding dictionary

toml.loads --- takes a dictionary and returns a string which is the contents of the corresponding toml file.


There are other functions which I use to dump and load various fragments of toml but dumps and loads will cover most usage.

Example usage:

```
import toml

with open("conf.toml") as conffile:
     config = toml.dumps(conffile.read())
# do stuff with config here
. . .
```
