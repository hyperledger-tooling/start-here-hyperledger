---
layout: default
title: firefly-tokens-erc20-erc721
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-tokens-erc20-erc721
---

# firefly-tokens-erc20-erc721 <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-tokens-erc20-erc721){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/88" class=".btn">#88</a>
            </td>
            <td>
                <b>
                    Only send one ack per batch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See #87 

Also contains fix for this build issue that crept in:
```
Step 23/31 : RUN npm install --production
 ---> Running in 77698a1b40ba
npm WARN config production Use `--omit=dev` instead.
npm WARN old lockfile
npm WARN old lockfile The package-lock.json file was created with an old version of npm,
npm WARN old lockfile so supplemental metadata must be fetched from the registry.
npm WARN old lockfile
npm WARN old lockfile This is a one-time fix-up, please be patient...
npm WARN old lockfile
npm notice
npm notice New minor version of npm available! 8.15.0 -> 8.19.1
npm notice Changelog: <https://github.com/npm/cli/releases/tag/v8.19.1>
npm notice Run `npm install -g npm@8.19.1` to update!
npm notice
npm ERR! code EACCES
npm ERR! syscall open
npm ERR! path /home/node/contracts/source/package-lock.json
npm ERR! errno -13
npm ERR! Error: EACCES: permission denied, open '/home/node/contracts/source/package-lock.json'
npm ERR!  [Error: EACCES: permission denied, open '/home/node/contracts/source/package-lock.json'] {
npm ERR!   errno: -13,
npm ERR!   code: 'EACCES',
npm ERR!   syscall: 'open',
npm ERR!   path: '/home/node/contracts/source/package-lock.json'
npm ERR! }
npm ERR!
npm ERR! The operation was rejected by your operating system.
npm ERR! It is likely you do not have the permissions to access this file as the current user
npm ERR!
npm ERR! If you believe this might be a permissions issue, please double-check the
npm ERR! permissions of the file and its containing directories, or try running
npm ERR! the command again as root/Administrator.

npm ERR! A complete log of this run can be found in:
npm ERR!     /home/node/.npm/_logs/2022-09-11T19_33_01_557Z-debug-0.log
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-11 18:16:57 +0000 UTC
    </div>
</div>

