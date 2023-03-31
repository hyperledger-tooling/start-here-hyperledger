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
                PR <a href="https://github.com/hyperledger-labs/weaver-dlt-interoperability/pull/389" class=".btn">#389</a>
            </td>
            <td>
                <b>
                    Rust dependencies upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Upgrade tokio from v0.2 to v1.27
2. Upgrade all dependencies of protos-rs
3. Upgrade almost all dependencies of relay.
4. Added TLS based tests in relay unit test workflow.
5. Add retry logic while opening DB for both relay and driver.
6. Delay of 1 sec before polling again in fabric sdk data sharing.

Version Bumps:
- Bump protos-rs to v1.5.7
- Bump relay to v1.5.11
- Bump Fabric Driver to v1.5.11
- Bump Fabric SDK to v1.5.11
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 06:41:26 +0000 UTC
    </div>
</div>

