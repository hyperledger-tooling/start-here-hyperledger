---
layout: default
title: firefly-ethconnect
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-ethconnect/pull/121" class=".btn">#121</a>
            </td>
            <td>
                <b>
                    Add env vars for debrand migration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR add environments variables to support migration of existing public API spec for ethconnect, once https://github.com/kaleido-io/ethconnect/pull/118 for debranding ethconnect away from Kaleido. This work is based off https://github.com/kaleido-io/ethconnect/pull/118 and can be merged after that PR is merged. 

Environment variables introduced are `PREFIX_SHORT` ( default values `fly`) and `PREFIX_LONG` (default `firefly`) 
as suggested by @jimthematrix here https://github.com/kaleido-io/ethconnect/pull/118#pullrequestreview-674348896
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-08 21:39:10 +0000 UTC
    </div>
</div>

