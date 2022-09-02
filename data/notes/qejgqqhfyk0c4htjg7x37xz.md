
(starting notes a little late)

- bunch of criteria and it depends.

- Module formats
    - defines a module
- Of course we should only support ESM.
- Package has a carbon footprint depending on the size of the bundle.
- Reduce publish size
    - only publish required files with `package.json` 's `files` field.
- DefinitelyTyped will reduce package size.  _lol_
- TypeScript dist tags.
    - You can have a @variant on a package name `@scope/<name>@variant` when exporting a package.
- Provide ESM version of your package.
- Smaller modules
- Tree-shaking.

- Publishing a JS package:
    - Small package size
    - Observability with Open Trace (types.d.ts)
    - Support ESM and Common JS with multiple packages.
