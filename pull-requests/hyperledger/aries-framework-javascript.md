---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/657" class=".btn">#657</a>
            </td>
            <td>
                <b>
                    fix(basic-message): assert connection is ready
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim <karim@animo.id>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 22:12:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/655" class=".btn">#655</a>
            </td>
            <td>
                <b>
                    feat(core): add OOB record
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There are still some places where it's not so nice because of preserving compatibility with old connection protocol initialization.

I added `protocolCreateRequest` and `protocolProcessRequest` to `ConnectionService` but I want to separate them to`ConnectionProtocol` class later together with other "protocol" methods as `DidExchangeProtocol` class is organized.

We can also add some events around the OOB record, but I also leave it out, for now, to keep it simple.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 09:52:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/652" class=".btn">#652</a>
            </td>
            <td>
                <b>
                    feat: add wallet module with import export
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a wallet module that exposes the public api of the wallet. This is in preparation of the wallet upgrade work, but better addressed in a separate PR. 

After creating a wallet we should store the framework storage version in the wallet. If we do this directly in the wallet we depend on a repository from the wallet, which in turn depends on the wallet, creating a dependency cycle. I first created a hacky solution with tsyringe.

However it probably makes more sense to add another layer (the WalletModule) that exposes the public api of the wallet and allows to add extra logic to wallet methods without adding it to the wallet methods itself. Advantage is that wallet class keeps dependencies lighter, and we also can perform tasks that are generic to all wallet types (such as storing the framework storage version after creating a wallet). I will add this in a separate PR.

In addition this PR also adds support for import / export of the wallet which we'll also be using for the upgrade work. Now for NodeJS and will soon update rn-indy-sdk to support import / export

Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 18:48:26 +0000 UTC
    </div>
</div>

