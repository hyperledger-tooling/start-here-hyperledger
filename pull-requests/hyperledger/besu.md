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
                PR <a href="https://github.com/hyperledger/besu/pull/4906" class=".btn">#4906</a>
            </td>
            <td>
                <b>
                    Address bonsai self-destruct stale code present 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
During an initial worldstate sync, a self-destruct that occurs between the initial pivot block and final heal pivot block will leave stale code in bonsai code storage.  If subsequently the code is redeployed via create2 to the same contract address, the bonsai db will fail to roll code changes to the block where the redeployment occurs.  This presents in a handful of ways such as 'worldstate not present' or 'unable to copy layered worldstate'.

Discussing with @matkt, since the repivot and heal process does not presently have an opportunity to 'heal' the code storage, and we should be able to trust the trielogs, this PR changes the rollCodeForward behavior to overwrite stale code if/when it is found.  This should resolve #4784 and give the besu team an opportunity to revisit this in flat database heal work that is ongoing.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
addresses #4784 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 16:05:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4905" class=".btn">#4905</a>
            </td>
            <td>
                <b>
                    Ibft1 deprecation warning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Add IBFT1 deprecation warning.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fix #4851
related to #4839

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 03:02:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4903" class=".btn">#4903</a>
            </td>
            <td>
                <b>
                    Preload node and not only rlp
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 14:28:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4902" class=".btn">#4902</a>
            </td>
            <td>
                <b>
                    [RPC] add SAFE and FINALIZED options for block param
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">RPC</span>
            </td>
            <td>
                RPC method changes
- add SAFE and FINALIZED options for block param
- check length of blockNumber / blockHash param - if it's too short to be a blockHash and too long to be a blockNumber, throw Invalid params
- added some extra tests. Specifically this file `eth_getTransactionCount_invalidBlockNumber.json` - without the code changes in this PR, that spec test returns "block not found", with these changes returns Invalid params

See #4233 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 05:02:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4900" class=".btn">#4900</a>
            </td>
            <td>
                <b>
                    Support Shanghai in Reference Tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Add support for Shanghai in reference tests
* Add Shanghai and Cancun milestones
* Add "withdrawals" and "withdrawalsRoot" to json objects
* Migrate to schedule by block header.

Signed-off-by: Danno Ferrin <danno.ferrin@swirldslabs.com>

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 23:07:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4899" class=".btn">#4899</a>
            </td>
            <td>
                <b>
                    fix toml parsing of double type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix toml config file parsing for options that map to type Double. Previously setting a value in toml config for a long option type would result in, e.g. :

```
Value of 'tx-pool-limit-by-account-percentage' is a float
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 16:03:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4898" class=".btn">#4898</a>
            </td>
            <td>
                <b>
                    EOF Optimization - don't split code sections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Optimize the EOF Functions implementation by not splitting code sections into separate Bytes object.  Instead the EOF evaluation occurs on a single container space.  When a function is called the PC (relative to container start, not section start) is moved, and no section re-loading needs to occur.

EOF lacks PC introspection and absolute jumps, so where "PC=0" starts is not observable to the code.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 15:44:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4897" class=".btn">#4897</a>
            </td>
            <td>
                <b>
                    use bonsai updater cache to avoid calling database several times for the same account
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …the same value

Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 14:22:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4895" class=".btn">#4895</a>
            </td>
            <td>
                <b>
                    For TimestampSchedule (Shanghai) remove evmBuilder override but leave other mods in
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span><span class="chip">EIP</span>
            </td>
            <td>
                Ideally, want to remove all the modifications, but that will be addressed by https://github.com/hyperledger/besu/issues/4788
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 08:12:37 +0000 UTC
    </div>
</div>

