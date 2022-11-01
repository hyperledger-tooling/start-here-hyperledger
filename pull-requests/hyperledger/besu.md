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
                PR <a href="https://github.com/hyperledger/besu/pull/4557" class=".btn">#4557</a>
            </td>
            <td>
                <b>
                    DRY-up *PendingTransactionSorter tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Based on previous work of @garyschulte

Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

`BaseFeePendingTransactionsTest` and `GasPricePendingTransactionsTest` have a lot in common, so make sense to extract shared code in a superclass

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-25 14:41:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4555" class=".btn">#4555</a>
            </td>
            <td>
                <b>
                    List.of like utility class for BlockBodies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a QoL refactor that should not have an effect of behaviour. 

When working on Withdrawals I noticed code similar to some of these:
```
  new BlockBody(emptyList(),emptyList());
  new BlockBody(List.of(transaction1),emptyList());
  new BlockBody(emptyList(),List.of(ommerHeader));
```

This PR adds a utility class BlockBodies that should work similarly to List.of(...) there is a BlockBodies.empty()
there is a utility method for BlockBodies.of(transaction) there is a utility method for BlockBodies.of(ommerHeader)

And there will be probably similar one when you will need a Block body only with a withdrawal.

The BlockBody.empty() was moved into this utility class as well...

Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-25 10:07:31 +0000 UTC
    </div>
</div>

