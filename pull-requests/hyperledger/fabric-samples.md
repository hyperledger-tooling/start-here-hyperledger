---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/801" class=".btn">#801</a>
            </td>
            <td>
                <b>
                    Fix vulnerabilities in typescript chaincode deps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                npm audit reveals several high and one critical vulnerabilities in the dependencies of asset-transfer-basic/chaincode-typescript:

ansi-regex  4.0.0 - 4.1.0
Severity: high
Inefficient Regular Expression Complexity in chalk/ansi-regex - https://github.com/advisories/GHSA-93q8-gq69-wqmw
fix available via `npm audit fix`
node_modules/nyc/node_modules/ansi-regex

minimist  <=1.2.5
Severity: critical
Prototype Pollution in minimist - https://github.com/advisories/GHSA-xvch-5gv4-984h
Prototype Pollution in minimist - https://github.com/advisories/GHSA-vh95-rmgr-6w4m
fix available via `npm audit fix --force`
Will install mocha@10.0.0, which is a breaking change
node_modules/minimist
node_modules/ts-node/node_modules/minimist
  mkdirp  0.4.1 - 0.5.1
  Depends on vulnerable versions of minimist
  node_modules/mkdirp
    mocha  1.21.5 - 6.2.2 || 7.0.0-esm1 - 7.1.0
    Depends on vulnerable versions of mkdirp
    node_modules/mocha

protobufjs  6.11.0 - 6.11.2
Severity: high
Prototype Pollution in protobufjs - https://github.com/advisories/GHSA-g954-5hwp-pp24
fix available via `npm audit fix`
node_modules/protobufjs

5 vulnerabilities (2 moderate, 2 high, 1 critical)

This change (from running npm audit fix --force) removes all of them:
npm audit
found 0 vulnerabilities

Signed-off-by: Arnaud J Le Hors <lehors@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 14:28:21 +0000 UTC
    </div>
</div>

