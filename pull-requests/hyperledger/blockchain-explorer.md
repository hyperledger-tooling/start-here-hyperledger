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

