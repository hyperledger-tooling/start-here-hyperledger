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
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/445" class=".btn">#445</a>
            </td>
            <td>
                <b>
                    enhancement: Starting only agents given in cmd
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

This PR modifies manage to only start agents specifically stated in the command. Previously it would attempt to start all roles even if they we not given. Now we can do commands like the following to just start agents needed. 
`./manage start -a acapy-main` Only starts acme as acapy-main. All other roles are not started.
`./manage start -a acapy-main -b afgo-interop` Only starts acme and bob. 
`./manage start -a afgo-interop -d acapy-main` This still works as before, acme is started as afgo, and all other roles are started as acapy-main. 

This enhancement is being done to support aries-mobile-test-harness that can use these agents as services when running mobile tests. It will not need 4 agents running so limiting to only what is asked for is required. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 13:00:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/444" class=".btn">#444</a>
            </td>
            <td>
                <b>
                    feat: didcomm v2 connection steps and afgo support
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
        Created At 2022-03-03 21:05:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/443" class=".btn">#443</a>
            </td>
            <td>
                <b>
                    Invalid link to Advanced Test Reporting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull request fixes an invalid link to Advanced Test Reporting in README.md.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 09:25:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/442" class=".btn">#442</a>
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
        Created At 2022-03-01 03:52:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/441" class=".btn">#441</a>
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
        Created At 2022-02-27 03:52:20 +0000 UTC
    </div>
</div>

