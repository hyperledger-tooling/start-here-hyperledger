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
                PR <a href="https://github.com/hyperledger/fabric/pull/3072" class=".btn">#3072</a>
            </td>
            <td>
                <b>
                    1121 peers e2e and gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

- Peers topic e3e edit for gateway, in detail, substantial.
- Minor updates to gateway overview since prior commit.
- Flow diagrams figure 6 and figure 10 are commented out for now - pending design update to reflect the associated text updates. 

#### Type of change

- New feature
- Documentation update

#### Description

Fabric Gateway service - new feature.

#### Related issues

https://github.com/hyperledger/fabric/issues/2807


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 22:37:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3070" class=".btn">#3070</a>
            </td>
            <td>
                <b>
                    goimports updates to prepare for Go 1.17
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Run goimports to make code compatible with Go 1.17.
The changes work with both Go 1.16 and Go 1.17, therefore it can be merged now.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-21 16:04:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3067" class=".btn">#3067</a>
            </td>
            <td>
                <b>
                    add http proxy support to core/chaincode/platforms
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: itaru2622 <itaru2622@gmail.com>

close #3066 

#### Type of change

- New feature

#### Description

add http proxy support to chaincode container build phase when fabric-peer container run with  "-e https_proxy=... " 
for details, refer #3066 

#### Additional details

when your devenv is located behind http proxy, additional no_proxy entries may be required to pass unit-test and integration-test.
the reasons is  described in #3066 and end of docs/sources/dev-setup/devenv.rst

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-21 08:05:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3065" class=".btn">#3065</a>
            </td>
            <td>
                <b>
                    Fix Issue #257 by including additional details on Kube Service routing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Type of change

- Documentation update

#### Description

This PR adds a brief summary of Kubernetes Service routing as a mechanism to implement basic HA / DR / connection load balancing to the Fabric Gateway. 

#### Additional details

A sample integration of the Kube routing is available in the Kubernetes Test Network [HA GUIDE](https://github.com/hyperledger/fabric-samples/blob/main/test-network-k8s/docs/HIGH_AVAILABILITY.md)

Kube test network updates to enable gateway client load balancing are available in [fabric-samples PR #532](https://github.com/hyperledger/fabric-samples/pull/532)
#### Related issues

Additional discussion, and the original issue, is tracked at [fabric-gateway issue #257](https://github.com/hyperledger/fabric-gateway/issues/257) 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 19:15:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3064" class=".btn">#3064</a>
            </td>
            <td>
                <b>
                    Reference current application APIs in peer event service docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Contributes to #2807 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 17:16:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3062" class=".btn">#3062</a>
            </td>
            <td>
                <b>
                    Remove redundant SDK documentation page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This page is out of date, duplicates information in sdk_chaincode.rst, and does not fit well in the architecture section.

Contributes to #2807 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 15:22:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3061" class=".btn">#3061</a>
            </td>
            <td>
                <b>
                    Log the transactionID in all log messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger/fabric-gateway/issues/303

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 13:29:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3060" class=".btn">#3060</a>
            </td>
            <td>
                <b>
                    Updates to endorser and gateway logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update endorser and gateway log levels to improve troubleshooting.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 21:07:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3059" class=".btn">#3059</a>
            </td>
            <td>
                <b>
                    Update protobuf definitions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Redundant `result` fields removed from gateway.EndorseResponse and gateway.PreparedTransaction.

Contributes to hyperledger/fabric-gateway#316
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 18:23:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3056" class=".btn">#3056</a>
            </td>
            <td>
                <b>
                    docs: fixing some typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update

#### Description

This change fixes some typos  in the docs

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 11:38:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3055" class=".btn">#3055</a>
            </td>
            <td>
                <b>
                    Use Heap To Maintain First Differences
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Julian Castrence <juliancastrence@ibm.com>

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (improvement to code, performance, etc)


#### Description

- Changed ledgerutil compare naive implementation of maintaining list of first differences to use heap implementation for better performance

<!--- Describe your changes in detail, including motivation. -->


<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->


<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

<!--
Checklist (DELETE AFTER READING):

- `Signed-off-by` added to commits (required for DCO check to pass)
- Tests have been added/updated (required for bug fixes and features)
- Unit and/or integration tests pass locally
- Run linters and checks locally using 'make checks'
- If change requires documentation updates, make updates in pull request,
  or open a separate issue and provide link
- Squash commits into a single commit, unless a stack of commits is
  intentional to assist reviewers or to preserve review comments.
- For additional contribution guidelines see the project's CONTRIBUTING.md file
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-17 23:15:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3051" class=".btn">#3051</a>
            </td>
            <td>
                <b>
                    Don't use EndorseResponse.Result field
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This duplicates information already held within the transaction envelope, and can cause failures on gRPC message size limit with large transaction results.
    
Also:
- nil out the ProposalResponse.Response.Payload field in EndorseResponse messages since, in the successful endorsement case, this is typically populated with a duplicate of the transaction result. This field is not required by the Fabric Gateway client and can cause gRPC message size limit failures.
- prefer the transaction result within the proposal response payload for EvaluateResponse messages since the Response.Payload in the proposal response is not required to be the transaction result and may instead contain metadata.

Contributes to hyperledger/fabric-gateway#316
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-17 15:36:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3050" class=".btn">#3050</a>
            </td>
            <td>
                <b>
                    Fix CI script syntax
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: Arnaud J Le Hors <lehors@us.ibm.com>

#### Type of change

- Bug fix

#### Description

Previous change made for Windows in PR #2991 introduced a syntax error which
this fixes.

#### Related issues

N.A.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-17 13:14:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3049" class=".btn">#3049</a>
            </td>
            <td>
                <b>
                    Add gateway ref to private data doc topic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Minor doc update.  Contributes to #2807 

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-16 14:41:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3048" class=".btn">#3048</a>
            </td>
            <td>
                <b>
                    Update Contract and Application API docs for Fabric Gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Contributes to #2807 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-16 11:05:02 +0000 UTC
    </div>
</div>

