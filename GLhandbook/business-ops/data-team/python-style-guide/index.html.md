---
layout: handbook-page-toc
title: "Python Style Guide"
description: "GitLab Data Team Handbook"
---

## On this page
{:.no_toc .hidden-md .hidden-lg}

- TOC
{:toc .toc-list-icons .hidden-md .hidden-lg}

----

## Python Style Guide 

**It is *our collective responsibility* to enforce this Style Guide since our chosen linter does not catch everything.**

#### Linting

We use [Black](https://github.com/ambv/black) as our linter. We use the default configuration.

There is a manual CI job in the `review` stage that will lint the entire repo and return a non-zero exit code if files need to be formatted. It is up to both the MR author and the reviewer to make sure that this job passes before the MR is merged. To lint the entire repo, just execute `black .` from the top of the repo.
 
##### Spacing

Following [PEP8](https://www.python.org/dev/peps/pep-0008/#blank-lines) we recommend you put blank lines around logical sections of code. When starting a `for` loop or `if/else` block, add a new line above the section to give the code some breathing room. Newlines are cheap - [brain time is expensive](https://blog.getdbt.com/write-better-sql-a-defense-of-group-by-1/). 

#### Type Hints

All function signatures should contain type hints, including for the return type, even if it is `None`. This is good documentation and can also be used with [mypy](http://mypy-lang.org/) for type checking and error checking.

Examples:
```python
def foo(x: int, y: int) -> int:
    """
    Add two numbers together and return.
    """

    return x + y

def bar(some_str: str) -> None:
    """
    Print a string.
    """
    print(some_str)
    return
```

#### Import Order

Imports should follow the [PEP8](https://www.python.org/dev/peps/pep-0008/#imports) rules and furthermore should be ordered with any `import ...` statements coming before `from .... import ...`

Example:
```python
import logging
import sys
from os import environ

import pandas as pd
from requests import get

import some_local_module
from another_local_module import something
```

#### Docstrings

Docstrings should be used in every single function. Since we are using type hints in the function signature there is no requirement to describe each parameter. 
Docstrings should use triple double-quotes and use complete sentences with punctuation.

Examples:
```python
def foo(x: int, y: int) -> int:
    """
    Add two numbers together and return the result.
    """

    return x + y

def bar(some_str: str) -> None:
    """
    Print a string.
    
    This is another proper sentence.
    """
    print(some_str)
    return
```

#### How to integrate Environment Variables

To make functions as reusable as possible, it is highly discouraged (unless there is a *very* good reason) from using environment variables directly in functions (there is an example of this below).
Instead, the best practice is to either pass in the variable you want to use specifically or pass all of the environment variables in as a dictionary.
This allows you to pass in any dictionary and have it be compatible while also not requiring the variables to being defined at the environment level.

Examples:
```python
import os
from typing import Dict

## Don't do this!
def foo(x: int) -> int:
    """
    Add two numbers together and return.
    """
    
    return x + os.environ["y"]
foo(1)

## Do this!
env_vars = os.environ.copy() # The copy method returns a normal dict of the env vars.
def bar(some_str: str, another_string: str) -> None:
    """
    Print two strings concatenated together.
    """
    print(some_str + another_string)
    return
bar("foo", env_vars["bar"])

## Or do this!
def bar(some_str: str, env_vars: Dict[str, str]) -> None:
    """
    Print two strings concatenated together.
    """
    print(some_str + env_vars["another_string"])
    return
bar("foo", env_vars)

```

#### Package Aliases

We use a few standard aliases for common third-party packages. They are as follows:
- `import pandas as pd`
- `import numpy as np`

#### Variable Naming Conventions

When possible, use descriptive naming for variables, especially with regards to data type. Here are some examples:

- `data_df` is a dataframe
- `params_dict` is a dictionary
- `retries_int` is an int
- `bash_command_str` is a string

Although usually in the case of constants (particularly strings and numbers) it isn't as helpful, adding the type to the name is good self-documenting code.

#### Making your script executable

If your script is not able to be run even though you've just made it, it most likely needs to be executable. Run the following:

```bash
chmod 755 yourscript.py
```

For an explanation of chmod 755 read this [askubuntu page](https://askubuntu.com/questions/932713/what-is-the-difference-between-chmod-x-and-chmod-755).

#### When not to use Python

Since this style guide is for the entire data team, it is important to remember that there is a time and place for using Python and it is usually outside of the data modeling phase.
Stick to SQL for data manipulation tasks where possible.
 
