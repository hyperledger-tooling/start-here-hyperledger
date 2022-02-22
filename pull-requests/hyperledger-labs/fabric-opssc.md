---
layout: default
title: fabric-opssc
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-opssc
---

# fabric-opssc <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-opssc){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/32" class=".btn">#32</a>
            </td>
            <td>
                <b>
                    feat(*): Improve Web Socket notifications and some log formats
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch includes:
- feat(api-server): Add config options whether to enable WebSocket server
- feat(agent): Improve console log and WebSocket message format
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-18 11:32:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/31" class=".btn">#31</a>
            </td>
            <td>
                <b>
                    chore(*): Bump fabric versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch updates the fabric versions for build and testing:
- Update Fabric from 2.4.1 to 2.4.2
- Update Fabric from 2.2.4 to 2.2.5

Also, this patch removes the v2.3 series from build and testing
because they haven't been an update since the release of the 2.4 series.

This includes updating the OpsSC related material information in README.

Signed-off-by: Tatsuya Sato <tatsuya.sato.so@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-17 01:13:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/30" class=".btn">#30</a>
            </td>
            <td>
                <b>
                    Some bug fixes and adding a minor API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR includes the following updates.

- Bug fixes
  - Bug fix on the conditions for a vote to be considered `Rejected`
  - Bug fix in the case of reusing chaincode definitions without proposals
-  API updates
   - Add API to get organization information
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-16 04:02:42 +0000 UTC
    </div>
</div>

