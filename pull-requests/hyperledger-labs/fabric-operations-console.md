---
layout: default
title: fabric-operations-console
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operations-console
---

# fabric-operations-console <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operations-console){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/688" class=".btn">#688</a>
            </td>
            <td>
                <b>
                    Revert to UBI8 for now.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It's premature to move to UBI-9 at the moment and causes too many issues with build process.  The other changes can stay and remain helpful improvements.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-12 16:08:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/687" class=".btn">#687</a>
            </td>
            <td>
                <b>
                    Upgrade underlying runtimes/os.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

* Upgrade console image(s) to UBI-9 base image and build images.
* Upgrade grpcweb base image to Go v1.21.9.
* Upgrade to Python v3.12 in workflows.

My motivation is that many of these OSes and runtime versions have either gone End of Life or are approaching EOL, and many of them contain known security vulnerabilities.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-09 20:36:45 +0000 UTC
    </div>
</div>

