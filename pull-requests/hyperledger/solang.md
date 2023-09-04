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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1511" class=".btn">#1511</a>
            </td>
            <td>
                <b>
                    improve resolve pragma
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                reopen https://github.com/hyperledger/solang/pull/1218
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-31 13:28:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1509" class=".btn">#1509</a>
            </td>
            <td>
                <b>
                    Multiply known bits were not calculated correctly for unsigned multiply
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger/solang/issues/1507
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-30 13:37:34 +0000 UTC
    </div>
</div>

