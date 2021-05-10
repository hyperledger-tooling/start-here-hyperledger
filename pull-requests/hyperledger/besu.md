---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2259" class=".btn">#2259</a>
            </td>
            <td>
                <b>
                    Rayonism
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
 merge master into rayonism


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 03:47:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2258" class=".btn">#2258</a>
            </td>
            <td>
                <b>
                    Revert "fix newblock transaction decoding RPC"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reverts hyperledger/besu#2256.  revert so Proto can get cred for his commit :)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 03:43:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2257" class=".btn">#2257</a>
            </td>
            <td>
                <b>
                    rayonism: fix newblock transaction decoding RPC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)

Previous `consensus_newBlock` (for the Merge prototype) was expecting full transactions, but the beacon node sends opaque transactions, and so blocks with a transaction would fail and cause the besu node to fail to sync the chain.

This mirrors the encoding code (stream tx list, map from hex and decoding instead of encoding and to hex, collect in list), and wraps it with some logging and error handling just in case. Tested this on a local merge testnet with all consensus and execution clients mining on top of the blocks, no errors.

<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
  - Small fix in experimental fork of besu, no new features, not updating changelog.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 03:35:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2256" class=".btn">#2256</a>
            </td>
            <td>
                <b>
                    fix newblock transaction decoding RPC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
fix consensus_newBlock transaction decoding

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 03:26:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2254" class=".btn">#2254</a>
            </td>
            <td>
                <b>
                    remove haveged; rename gq ATs executor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Remove haveged install; rename GoQuorum ATs executor to avoid confusion

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 01:42:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2252" class=".btn">#2252</a>
            </td>
            <td>
                <b>
                    Fix discovery packet size
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Antoine Toulme <antoine@lunar-ocean.com>

## PR description
Make sure Besu sends NEIGHBORS packets under MTU size.

## Fixed Issue(s)
#2250 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-08 23:00:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2249" class=".btn">#2249</a>
            </td>
            <td>
                <b>
                    parallelism 6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Parallelism 6

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-07 23:25:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2248" class=".btn">#2248</a>
            </td>
            <td>
                <b>
                    add ACCESS_LIST to BlockTransactionSelector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
