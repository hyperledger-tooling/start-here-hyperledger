---
layout: default
title: minbft
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/minbft
---

# minbft <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/minbft){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minbft/pull/214" class=".btn">#214</a>
            </td>
            <td>
                <b>
                    NewView message type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                <!-- NOTE: Please check the contribution guideline before submitting -->

<!-- describe the purpose of the pull request, as well as its benefits
     and possible concerns related to the proposed changes -->
This pull request defines and implements NewView message type. NewView messages will be generated when the new primary collects a quorum of ViewChange messages.

Related to #178.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 21:01:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/minbft/pull/213" class=".btn">#213</a>
            </td>
            <td>
                <b>
                    Perform full testing in make test target by default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                This pull request changes the default behavior of make test target to perform full testing. The CI behavior is not changed: it still runs only short tests by setting `GOFLAGS="-short"` in the environment.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-29 20:56:07 +0000 UTC
    </div>
</div>

