---
layout: default
title: firefly-signer
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-signer
---

# firefly-signer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-signer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/44" class=".btn">#44</a>
            </td>
            <td>
                <b>
                    Separate error for parse result
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Correct invalid assumption in https://github.com/hyperledger/firefly-signer/pull/43 and provide a more helpful error on parse result failures.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-17 01:15:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/43" class=".btn">#43</a>
            </td>
            <td>
                <b>
                    Fix coverage gaps from recent PRs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Note there was one path I believe it was impossible to reach, with a special case for a receiving a valid JSON payload, where the `.result` could not be parsed as JSON.
So I change the code to not have a special branch for this, but still to ensure we capture the error if it ever happened.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-15 14:37:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-signer/pull/42" class=".btn">#42</a>
            </td>
            <td>
                <b>
                    fix: ABI decoding dynamic tuple arrays
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 10:08:41 +0000 UTC
    </div>
</div>

