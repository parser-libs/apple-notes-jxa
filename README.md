Parser-Libs / Apple Note JXA
===================

Simple module to read, edit, and manage Apple Notes throught JXA (offline)

## Using this module in other modules

Here is a quick example of how this module can be used in other modules. The [TypeScript Module Resolution Logic](https://www.typescriptlang.org/docs/handbook/module-resolution.html) makes it quite easy. The file `src/index.ts` acts as an aggregator of all the functionality in this module. It imports from other files and re-exports to provide a unified interface for this module. The _package.json_ file contains `main` attribute that points to the generated `lib/index.js` file and `typings` attribute that points to the generated `lib/index.d.ts` file.



- To use in TypeScript file -

```ts
import * as Notes from "@parser-libs/apple-notes-jxa";

Notes.accounts()
  .then((accounts) => console.log(accounts));
```

- To use in a JavaScript file -

```js
const Notes = require('@parser-libs/apple-notes-jxa');

Notes.accounts()
  .then((accounts) => console.log(accounts));
```

## License

Source code is licensed under the [Apache Licence, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html).

Copyright (c) 2022 Alex <alex@milyutin.work>

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
