# Haskell Package ReadTheDocs Template

This repo contains a template for writing Haskell package introductions and
tutorials using ReadTheDocs.

## Dowloading and using the template

Clone the repository somewhere outside of your repo:
```
git clone --recurse-submodules https://github.com/m-renaud/haskell-rtd-template.git
```

Copy the `docs` directory into your repo:
```
cp -r haskell-rtd-template/docs /path/to/your/package/
```

Add submodules:
```
echo haskell-rtd-template/.gitmodules >> /path/to/your/package/.gitmodules
```

Build the skeleton:
```
cd /path/to/your/package/docs/
make html
```

And you're done!
