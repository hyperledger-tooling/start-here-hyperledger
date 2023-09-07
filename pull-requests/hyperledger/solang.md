---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1516" class=".btn">#1516</a>
            </td>
            <td>
                <b>
                    Polkadot: Support errors according to `solc`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">polkadot</span>
            </td>
            <td>
                Implement `Panic` and custom errors for the Polkadot target:
- Allow catching `Panic` in sema
- Allow custom errors in sema
- Implement selector  calculation for custom errors
- Refactor try-catch in codegen to allow catch clauses on `Panic` errors in
- Add any custom errors in the metadata
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 08:48:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1514" class=".btn">#1514</a>
            </td>
            <td>
                <b>
                    Add Rename functionality
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This feature depends on having the right span information for identifiers in the parse tree. Currently, some changes are needed to either add the missing span information in some cases, or improve the already present spans (look for one-off errors). 

The rest of the "goto-*" functions also depend on the availability of proper spans. But in their case, as no modification is made to the source code, lack of accurate spans is less of an issue. But `rename` does modify the source code and hence having incorrect spans can result in unintentionally overwriting pieces of source code, which is highly undesirable. 

The changes made as part of this PR provide the necessary code for `rename` to work. Correcting the parse tree is expected to be done as part of future PRs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-05 05:22:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1513" class=".btn">#1513</a>
            </td>
            <td>
                <b>
                    Reduce CI costs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                cargo clippy and cargo doc need to do the same work as cargo build, so put them in the linux job, and reduce the duplicate effort.

In addition, use the free windows runner as the cost for solang-windows-latest is much too high. @ryjones 

Before this PR, we would running clippy with the latest stable. After this PR, we run clippy with 1.70.0 (or the current version we're using for building, rather than latest). 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-04 12:49:31 +0000 UTC
    </div>
</div>

