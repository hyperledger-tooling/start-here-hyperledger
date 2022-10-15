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
                PR <a href="https://github.com/hyperledger/fabric/pull/3692" class=".btn">#3692</a>
            </td>
            <td>
                <b>
                    Add delivery client logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add logging for delivery client connections to ordering service, as well as disconnections.
This will help with troubleshooting when connections between peer and orderer are in doubt.

Also improve related log messages and config descriptions.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-15 05:19:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3690" class=".btn">#3690</a>
            </td>
            <td>
                <b>
                    Revert "Remove an unused config parameter from peer"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It turns out the delivery client keepalive settings were still being used.
We need to revert the change in main branch and release-2.5 branch.

This reverts commit ccfa8a4a78f51e81bed877c8336e3de6141d3774.
Signed-off-by: David Enyeart enyeart@us.ibm.com

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-14 16:56:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3689" class=".btn">#3689</a>
            </td>
            <td>
                <b>
                    Revert "Remove an unused config parameter from peer"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It turns out the delivery client keepalive settings were still being used.
We need to revert the change in main branch and release-2.5 branch.

This reverts commit ccfa8a4a78f51e81bed877c8336e3de6141d3774.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-14 16:48:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3688" class=".btn">#3688</a>
            </td>
            <td>
                <b>
                    Use safe accessors for RWset protos (backport #3686)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3686 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-14 15:09:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3687" class=".btn">#3687</a>
            </td>
            <td>
                <b>
                    Use safe accessors for RWset protos (backport #3686)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3686 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-14 15:09:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3686" class=".btn">#3686</a>
            </td>
            <td>
                <b>
                    Use safe accessors for RWset protos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use the Getter functions rather than direct access to fields in the proto structures.

Resolves #3685 

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-13 08:40:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3681" class=".btn">#3681</a>
            </td>
            <td>
                <b>
                    Use env variables to initialize the PKCS11 BCCSP
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The environment variables to configure the PKCS11 BCCSP are ignored for the peer node, such as CORE_PEER_BCCSP_PKCS11_LIBRARY. This change allows specifying the BCCSP Default and to configure all of the PKCS11 BCCSP settings using environment variables.

Signed-off-by: Jonathan Patchell <Jonathan.Patchell@thalesgroup.com>

#### Type of change

- Bug fix

#### Description

When integrating the peer node with an HSM, it isn't possible to specify environment variables to configure the PKCS11 BCCSP. With these changes the environment variables are no longer ignored allowing configuration from environment variables for the  PKCS11 BCCSP.

#### Additional details

#### Related issues

#1900

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-11 19:46:34 +0000 UTC
    </div>
</div>

