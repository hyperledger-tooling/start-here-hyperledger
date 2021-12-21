---
layout: default
title: fabric-opssc
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-opssc
---

# fabric-opssc <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-opssc){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/19" class=".btn">#19</a>
            </td>
            <td>
                <b>
                    Bump to 2.4.1 and fix some bugs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR bumps the fabric version to 2.4.1.
Also, the PR adds an API to get channel info for API server and fixes a bug in agent to pass the integration tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-20 11:14:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/18" class=".btn">#18</a>
            </td>
            <td>
                <b>
                    fix(agent): Fix a bug when handling a proposal not using the next sequence
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Normally, if a proposal uses an incorrect sequence number, there is no problem
because committing the chaincode definition will fail.

However, in the case of a proposal with the current sequence number and a new
chaincode source code, the approval process will update the chaincode package
in the sequence unexpectedly. Furthermore, in the case of using an earlier
sequence number, resources are wasted due to installing the chaincode successfully.

To avoid the cases, this patch adds a process to compare the committed sequence
number with the proposed one at the top of prepareToDeploy().

Also, the PR includes some minor modifications.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-16 11:22:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/17" class=".btn">#17</a>
            </td>
            <td>
                <b>
                    fix(common,agent,api-server): Improve log formats
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch improves the log formats as follows:
- Change the formats from 'simple' to 'json'
- Improve readability of submitTransaction() error messages

Signed-off-by: Tatsuya Sato <tatsuya.sato.so@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-16 06:30:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/16" class=".btn">#16</a>
            </td>
            <td>
                <b>
                    Add voting config option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch adds a voting configuration option for chaincode_ops.
This allows OpsSC users to configure the maximum number of malicious organizations (`f`) in the voting process.

- If the option is set, 2f + 1 is required to judge a proposal get `Approved`.
- If the option is not set, a majority of all participating organizations is required to judge a proposal get `Approved`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-14 11:23:01 +0000 UTC
    </div>
</div>