add ACCESS_LIST to BlockTransactionSelector transaction size check switch statement 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2220
## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-07 22:47:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2247" class=".btn">#2247</a>
            </td>
            <td>
                <b>
                    force downloadLicenses when clean (#2104)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                when clean task is mentioned the lazyDownloadLicenses gets called before the clean runs, but during clean the license-dependency.xml also gets removed hence the checkLicenses.doLast fails. added the check to force downloadLicenses when clean task is going to run

Signed-off-by: Saravana Perumal Shanmugam <perusworld@linux.com>

fixes #2104 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-07 18:34:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2245" class=".btn">#2245</a>
            </td>
            <td>
                <b>
                    Implement eip 3541
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

Implement EIP 3541 as defined here https://github.com/ethereum/EIPs/pull/3541

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-07 16:45:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2244" class=".btn">#2244</a>
            </td>
            <td>
                <b>
                    Use gasLimit for EIP1559
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

Use gasLimit for EIP1559 as defined here https://github.com/ethereum/EIPs/commit/67d0d75f6393f6a109f2dc81cffc1e6541fb7aa3

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-07 15:14:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2242" class=".btn">#2242</a>
            </td>
            <td>
                <b>
                    [MINOR] condense tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

eth-api-disabled is always the first visible in the "thread blocked" logs

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-07 04:03:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2240" class=".btn">#2240</a>
            </td>
            <td>
                <b>
                    haveged + urandom
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Install haveged on AT executor to increase entropy available for non-java processes.

Also setting secure source to /dev/urandom/ explicitly (but not sure that is relevant)

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-06 23:04:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2239" class=".btn">#2239</a>
            </td>
            <td>
                <b>
                    Make 2930 accesslist transactions use frontier txn price calculator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
* Makes 1559 transaction price calculator use frontier for ACCESSLIST txns (as well as frontier txns)


## Fixed Issue(s)
fixes #2220

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-06 21:57:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2238" class=".btn">#2238</a>
            </td>
            <td>
                <b>
                    Implement eip 3529
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

Implement eip 3529 (version of the spec https://github.com/ethereum/EIPs/commit/6079eba5d1344a6b68075f79c14d4b7caf13ef53)

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-06 13:00:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2237" class=".btn">#2237</a>
            </td>
            <td>
                <b>
                    Add new fork for london, baikal and aleut
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

Changing the code to have :
- Aleut with only EIP1559 + BASEFEE OP CODE
- (Baikal + London) with 1559 + BASEFEE + other London EIPs
- Remove deprecated yolov3

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-06 10:55:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2236" class=".btn">#2236</a>
            </td>
            <td>
                <b>
                    change executor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-06 08:34:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2235" class=".btn">#2235</a>
            </td>
            <td>
                <b>
                    Refactor permissioning config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Tidy up the way PermissioningConfiguration get propagated between BesuCommand and BesuNode

Duplicate of https://github.com/hyperledger/besu/pull/2155 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-06 08:02:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2232" class=".btn">#2232</a>
            </td>
            <td>
                <b>
                    Qbft vote encoding to use empty for drop for extradata to match quorum
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
Qbft vote encoding to use empty for drop for extradata to match quorum

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2233

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-06 06:55:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2231" class=".btn">#2231</a>
            </td>
            <td>
                <b>
                    [MINOR] refactor out deprecation in test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Recursive comparison
 
## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-06 06:43:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2230" class=".btn">#2230</a>
            </td>
            <td>
                <b>
                    refactored perm ATs to remove dupe
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

While looking at flaky ATs, noticed these two tests were almost the same. 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-06 05:06:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2228" class=".btn">#2228</a>
            </td>
            <td>
                <b>
                    entropy - reduce parallelism
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Reduce parallelism to improve thread blockage situation.
Changing from 8 to 4 increased test time from 13 to 23 min
Changing to 6 made it ~15 min which is acceptable.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-06 00:18:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2227" class=".btn">#2227</a>
            </td>
            <td>
                <b>
                    Fix tracer crash
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

Fix a crash with tracer on Staticcall and callcode

## Test performed 

- Ropsten 
>curl --location --request POST 'http://127.0.0.1:8545' --header 'Content-Type: application/json' --data-raw '{"jsonrpc":"2.0","method":"debug_standardTraceBlockToFile","params":["0x0d9db1248c91a8a2f9b37442d50e7c38b2344853f35b1862e1cf6275ce792467", {"disableMemory":true}],"id":1}'

- Test with some FuzzyVM tests

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 13:28:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2226" class=".btn">#2226</a>
            </td>
            <td>
                <b>
                    Prevents EIP1559 blocks from being mined before fork
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

Prevents EIP1559 blocks from being mined before fork

## Changelog

- [x I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 13:12:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2224" class=".btn">#2224</a>
            </td>
            <td>
                <b>
                    fix goquorum privacy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #2198
The bug was that when we have a private transaction in goquorum mode and a contract calls another contract or a contract deploys another contract the sender account from the public world state was used, which caused the nonce to be incremented in the public state. 

Signed-off-by: Stefan Pingel <stefan.pingel@consensys.net>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 01:58:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2223" class=".btn">#2223</a>
            </td>
            <td>
                <b>
                    Rayonism Branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull puts the rayonism branch we used for steklo into a hyperledger branch.  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 01:46:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2222" class=".btn">#2222</a>
            </td>
            <td>
                <b>
                    update json-rpc responses for 1559
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
* adds 1559-specific fields to json-rpc responses for BlockResult and TransactionResult
* removes empty gasPrice from TransactionResult from json-rpc serialization
* removes gasLimit from 1559 transactions json-rpc serialization
* fixes retesteth eth_getTransactionCount to use a hex rather than decimal for result

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2215 
## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 01:27:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2218" class=".btn">#2218</a>
            </td>
            <td>
                <b>
                    PermissioningService Besu Plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # PermissioningService Besu Plugin

An additional plugin extension point has been added to besu to enable developers to intercept p2p connections and messages.

```java
public interface PermissioningService extends BesuPluginService {
  void registerNodePermissioningProvider(NodeConnectionPermissioningProvider provider);
  void registerNodeMessagePermissioningProvider(NodeMessagePermissioningProvider provider);
}
```

## NodeConnectionPermissioningProvider
This will allow plugin users to hook into node connections and when a node attempts to send messages using the following interface.
```java
@FunctionalInterface
public interface NodeConnectionPermissioningProvider {
  /**
   * Can be used to intercept the initial connection to a peer. Note that once a connection is
   * established it's bi-directional.
   *
   * @param sourceEnode the originators enode
   * @param destinationEnode the enode you are about to send to
   * @return if you can connect
   */
  boolean isConnectionPermitted(final EnodeURL sourceEnode, final EnodeURL destinationEnode);
}
```

## NodeMessagePermissioningProvider

If a provider has been registered through the plugin API all messages sent to a peer will use the hook to check if the message can be sent to a peer.

```java
@FunctionalInterface
public interface NodeMessagePermissioningProvider {
  /**
   * Can be used to intercept messages before they are sent from besu. 
   *
   * Note! this method is called on every message send.
   *
   * @param destinationEnode the enode you are about to send to
   * @param code devp2p code for the message
   * @return if we can send the message to the peer
   */
  boolean isMessagePermitted(final EnodeURL destinationEnode, final int code);
}
```
    

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-04 14:04:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2213" class=".btn">#2213</a>
            </td>
            <td>
                <b>
                    Ask block when not present
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

Two nodes stopped importing this weekend. This PR is a fix candidate. The nodes were late and some blocks were not stored in the pending blocks cache (because there is a size limit with announced blocks). At the time of importing the missing block, Besu did not find the block and stopped; Here is my theory. So I implemented a mechanism that directly asks the missing blocks to peers in these cases

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 14:13:55 +0000 UTC
    </div>
</div>

