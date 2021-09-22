---
layout: default
title: business-partner-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/business-partner-agent
---

# business-partner-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/business-partner-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/629" class=".btn">#629</a>
            </td>
            <td>
                <b>
                    Feature/matching credential
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See #611

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/629"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 08:56:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/628" class=".btn">#628</a>
            </td>
            <td>
                <b>
                    delete old packages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/628"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 08:07:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/627" class=".btn">#627</a>
            </td>
            <td>
                <b>
                    Reset build.yml output tags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/627"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-21 16:03:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/626" class=".btn">#626</a>
            </td>
            <td>
                <b>
                    Update build.yml
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
        Created At 2021-09-21 15:47:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/625" class=".btn">#625</a>
            </td>
            <td>
                <b>
                    Update build.yml
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
        Created At 2021-09-21 15:37:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/624" class=".btn">#624</a>
            </td>
            <td>
                <b>
                    Option to set auto respond credential proposal flag to false
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
        Created At 2021-09-21 12:25:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/623" class=".btn">#623</a>
            </td>
            <td>
                <b>
                    Handle valid invitation type (didcomm)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `https://didcomm.org/connections/1.0/invitation` is a valid invitation type, so let's handle the current case and this value.
IBM had generated a connection invitation with the didcomm format and we couldn't connect, so we needed to update our invitation parser class.

We can generate invitations with the same `@type` by starting the agent with `--emit-new-didcomm-prefix` option.

fixes #620

Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/623"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 18:04:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/621" class=".btn">#621</a>
            </td>
            <td>
                <b>
                    Import Error Message - show backend message.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                400 was being handled in the frontend to always mean one error (Schema exists), but that hid other types of errors so message was misleading.

Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/621"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 00:51:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/619" class=".btn">#619</a>
            </td>
            <td>
                <b>
                    ternary instead of pipe
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jason Sy <jasyrotuck@gmail.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/619"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 22:41:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/618" class=".btn">#618</a>
            </td>
            <td>
                <b>
                    Expert Mode - Issue Credential from CSV
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allow user to copy/paste, type or upload a CSV file and load the credential data (first row only).
Further enhancement to the Expert Mode Load Credential data.
As noted by @etschelp, this is just a basic first step and we should further enhance for multi-credential load etc.

Signed-off-by: Jason Sherman <jsherman@parcsystems.ca>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/618"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 22:38:02 +0000 UTC
    </div>
</div>

