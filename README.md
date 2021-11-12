# Python Packaging Tutorial

### Notes

[Tutorial URL](https://packaging.python.org/tutorials/packaging-projects/)
[License Picker](https://choosealicense.com/)

### Configuring metadata
There are two types of metadata: static and dynamic.

Static metadata (setup.cfg): guaranteed to be the same every time. This is simpler, easier to read, and avoids many common errors, like encoding errors.

Dynamic metadata (setup.py): possibly non-deterministic. Any items that are dynamic or determined at install-time, as well as extension modules or extensions to setuptools, need to go into setup.py.

Static metadata (setup.cfg) should be preferred. Dynamic metadata (setup.py) should be used only as an escape hatch when absolutely necessary. setup.py used to be required, but can be omitted with newer versions of setuptools and pip.