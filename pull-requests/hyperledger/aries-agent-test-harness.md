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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/291" class=".btn">#291</a>
            </td>
            <td>
                <b>
                    fix: acapy uniresolver plugin renamed, orb wrapper script made more robust
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
        Created At 2021-07-14 16:17:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/289" class=".btn">#289</a>
            </td>
            <td>
                <b>
                    chore: small bash script fix for platform compatibility
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
        Created At 2021-07-13 21:08:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/288" class=".btn">#288</a>
            </td>
            <td>
                <b>
                    feat: integrate orb did method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds `orb`, a new service, which runs a small orb network and a
universal resolver orb driver instance.

Integrates the service with the afgo backchannel, by having the service
create an orb did and save the value in a data folder for the afgo backchannel
to load.

Remember to start orb with `./manage service start orb` for tests where afgo
needs a public did.

Adds a general way to load files into agent containers:
A directory named <agent-name>.data (eg, afg-master.data), if present within the
backchannel's folder, will be mounted as a volume within the given agent,
to the path `/data-mount`.

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-12 15:02:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/287" class=".btn">#287</a>
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
        Created At 2021-07-12 03:52:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/286" class=".btn">#286</a>
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
        Created At 2021-07-10 03:52:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/285" class=".btn">#285</a>
            </td>
            <td>
                <b>
                    removed the acapy full runset since we are getting same-as-yesterday …
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …results from interop reports

Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-09 21:00:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/284" class=".btn">#284</a>
            </td>
            <td>
                <b>
                    removal of all role reversal tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

This PR removes any role reversal tests. This creates a strict adherence to the role assignments to the names used in the agents. IE. Acme is an issuer, Bob is a Holder, etc. Tests will no longer swap these roles, like Acme as a Holder or Bob as an Issuer. When assigning an agent in the run command to Acme `-a`, you can be sure that the agent will play the issuer role in all tests. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-09 20:53:47 +0000 UTC
    </div>
</div>

