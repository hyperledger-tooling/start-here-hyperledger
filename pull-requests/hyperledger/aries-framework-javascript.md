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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/411" class=".btn">#411</a>
            </td>
            <td>
                <b>
                    Fix bug/mediator restarts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-27 07:15:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/410" class=".btn">#410</a>
            </td>
            <td>
                <b>
                    build: fix start scripts for mediators
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                the start scripts used in the docker-compose setup do not match with the actual name of the start scripts that are defined in the package.json
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-26 07:58:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/408" class=".btn">#408</a>
            </td>
            <td>
                <b>
                    docs: mention monorepo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This mainly adds to the README that this is currenly a monorepo. It shows all the packages and their respective versioning. Since we use the same versionig strategy for every package, it might be a bit redundant. Open for suggestions, but IMO this is a relatively nice way to do it.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 11:06:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/407" class=".btn">#407</a>
            </td>
            <td>
                <b>
                    fix(redux-store): credential and proof selector by id
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The current `ById` selectors in the proof and credential selector were probably copied from the `connectionSelector`. Two function names did not change.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 10:13:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/406" class=".btn">#406</a>
            </td>
            <td>
                <b>
                    test: longer timeout for issue credential helper
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Because we use auto-accept in issue credential helper it can take a while to have the whole credential flow finished. Both parties need to interact with the ledger and sign/verify the credential
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 09:51:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/405" class=".btn">#405</a>
            </td>
            <td>
                <b>
                    test: fix test flakyness
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                this should hopefully fix the randomly failing tests. There were some weird promise calls causing timeouts...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 23:04:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/404" class=".btn">#404</a>
            </td>
            <td>
                <b>
                    chore: update to indy-sdk-react-native
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>

Use indy-sdk-react-native instead of rn-indy-sdk. Best to wait until https://github.com/hyperledger/indy-sdk-react-native/pull/14 is merged
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 22:23:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/403" class=".btn">#403</a>
            </td>
            <td>
                <b>
                    priority sorted transports
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Adam Burdett <burdettadam@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 00:38:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/402" class=".btn">#402</a>
            </td>
            <td>
                <b>
                    fix(core): do not use did-communication service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Do not include the `did-communication` service in the did doc for now. This break interop with AF.NET. We should solve this in the future by only using `IndyAgent` for connection protocol and did-communication for did exchange protocol
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 21:15:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/398" class=".btn">#398</a>
            </td>
            <td>
                <b>
                    feat(core): ledger module registerPublicDid implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add missing implementation for registerPublicDid in ledger module.

Apart from ledger source files, there were some updates in ledger setup scripts in order to properly run the tests, as it is needed to have some permissions to write public DIDs.

Signed-off-by: Ariel Gentile <gentilester@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-20 21:00:24 +0000 UTC
    </div>
</div>

