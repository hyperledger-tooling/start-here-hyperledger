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
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/348" class=".btn">#348</a>
            </td>
            <td>
                <b>
                    📝 channel: Improve Data documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For verifying signatures, we require that the State.Data encoding is stable, that is, `E(data) = E(D(E(data)))`. This PR proposes to specify that requirement at the Interface.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-30 13:43:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/347" class=".btn">#347</a>
            </td>
            <td>
                <b>
                    :art: client/test: Reduce setup complexity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously, we introduced error channels for immediate error handling.
However, this was done at the expense of requiring an additional error
channel parameter during testing setup, which made it more complicated
to setup a client test. Now the error channels are kept only with the
role and the changes to the setup function parameters are reverted.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-30 13:34:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/346" class=".btn">#346</a>
            </td>
            <td>
                <b>
                    Update CHANGELOG v0.10.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates the CHANGELOG for release v0.10.0.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-25 12:49:43 +0000 UTC
    </div>
</div>

