---
layout: default
title: weaver-dlt-interoperability
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/weaver-dlt-interoperability
---

# weaver-dlt-interoperability <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/weaver-dlt-interoperability){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/262" class=".btn">#262</a>
            </td>
            <td>
                <b>
                    changes to support various hash mechanisms
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Krishnasuri Narayanam <knaraya3@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 07:44:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/261" class=".btn">#261</a>
            </td>
            <td>
                <b>
                    Making Interop SDK Hash Extensible
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Feature addition:
1. Added interface to Fabric interop SDK for Hash. Implemented default SHA256.
2. Updated Fabric-cli as per the above hash interface.
3. Update fabric-cli exchange-step command, and replaced with different lock, claim, and unlock commands.
4. Docs updated as per above changes.
5. Updated SDK unit tests as per above change.

RFC:
1. Added API specs for relay.
2. Added message specs used for data sharing.

Others:
1. Version bump v1.3.0 for all fabric modules, relay and protos.
2. Access control logs added to corda interop app.
3. Fixed makefiles for interopcc, interop sdk, and fabric-cli.
4. Made semi-local tests in workflows use locally built docker images.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 06:50:46 +0000 UTC
    </div>
</div>

