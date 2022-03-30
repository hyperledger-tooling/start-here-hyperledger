---
layout: default
title: hlf-connector
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/hlf-connector
---

# hlf-connector <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/hlf-connector){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hlf-connector/pull/20" class=".btn">#20</a>
            </td>
            <td>
                <b>
                    Fabric Config - chaincode and block to accept List instead of comma-separated string
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: n0p0328 <nithin.pankaj@walmartlabs.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 12:24:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hlf-connector/pull/19" class=".btn">#19</a>
            </td>
            <td>
                <b>
                    add org to channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **6 Functionalities Covered:**
1. Get Configuration File
2. Generate Configuration Update File - Step 1/3
3. Sign the Configuration Update File - Step 2/3
4. Commit the Configuration File to the Ledger - Step 3/3
5. Add an Organization to the Channel Configuration (in one function call)
6.  Decode encoded configuration files produced by any of the above methods

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 01:47:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hlf-connector/pull/18" class=".btn">#18</a>
            </td>
            <td>
                <b>
                    Jackson serialize PrivateData EmptyList field to empty string
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Currently, if the privateData list is empty , jackson outputs it as json array i.e "[]" , to keep it inline with chaincode_event empty privateData, it is made empty string.

Signed-off-by:Jitendra Das <jitendra.das@walmartlabs.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 15:04:09 +0000 UTC
    </div>
</div>

