---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2428" class=".btn">#2428</a>
            </td>
            <td>
                <b>
                    fix(supply-chain-app): print correct web host in the cli-logs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Through this PR, I'm trying to fix the incorrect Cockpit address in CLI logs issue(https://github.com/hyperledger/cacti/issues/2390). This partially achieves it. In the [examples/supply-chain-app/README.md doc](https://github.com/hyperledger/cacti/blob/main/examples/supply-chain-app/README.md) there's two ways to build the supply chain app locally - 1. to build the entire app locally (under Running the Example Application Locally) 2. To build it using the dockerfile (under Building and running the container locally). The changes I've made in examples/cactus-example-supply-chain-backend/src/main/typescript/supply-chain-app.ts, changes the address to 127.0.0.1 and prints the same in the logs, but only if I build the entire app locally using method 1.
I also made changes in the Dockerfile and process.env, assuming the same output for the docker build. But somehow when I build the container locally using 2, I still get 0.0.0.0 in the output. I would need some help to further debug this issue.
(I'd made another PR with some errors, and have closed it)
Fixes https://github.com/hyperledger/cacti/issues/2390
Signed-off-by: deepto98 [ddepp98@outlook.com](mailto:ddepp98@outlook.com)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-15 13:06:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2426" class=".btn">#2426</a>
            </td>
            <td>
                <b>
                    fix(ci): multiple bug fixes in weaver deployment workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes:
1. Go publish workflows: Correct the tagnames
2. Node workflows: fix typo in package.json after changing version (removed changing version in worklow)
3. Fix a typo in relay deployment workflow
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-15 11:50:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2425" class=".btn">#2425</a>
            </td>
            <td>
                <b>
                    style: 2021-09-20 linter warnings batch 17 / 26; part 2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2092
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-15 06:06:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2424" class=".btn">#2424</a>
            </td>
            <td>
                <b>
                    fix(webpack): fix broken bundling - cannot find webpack.config.js
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The `examples/cactus-workshop-examples-2022-11-14` package was causing `yarn build:dev` to fail. This PR fixes the incorrect webpack config path in the example's `package.json` file and adds a missing `/src/main/typescript/index.web.ts` file.
Fixes https://github.com/hyperledger/cacti/issues/2357
Signed-off-by: deepto98 [ddepp98@outlook.com](mailto:ddepp98@outlook.com)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-14 15:43:36 +0000 UTC
    </div>
</div>

