---
layout: default
title: pdo-contracts
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/pdo-contracts
---

# pdo-contracts <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/pdo-contracts){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/38" class=".btn">#38</a>
            </td>
            <td>
                <b>
                    Parameterize docker(-compose) commands
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Companion to [PDO PR #487](https://github.com/hyperledger-labs/private-data-objects/pull/487)  . See there for more context.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 21:33:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/37" class=".btn">#37</a>
            </td>
            <td>
                <b>
                    Switch notebooks to use service groups instead of a fixed host
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update the notebooks to take advantage of the transition to service groups. This should enable significantly more flexibility in selecting services from multiple sites.
    
Changed some of the way the "root" of a context is handled in order to keep group specification easier. If all of the services groups (eservice, pservice, and sservice) have the same name then a single service group setting is sufficient to pick all. Otherwise, each group can be overridden in the custom bindings.
    
Fixed line length in several of the notebooks.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-22 23:49:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/36" class=".btn">#36</a>
            </td>
            <td>
                <b>
                    Make the jupyter context functions more robust
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In order to support multiple namespaces for the contexts used in jupyter notebooks, make the context names and data more explicit. Fixes a problem with the exchange token issuer caused by a conflict in contexts.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-19 20:26:33 +0000 UTC
    </div>
</div>

