---
layout: default
title: iroha-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-javascript
---

# iroha-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-javascript/pull/112" class=".btn">#112</a>
            </td>
            <td>
                <b>
                    Fix ESM/CJS problems
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">package: client</span><span class="chip">package: data model</span><span class="chip">package: crypto</span>
            </td>
            <td>
                ## List of changes

- Define packages exports with `exports` field too. Also use `.mjs` for ESM and `.cjs` for CJS bundles.

- Drop API Extractor and esbuild. Use `rollup` for everything.

  API Extractor broke after moving to `tsconfig` paths monorepo approach. It was done to define actual packages `main`/`module`/`exports` fields in their `package.json`. I moved to Rollup and `rollup-plugin-dts`.

  `esbuild` doesn't eliminate dead code in case like `if (undefined)` - [proof](https://hyrious.me/esbuild-repl/?version=0.14.42&mode=build&modules=%5B%5B%22main.js%22%2C%22if+%28undefined%29+%7B%5Cn++console.log%28123%29%5Cn%7D%5Cn%22%2C1%5D%5D&buildOptions=%7B%22bundle%22%3Atrue%2C%22format%22%3A%22esm%22%2C%22platform%22%3A%22neutral%22%2C%22minify%22%3Afalse%2C%22treeShaking%22%3Afalse%2C%22sourcesContent%22%3Afalse%2C%22keepNames%22%3Afalse%2C%22ignoreAnnotations%22%3Afalse%2C%22charset%22%3A%22utf8%22%2C%22splitting%22%3Afalse%2C%22target%22%3A%22esnext%22%2C%22sourcemap%22%3Afalse%7D). It brokes [in-source testing by Vitest](https://vitest.dev/guide/in-source.html#production-build). Thus, I moved again to Rollup.

- Drop `@iroha2/client-isomorphic-*`. Instead client library provides additional entrypoints for isomorphic adapters, like it is done at [`isomorphic-git`](https://github.com/isomorphic-git/isomorphic-git/tree/main#getting-started).
  
  For WebSocket, it has 2 entrypoints:

  ```ts
  // where native `WebSocket` exists
  import { adapter } from '@iroha2/client/web-socket/native'
  
  // Uses `ws` package for node.js
  import { adapter } from '@iroha2/client/web-socket/node'
  
  new Client({ ws: adapter })
  ```

  `fetch` could be provided in the same way, but `@iroha2/client` does not provide it by itself. There are `node-fetch` and `undici` packages that could solve it:

  ```ts
  import { fetch } from 'undici'
  import fetch from 'node-fetch'

  new Client({ fetch })
  ```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-31 14:09:04 +0000 UTC
    </div>
</div>

