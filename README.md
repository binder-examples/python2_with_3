# Mixing Python 2 and 3 kernels with `runtime.txt`

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/binder-examples/python2_with_3/master)

Sometimes you want *both* Python 2 and Python 3 (e.g., if you have a mixture of notebooks that use each
version of the language). This repository demonstrates how to handle these cases with `repo2docker`. You can
specify a Python 2.7 environment with the `runtime.txt` file. In this case, `repo2docker` will install Python 2
*alongside* Python 3 (though all commands will default to Python 2). In this case, you can install Python 3 dependencies
with `requirements3.txt`, while a file called `requirements.txt` alone will install to the Python 2 environment.