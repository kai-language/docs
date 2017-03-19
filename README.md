# Kai Lang Documentation
This repository is the home of Kai's language tour. Please feel free to contribute to the project.

## Getting started 🚀

Start by manually-installing [pip](https://pip.readthedocs.io/en/stable/installing/).

Using pip, install and setup [MkDocs](http://www.mkdocs.org). 

> You can use [brew](https://brew.sh) for this, but you may experience issues.
```
pip install mkdocs
```

Now that pip and MkDocs are setup, we need to install our theme, syntax-highlighting engine and MarkDown extensions. Thankfully, pip makes all of this easy.
```
pip install pygments
pip install pymdown-extensions
pip install mkdocs-material
```

That's it! You're ready to develop!

## Local development 🔨
Run the command `mkdocs serve` and open up `http://127.0.0.1:8000/` to view a local copy of the documentation. MkDocs will automatically detect modifications to local files and will refresh the page.

## Building and deploying 🚚
Before you can deploy your changes, you must build the documentation:
```
mkdocs build
```

Now, let's push to GitHub Project Pages:
```
mkdocs gh-deploy
```

And we're done! 🎉
> NOTE: Please make sure to commit your changes to the `master` branch.