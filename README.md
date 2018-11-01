# Haskell Package ReadTheDocs Template

This repo contains a template for writing Haskell package introductions and
tutorials using ReadTheDocs.

## Dowloading and using the template

Install [Sphinx](www.sphinx-doc.org) and the [ReadTheDocs
theme](https://github.com/rtfd/sphinx_rtd_theme):
```
pip install sphinx sphinx-autobuild sphinx_rtd_theme
```

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

And you're done! View in your browser by visiting
`file:///path/to/your/package/docs/_build/html/index.html`.

For a full example see the [containers
documentation](https://haskell-containers.readthedocs.io).

## Uploading to ReadTheDocs

1. Create an account at [ReadTheDocs](https://www.readthedocs.org).
2. [Import your
   docs](http://docs.readthedocs.io/en/latest/getting_started.html#import-your-docs)
   and name the project `haskell-<package-name>` (for example, the `containers`
   package would be `haskell-containers`).
3. View your new docs at `haskell-<package-name>.readthedocs.io`!

*Note: We prefix the package name with `haskell-` for consistency across
packages since the bare package name won't be available in many cases. If the
package name has the `haskell-` prefix already then just use the package name.*

## Haskell Specific ReadTheDoc Extension

I've also written a [Haddock Autolink](https://github.com/m-renaud/haddock-autolink) extension which allows you to easily link to Haddocks using simple syntax like:


```
:haddock:`containers`
```
=> [containers](https://hackage.haskell.org/package/containers)

```
:haddock:`containers/Data.Sequence`
```
=> [Data.Sequence](https://hackage.haskell.org/package/containers/docs/Data-Sequence.html)

```
:haddock:`containers/Data.Sequence#empty`
```
=> [Data.Sequence#empty](https://hackage.haskell.org/package/containers/docs/Data-Sequence.html#v:empty)

See the README for more info.
