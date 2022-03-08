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

