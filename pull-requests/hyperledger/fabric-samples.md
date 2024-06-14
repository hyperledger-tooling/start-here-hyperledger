---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1221" class=".btn">#1221</a>
            </td>
            <td>
                <b>
                    Add chaincode logging for binary chaincode in test-network-nano-bash
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Correct sh compability in ca_utils.sh
- Correct linux compatibility in external builder
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-14 16:33:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1219" class=".btn">#1219</a>
            </td>
            <td>
                <b>
                    Use more specific chaincode package versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This demonstrates good practice in restricting the chaincode package versions to those applicable for the specific Fabric (major/minor) version targeted for deployment.

Also some corrections to the repository README. Particularly referring to other branches for samples targeted at earlier Fabric versions, since samples in the main branch may exploit features not available in older Fabric releases, which can cause confusion for end users.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-13 22:12:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1218" class=".btn">#1218</a>
            </td>
            <td>
                <b>
                    Use only v2.2.x chaincode package dependencies (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Avoid chaincode packages picking up dependencies on later v2.x releases, such as v2.5.x. Later releases may exploit features not compatible with the v2.2 chaincode container runtime.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-13 21:26:42 +0000 UTC
    </div>
</div>

