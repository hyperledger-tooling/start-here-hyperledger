---
layout: default
title: go-perun
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/go-perun
---

# go-perun <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/go-perun){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/345" class=".btn">#345</a>
            </td>
            <td>
                <b>
                    Settle channel when funding fails
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #344.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 18:46:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/343" class=".btn">#343</a>
            </td>
            <td>
                <b>
                    Simplify virtual channel proposal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Before, it was quite involved to generate a virtual channel proposal. One had to provide so called index maps that specify how participant indices are remapped from root channel to virtual channel. For our current case of two-party, it is, however, quite simple to generate these based with a more simpler input (a boolean flag that denotes whether the participant order is the same or different).

depends on #342 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-19 15:12:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/342" class=".btn">#342</a>
            </td>
            <td>
                <b>
                    Satisfy linter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                My local version of golangci for some reason reports more than our CI. Goal of this PR: Satisfy local and remote golangci.

depends on #341 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-19 15:08:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/341" class=".btn">#341</a>
            </td>
            <td>
                <b>
                    Client tests: fail on error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Client tests involve concurrency. t.FailNow is not available there.
That's why we often used assert instead of require. Now we can use
role.Require.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-19 09:41:53 +0000 UTC
    </div>
</div>

