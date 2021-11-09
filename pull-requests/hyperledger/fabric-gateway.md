---
layout: default
title: fabric-gateway
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway
---

# fabric-gateway <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/305" class=".btn">#305</a>
            </td>
            <td>
                <b>
                    Additional node module information
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 14:49:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/304" class=".btn">#304</a>
            </td>
            <td>
                <b>
                    More specific errors in Node API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add EndorseError, SubmitError and CommitStatusError to better differentiate the point in the submit flow where a failure occurs.

Contributes to #302 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 14:30:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/300" class=".btn">#300</a>
            </td>
            <td>
                <b>
                    Simplify off-line signing flow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Locate all methods for creating signed objects on the Gateway object, removing the need for client code to remember the network or contract used to create the unsigned objects.

Closes #301 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 21:20:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/299" class=".btn">#299</a>
            </td>
            <td>
                <b>
                    Bump version to 0.1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 15:42:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/298" class=".btn">#298</a>
            </td>
            <td>
                <b>
                    Use ECMAScript private methods instead of TypeScript private modifiers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We already use ECMAScript private fields for properties so this just extends it for methods too. This provides hard privacy and prevents plain JavaScript applications from accidentally using internal methods that may change and break them in the future.

Closes #254 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 14:40:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/297" class=".btn">#297</a>
            </td>
            <td>
                <b>
                    Fix CI version check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 11:43:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/296" class=".btn">#296</a>
            </td>
            <td>
                <b>
                    Remove support for Node 12
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move to Node 14 as the minimum supported Node version.

Closes #288 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 11:29:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/295" class=".btn">#295</a>
            </td>
            <td>
                <b>
                    Add tags trigger to CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-05 09:36:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/290" class=".btn">#290</a>
            </td>
            <td>
                <b>
                    Update Java and Node versions used in CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 13:01:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/287" class=".btn">#287</a>
            </td>
            <td>
                <b>
                    Make fine-grained Go API usable without explicit context handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use default contexts throughout the Go API, except for chaincode events, which requires an explicit context for cancellation. This avoids requiring the burden of context management for the client application. Added ...WithContext() alternatives to finer-grained calls to allow a context to be specified if desired.

Also fixes a build break in Node linting when we picked up new type definitions for a dependency.

Closes #198 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 10:42:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/286" class=".btn">#286</a>
            </td>
            <td>
                <b>
                    Update CI to publish on tagged releases
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 10:29:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/285" class=".btn">#285</a>
            </td>
            <td>
                <b>
                    Reinstate nightly publishing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Old node module has been deprecated so can remove that step from ci and
switch back to nightly publishing

Signed-off-by: James Taylor <jamest@uk.ibm.com>

Contributes to #209 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 18:06:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/284" class=".btn">#284</a>
            </td>
            <td>
                <b>
                    Deprecate old node module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previous deprecation failed with `422 Unprocessable Entity` which should be
fixed in npm v7

Signed-off-by: James Taylor <jamest@uk.ibm.com>

Contributes to #209 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 17:14:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/283" class=".btn">#283</a>
            </td>
            <td>
                <b>
                    Rename node module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rename fabric-gateway module to scoped @hyperledger/fabric-gateway

Also deprecates existing published fabric-gateway module

Signed-off-by: James Taylor <jamest@uk.ibm.com>

Contributes to #209 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 16:08:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/281" class=".btn">#281</a>
            </td>
            <td>
                <b>
                    Default gRPC call timeouts for Go API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Updated samples to demonstrate setting default timeouts.
- Removed async submit example for HSM samples since this duplicates main samples and keeping them simple makes it easier to see the HSM-specific aspects.

Contributes to #198 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 15:52:29 +0000 UTC
    </div>
</div>

