Steps to reproduce:
1. `npm install` from `core-package`
2. `npm install ../core-package` from 'application'
3. run `typings install npm:@company/core-package/typings.json --save` it fails with 

```
typings ERR! message Unable to resolve "npm:ng-table" from "npm:@company/core-package/typings.json"
typings ERR! caused by Unable to find "node_modules\ng-table\package.json" from "c:\Work\application\node_modules\@company\core-package"
```

It works OK, if I move ng-table from dependencies to ambientDependencies