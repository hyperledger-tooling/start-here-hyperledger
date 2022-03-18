---
layout: default
title: blockchain-explorer
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/blockchain-explorer
---

# blockchain-explorer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/blockchain-explorer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/blockchain-explorer/pull/283" class=".btn">#283</a>
            </td>
            <td>
                <b>
                    Fix: convert-hex can’t convert Buffer to Hex properly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Bug
In explorer, you convert `envelope_signature`, `payload_extension`, `creator_nonce`, `input`, `endorser_signature` to Hex with `convertHex.bytesToHex`

`convertHex.bytesToHex` can’t deal with hex include `a` `b` `c` `d` `e`, for example, 
```node
const convertHex = require('convert-hex');

let test = Buffer.from('HELLO');
console.log(test.toString('hex'));
console.log(convertHex.bytesToHex(test));
```
`H` is `48`
`E` is `45`
`L` is `4c`
`O` is `4f`
`HELLO` should be `48454c4c4f`

But when I try to use `convertHex.bytesToHex`, the result is `4845000`. Those hex with `abcde` is converted into `0`

# Steps To Reproduce
Step1: Add some `console.log` to explore (in commit 7a3caeedae72181c8df54b929b85f7cee2cf6e5d), build a docker image. 
```bash
git checkout 7a3caeedae72181c8df54b929b85f7cee2cf6e5d
docker build -t hyperledger/explorer:1.1.3 . # BDK use image `hyperledger/explorer:1.1.3` by default.
```
Step2: Use [BDK](https://github.com/cathayddt/bdk) build a simple network with explorer for test
```bash
cd ~
git clone https://github.com/cathayddt/bdk.git
cd bdk

# Install the bdk
npm install
npm run build:console

# set network name
export BDK_NETWORK_NAME=explorer-test
. ./cicd/test_script/steps/set-params.sh

# create network
bdk network create -f ./cicd/test_script/network-create.json --create-full
. ./cicd/test_script/steps/peer-and-orderer-up.sh

# create channel
. ./cicd/test_script/steps/channel.sh

# start explorer
. ./cicd/test_script/steps/explorer.sh

# build and use chaincode
. ./cicd/test_script/steps/chaincode.sh
```
hint: BDK would create folder at `~/.bdk` and run several docker container. You can delete those after testing.

Step3: run `docker logs -f explorer.explorer-test` show explorer log.

The result show that `envelope_signature`, `payload_extension`, `creator_nonce`, `input`, `endorser_signature` is Buffer type, and `Buffer.from(xxx).toString(‘hex’)` work correctly: 
```
-----envelope_signature-----
raw: <Buffer 30 44 02 20 75 34 f8 ed 6f f0 e2 9f 74 53 73 35 54 5f ed c7 e8 22 bc c6 14 ff d8 79 44 21 2b 36 f0 dc 55 59 02 20 6d 55 b8 89 c7 34 fa 94 b2 1d b8 64 ... 20 more bytes>
convertHex: 3044220753400000074537335540000220014007944210360055592200550890340940006407432333401900201114075009926944
toString: 304402207534f8ed6ff0e29f74537335545fedc7e822bcc614ffd87944212b36f0dc555902206d55b889c734fa94b21db864b174323334a119d6a8201114e475fe3a99260944
++++++++++++++++++++++++++++
-----payload_extension-----
raw: <Buffer 12 08 12 06 66 61 62 63 61 72>
convertHex: 128126666162636172
toString: 12081206666162636172
+++++++++++++++++++++++++++
-----creator_nonce-----
raw: <Buffer 29 e2 19 8e 77 60 83 2a c6 23 92 27 33 91 8b 68 79 2a 16 31 6b 21 0d 21>
convertHex: 2901907760830023922733910687901631021021
toString: 29e2198e7760832ac623922733918b68792a16316b210d21
+++++++++++++++++++++++
-----input-----
raw: <Buffer 43 72 65 61 74 65 43 61 72>
convertHex: 437265617465436172
toString: 437265617465436172
+++++++++++++++
-----input-----
raw: <Buffer 43 41 52 5f 4f 52 47 33 5f 50 45 45 52 30>
convertHex: 4341520052473305045455230
toString: 4341525f4f5247335f5045455230
+++++++++++++++
-----input-----
raw: <Buffer 42 4d 57>
convertHex: 42057
toString: 424d57
+++++++++++++++
-----input-----
raw: <Buffer 58 36>
convertHex: 5836
toString: 5836
+++++++++++++++
-----input-----
raw: <Buffer 62 6c 75 65>
convertHex: 6207565
toString: 626c7565
+++++++++++++++
-----input-----
raw: <Buffer 4f 72 67 33>
convertHex: 0726733
toString: 4f726733
+++++++++++++++
-----endorser_signature-----
<Buffer 30 45 02 21 00 ec 52 51 c1 30 88 f4 85 82 c9 65 75 b7 08 11 95 67 3e 36 57 37 2d f1 30 b1 19 24 20 99 2a d0 69 02 20 6f 19 18 93 38 7b 1e c6 83 f4 c2 ... 21 more bytes>
convertHex: 3045221005251030880858206575081195670365737003001924209900692200191893380008300007250026470010000078930320
toString: 3045022100ec5251c13088f48582c96575b7081195673e3657372df130b1192420992ad06902206f191893387b1ec683f4c29d9f7205f78f26478af501b6ee6be6a67893c0320a
++++++++++++++++++++++++++++
```

# Solution
Use `Buffer.from(input).toString('hex')` rather then `convertHex.bytesToHex(input)`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 07:32:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/blockchain-explorer/pull/282" class=".btn">#282</a>
            </td>
            <td>
                <b>
                    Bump follow-redirects from 1.14.7 to 1.14.9 in /client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [follow-redirects](https://github.com/follow-redirects/follow-redirects) from 1.14.7 to 1.14.9.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/13136e95bbe23cabbeaeb74bd0c933aa98dd9b96"><code>13136e9</code></a> Release version 1.14.9 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/2ec9b0ba850b932e82cf7fdc835e5136d0d0c8ad"><code>2ec9b0b</code></a> Keep headers when upgrading from HTTP to HTTPS.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/5fc74dd975b88a82508679cc0fda63f8c6a396ec"><code>5fc74dd</code></a> Reduce nesting.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/3d81dc3237b4ffe8b722bb3d1c70a7866657166e"><code>3d81dc3</code></a> Release version 1.14.8 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/62e546a99c07c3ee5e4e0718c84a6ca127c5c445"><code>62e546a</code></a> Drop confidential headers across schemes.</li>
<li>See full diff in <a href="https://github.com/follow-redirects/follow-redirects/compare/v1.14.7...v1.14.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=follow-redirects&package-manager=npm_and_yarn&previous-version=1.14.7&new-version=1.14.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
[//]: # (dependabot-automerge-end)

---

<details>
<summary>Dependabot commands and options</summary>
<br />

You can trigger Dependabot actions by commenting on this PR:
- `@dependabot rebase` will rebase this PR
- `@dependabot recreate` will recreate this PR, overwriting any edits that have been made to it
- `@dependabot merge` will merge this PR after your CI passes on it
- `@dependabot squash and merge` will squash and merge this PR after your CI passes on it
- `@dependabot cancel merge` will cancel a previously requested merge and block automerging
- `@dependabot reopen` will reopen this PR if it is closed
- `@dependabot close` will close this PR and stop Dependabot recreating it. You can achieve the same result by closing it manually
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/blockchain-explorer/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-13 15:40:22 +0000 UTC
    </div>
</div>

