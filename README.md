# Sphinx Issue Example 

In Sphinx v4.3.1 and Python 3.8.2, setting a private class's `__module__` to the module name allows it to be documented, but its attributes' docstrings are ignored.

To produce, install Sphinx into your Python environment (e.g., `pip install sphinx`), then:

```sh
cd docs
make html
```

Then view the generated html for the module at: `docs/build/html/testmod.html`.
`ClassPrivate.foo` appears in documentation, but without its docstring.
