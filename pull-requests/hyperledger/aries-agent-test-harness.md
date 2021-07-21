---
layout: default
title: aries-agent-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-agent-test-harness
---

# aries-agent-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-agent-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/299" class=".btn">#299</a>
            </td>
            <td>
                <b>
                    Mobile wait states
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a delay to wait for mobile to make a connection request before responding

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-20 18:14:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/298" class=".btn">#298</a>
            </td>
            <td>
                <b>
                    chore: update afj backchannel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates AFJ backchannel to latest release on NPM. Haven't updated yet to use the main branch but that should be a minor addition now.

Let's hope this also resolves #282 (works for me locally)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-19 16:09:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/297" class=".btn">#297</a>
            </td>
            <td>
                <b>
                    Changes by create-pull-request action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-17 03:52:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/296" class=".btn">#296</a>
            </td>
            <td>
                <b>
                    fix: wait for uniresolver to be ready before running tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 20:10:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/295" class=".btn">#295</a>
            </td>
            <td>
                <b>
                    fix: stable uniresolver version for compatibility
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 07:10:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/294" class=".btn">#294</a>
            </td>
            <td>
                <b>
                    Changes by create-pull-request action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 03:52:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/293" class=".btn">#293</a>
            </td>
            <td>
                <b>
                    fix: acapy-backchannel not having curl
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Running this locally, the tests were failing after being unable to detect if the agents had been started. Upon inspection of the logs for the agents (which had actually started), the following was repeatedly printed until it timed out:

```
acapy/ngrok-wait.sh: line 12: curl: command not found
ngrok not ready, sleeping 5 seconds....
```

So I added curl to both of the acapy backchannel docker files which seemed to fix things. Not sure how this wasn't breaking things outside of my environment though :thinking: 

The other small tweak I've included is just a RHEL based system compatibility thing for mapping SELinux context.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-15 22:46:18 +0000 UTC
    </div>
</div>

