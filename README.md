# ODP-EL-textX

**Note:** The work on this project is continued at https://github.com/computable-governance/ODP-EL-textX

This is a an implementation of the subset of ODP-EL in textX.
 
This project is in an initial stage of development.

# How to setup

``` sh
python -m venv venv
source venv/bin/activate
pip install textx[dev]
pip install -e .
```

To verify that everything is ok you can list all textx languages in the environment:

``` sh
textx list-languages
```

and see ODP-EL language in the list:

```
odpel (*.odpl)                ODP-EL-textX[0.1.0.dev0]                odpel language
```

You can generated meta-model diagrams by:

``` sh
cd odpel
make
```

Note: you must have [plantuml](https://plantuml.com/) installed and available on
your PATH.


Now, test that provided example is parsed correctly:

``` sh
textx check examples/consent.odpl
```



# Credits

Initial project layout generated with `textx startproject`.
