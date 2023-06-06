---
layout: default
title: aries-rfcs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-rfcs
---

# aries-rfcs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-rfcs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/785" class=".btn">#785</a>
            </td>
            <td>
                <b>
                    Revise the well known goal codes aries.rel and aries.rel.build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 22:39:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/784" class=".btn">#784</a>
            </td>
            <td>
                <b>
                    [RFC0721] Add generic revocation format for anoncreds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding a dedicated revocation format entry for AnonCreds in Revocation Notification V2 protocol.

I'm not sure if it's actually needed, as we can probably use the existing 'indy-anoncreds' if we consider it appropriate for both indy and the standardized anoncreds specification. At least from the formatting (with the :: as separator) it seems it suits pretty well if all AnonCreds object IDs are URIs.

Not sure also if it would be needed to version it (like `anoncreds-v1`) in case AnonCreds V2 data model require a different approach.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-01 20:57:01 +0000 UTC
    </div>
</div>

