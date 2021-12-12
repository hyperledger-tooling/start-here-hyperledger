---
layout: default
title: indy-did-method
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-did-method
---

# indy-did-method <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-did-method){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/25" class=".btn">#25</a>
            </td>
            <td>
                <b>
                    Change the separator for a sub-namespace to . from :
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Per #22 -- a PR that proposes changing the separator within the namespace component to be a "." instead of a ":", so that regex's are easier for extracting the components of a DID -- the "did" prefix, the "indy" method, the namespace and the namespace identifier. With this change, for each there is exactly one ":" between each of the 4 segments of the identifier (vs. 4 or 5 depending on the ledger name).

Per the [DID Spec identifier syntax rules](https://www.w3.org/TR/did-core/#did-syntax), the "." is permitted.  Alternatives are "-" and "_", but I think "." makes the most sense.



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-11 19:29:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-did-method/pull/24" class=".btn">#24</a>
            </td>
            <td>
                <b>
                    Fix typos
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
        Created At 2021-12-11 19:05:14 +0000 UTC
    </div>
</div>

