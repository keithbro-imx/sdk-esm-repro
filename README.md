```
npm i
npm run repro
```

Output:
```
❯ npm run repro     

> esm-sdk@1.0.0 repro
> node index.mjs

node:internal/process/esm_loader:34
      internalBinding('errors').triggerUncaughtException(
                                ^

Error [ERR_MODULE_NOT_FOUND]: Cannot find module '/Users/xxxx/dev/node-esm-sdk/node_modules/@opensea/seaport-js/lib/utils/eip712/bulk-orders' imported from /Users/xxxx/dev/node-esm-sdk/node_modules/@imtbl/sdk/dist/index.js
Did you mean to import "@opensea/seaport-js/lib/utils/eip712/bulk-orders.js"?
    at finalizeResolution (node:internal/modules/esm/resolve:265:11)
    at moduleResolve (node:internal/modules/esm/resolve:933:10)
    at defaultResolve (node:internal/modules/esm/resolve:1157:11)
    at ModuleLoader.defaultResolve (node:internal/modules/esm/loader:390:12)
    at ModuleLoader.resolve (node:internal/modules/esm/loader:359:25)
    at ModuleLoader.getModuleJob (node:internal/modules/esm/loader:234:38)
    at ModuleWrap.<anonymous> (node:internal/modules/esm/module_job:87:39)
    at link (node:internal/modules/esm/module_job:86:36) {
  code: 'ERR_MODULE_NOT_FOUND',
  url: 'file:///Users/xxxx/dev/node-esm-sdk/node_modules/@opensea/seaport-js/lib/utils/eip712/bulk-orders'
}

Node.js v20.12.2
```