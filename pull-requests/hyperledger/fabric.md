---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4569" class=".btn">#4569</a>
            </td>
            <td>
                <b>
                    Increase default transientstoreMaxBlockRetention
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Increase the default value of transientstoreMaxBlockRetention

Change-Id: I24eb6a6c4be38fbb964970b518d40c72e02e12ff

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

`transientstoreMaxBlockRetention` is used to trigger the purge of private data in the transient store.

The current default value is 1000, which is OK for simple cases with several blocks per second. Howerver, in our test with 10K tps case, it is possible to purge the private data too early before the peer gets a chance to commit the tx into the ledger.

With a larger retention window, the only cost is a larger transient database in the peer node, which is not a big deal.

Hence, this patchset suggest to increase the default value to a larger value of 100000, and it is open to have other reasonable value too.

#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-08 18:57:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4568" class=".btn">#4568</a>
            </td>
            <td>
                <b>
                    Add TLS passthrough and SANs info to TLS doc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add TLS passthrough and SANs info to the TLS documentation to address common user questions.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-08 17:01:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4563" class=".btn">#4563</a>
            </td>
            <td>
                <b>
                    Get value from array directly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The patchset simplifies the code implementation to iterate over an array.

Change-Id: I2f29335955e2ee1a4c0aabf2c744ca9b223a1a87

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

The patchset simplifies the code implementation to iterate over an array.

#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-05 17:32:50 +0000 UTC
    </div>
</div>

