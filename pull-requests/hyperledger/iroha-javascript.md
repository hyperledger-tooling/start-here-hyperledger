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
                PR <a href="https://github.com/hyperledger/iroha-javascript/pull/78" class=".btn">#78</a>
            </td>
            <td>
                <b>
                    Fix packages: paths (ts & jest), versions, changelogs etc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Remove paths from tsconfig and jest config - now direct imports from `"main": "src/lib.ts"` in `package.json`;
- Setup publish configs for each non-private package in `publishConfig` field of each `package.json`;
- Set `"private": true` for each of internal packages - test sub-packages of `crypto`, `@iroha2/test-peer`, `@iroha2/monorepo`;
- Make names of packages dirs consistent - remove `iroha-` prefix (so there a lot of just renamed files);
- Update dependencies;
- Setup `changesets` for version control.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 08:26:48 +0000 UTC
    </div>
</div>

