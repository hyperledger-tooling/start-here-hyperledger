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
                PR <a href="https://github.com/hyperledger/besu/pull/4336" class=".btn">#4336</a>
            </td>
            <td>
                <b>
                    Feature/tx sender future nonce limits
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">doc-change-required</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Adds cli configuration parameter and default value to limit concurrent/future transactions per sender in the txpool.  Also changes AbstractPendingTransactionSorter constructor to take a TransactionPoolConfiguration, rather than individual parameters per config item



## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
related to protocol-misc 629

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

TBA

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-01 03:38:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4335" class=".btn">#4335</a>
            </td>
            <td>
                <b>
                    4328 quiet cors errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Open question as to if this is overly broad: This will log the error message for all failed RPC calls, but not the stack trace, unless logging is turned up to debug.

This _seems_ to be the preferred way to do this in Vert.x, but I'm open to solutions that are more narrowly aimed at the CORS handling case.

## PR description

## Fixed Issue(s)
fixes #4328 

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 20:19:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4334" class=".btn">#4334</a>
            </td>
            <td>
                <b>
                    Fixing sub logging and moving stack trace to debug.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">logging</span>
            </td>
            <td>
                ## PR description
PR to change logging for more graceful usage on #4323. To access stack trace, use DEBUG for subscriber. 

## Fixed Issue(s)
 
Fixes #4323 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 19:06:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4327" class=".btn">#4327</a>
            </td>
            <td>
                <b>
                    Evict Transactions by sender from tail first
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
Ensure when besu evicts transactions by sender, that future nonces are evicted first


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
related to protocol-misc 629

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 17:06:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4325" class=".btn">#4325</a>
            </td>
            <td>
                <b>
                    refactors to rely on blocks added, and behave like singleton
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Will not show ready for merge on startup when local stored chain is past ttd.
Uses block observer to determine state change

Signed-off-by: Justin Florentine <justin+github@florentine.us>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-29 17:30:27 +0000 UTC
    </div>
</div>

