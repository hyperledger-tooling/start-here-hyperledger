---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1570" class=".btn">#1570</a>
            </td>
            <td>
                <b>
                    Detect future timestamp on queue push
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change
Make `Queue` determine if a transaction has been tampered to have a future timestamp,
based on configurable threshold

### Issue
Close #1494

### Benefits
Prevent future timestamps and make transaction TTLs work well

### Possible Drawbacks
`DEFAULT_FUTURE_THRESHOLD_MS` may be debatable

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-27 14:43:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1569" class=".btn">#1569</a>
            </td>
            <td>
                <b>
                    GaroRobe/issue1197
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                <!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->


### Description of the Change

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

Added DiskIO mock for Kura testing. Currently only error injection is implemented.

### Issues

Closes #1197 

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks 

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 10:21:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1567" class=".btn">#1567</a>
            </td>
            <td>
                <b>
                    [GHA] remake matrix to buildspec, fix build with URSA
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Simplify GHA workflow matrix. Iroha+Ursa now is built, earlier it was a regular irohad.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 09:17:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1566" class=".btn">#1566</a>
            </td>
            <td>
                <b>
                    CI improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Aleksandr <a-p-petrosyan@yandex.ru>


### Description of the Change

Replaced the linker for coverage instrumentation tests with `lld`. 

### Issue

Should close  #1561 and #1558

### Benefits

Coverage works. 

### Possible Drawbacks

None
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 09:13:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1564" class=".btn">#1564</a>
            </td>
            <td>
                <b>
                    [GHA] CTest categories
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Better cathegories in CTest logs. Just a little improvement.
system_irohad_test now MAY FAIL, see #1554 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 08:45:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1563" class=".btn">#1563</a>
            </td>
            <td>
                <b>
                    Add optional nonce to distinguish transactions. Close #1493
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">api-changes</span>
            </td>
            <td>
                ### Description of the Change
* Add `Transaction.Payload.nonce` field
* Whether add nonce or not is configurable in `client/config.json`

### Issue
Close #1493

### Benefits
Can make different hashes for transactions which occur repeatedly and simultaneously

### Possible Drawbacks
Affection to performance unmeasured
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 06:28:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1562" class=".btn">#1562</a>
            </td>
            <td>
                <b>
                    I2 ci fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change

Removed unnecessary `sudo`, to fix the push pipeline.

### Issue

Closes #1561. 

### Benefits

Docker test and push pipelines should work. 

### Possible Drawbacks

Might not fix #1561. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-25 10:44:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1557" class=".btn">#1557</a>
            </td>
            <td>
                <b>
                    [mst] #1489 clean up, prettify
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                /build all

Signed-off-by: kuvaldini <ivan@kuvaldini.pro>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-25 08:32:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1556" class=".btn">#1556</a>
            </td>
            <td>
                <b>
                    Fix the random bounces in `create-docker` workflow.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ### Description of the Change

Changes the push workflow to run on a self-hosted container

### Issue

Some docker workflows have been failing on GitHub-hosted containers. 

### Benefits

They should now always work. 

### Possible Drawbacks

More CI usage and heavier load on the CI runners hosted on AWS. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-25 06:53:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1555" class=".btn">#1555</a>
            </td>
            <td>
                <b>
                    Add Unregister peer instruction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">iroha2</span><span class="chip">api-changes</span>
            </td>
            <td>
                ### Description of the Change

Adds an unregister peer instruction that  turns a trusted peer into an untrusted peer. 

### Issue

Resolves #1143 

### Benefits

Peers can now be unregistered. 

### Possible Drawbacks

Anyone can unregister the peer. The peer can be re-registered. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-25 06:45:11 +0000 UTC
    </div>
</div>

