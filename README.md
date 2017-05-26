# luapackageloader
CTAN module to allow LuaTeX to load packages from the default `package.path` and `package.cpath` locations. This could be useful
to load external Lua modules, including modules installed via [LuaRocks](https://luarocks.org).

## Usage
See the [PDF documentation](doc.pdf) for details.

Here is a quick TeX example:

```tex
\input luapackageloader

% Now we proceed to load a LuaRocks package
\directlua{
  local spt = require("serpent")
}
```

## License
Distributable under the LaTeX Project Public License, version 1.3c or higher (your choice). The latest version of this license is at: http://www.latex-project.org/lppl.txt

This work is "maintained" (as per LPPL maintenance status) by Deepak Jois.
