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
                PR <a href="https://github.com/hyperledger/besu/pull/6329" class=".btn">#6329</a>
            </td>
            <td>
                <b>
                    Copy also computed fields, when doing a Transaction detached copy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-22 15:59:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6328" class=".btn">#6328</a>
            </td>
            <td>
                <b>
                    Optimize RocksDB WAL file
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

Currently Besu uses the default RocksDB WAL options, with the result that usually the WAL files could occupy ~15GB of disk space, due to the fact that different column families are flushed at very different intervals, this has also the bad effect of slow restarts, when Besu has to parse an reapply all these WAL files.

Capping the WAL files total size to 1GB and reusing old files when possible, has the advantage of a faster restart, and a more linear disk usage, instead of the classic saw tooth shape that we see today.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-22 11:01:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6322" class=".btn">#6322</a>
            </td>
            <td>
                <b>
                    Cancun forkids for non-mainnets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                add new forkids for testnets, update forkid test to Junit5, no longer need named network specific trusted setups


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-21 18:53:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6316" class=".btn">#6316</a>
            </td>
            <td>
                <b>
                    add missing check for static peers to allow them to exceed the connection limit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
In one place there was a check missing to allow static peers to exceed the connection limit.
Another improvement is that streamBestPeers() does only return fully validated peers.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-20 02:13:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6315" class=".btn">#6315</a>
            </td>
            <td>
                <b>
                    Log/Address Trielog rolling failure
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

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-19 23:41:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6313" class=".btn">#6313</a>
            </td>
            <td>
                <b>
                    fix: call OperationTracer.traceEndTx for failing transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Call `OperationTracer.traceEndTx` even when a transaction failed.

## Fixed Issue(s)
fixes #6312 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-19 13:06:11 +0000 UTC
    </div>
</div>

