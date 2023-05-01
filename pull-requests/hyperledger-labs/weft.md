---
layout: default
title: weft
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weft
---

# weft <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weft){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weft/pull/31" class=".btn">#31</a>
            </td>
            <td>
                <b>
                    Fix walletpath option in wallet command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Example error:

```
$ weft wallet ls --walletpath ./_cfg/_wallets/DigiBank
weft wallet ls

Lists Application Wallet identities

Opciones:
      --help          Muestra ayuda  [booleano]
  -v, --version       Muestra número de versión  [booleano]
  -w, --walletpath    Path to application wallet  [requerido]
  -c, --compat        Set to use the 1.4 wallet format  [booleano] [defecto: false]
  -r, --createwallet  Create the wallet if not present  [booleano] [defecto: false]
  -f, --force         If the identity is already present, force overwrite it  [booleano] [defecto: false]

TypeError: The "path" argument must be of type string. Received undefined
    at new NodeError (node:internal/errors:399:5)
    at validateString (node:internal/validators:163:11)
    at Object.resolve (node:path:1102:7)
    at resolveWalletPath (/opt/homebrew/lib/node_modules/@hyperledger-labs/weft/src/userutils.ts:12:19)
    at /opt/homebrew/lib/node_modules/@hyperledger-labs/weft/src/cli.ts:267:53
    at Generator.next (<anonymous>)
    at /opt/homebrew/lib/node_modules/@hyperledger-labs/weft/lib/cli.js:32:71
    at new Promise (<anonymous>)
    at __awaiter (/opt/homebrew/lib/node_modules/@hyperledger-labs/weft/lib/cli.js:28:12)
    at Object.handler (/opt/homebrew/lib/node_modules/@hyperledger-labs/weft/src/cli.ts:265:33) {
  code: 'ERR_INVALID_ARG_TYPE'
}
```

After the fix:

```
weft wallet ls --wallet ./_cfg/_wallets/DigiBank
Listing application wallet identities /Users/japi/tmp/_cfg/_wallets/DigiBank
Complete
> digibankadmin
> digibankcaadmin

```
The problem occurs because it uses args['wallet'] instead of args['walletpath']:

```
        .command(
            'ls',
            'Lists Application Wallet identities',
            (yargs: any) => {
                return yargs;
            },
            async (args: any) => {
                // resolve the supplied gateway and wallet paths
                const walletPath = resolveWalletPath(args['wallet'] as string);
                log({ msg: 'Listing application wallet identities', val: walletPath });

                const idtools = new Identities(walletPath);
                idtools.list();
            },
        );

```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-01 17:32:22 +0000 UTC
    </div>
</div>

