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
                PR <a href="https://github.com/hyperledger/fabric/pull/3701" class=".btn">#3701</a>
            </td>
            <td>
                <b>
                    Move inactive maintainers to emeritus status
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The TOC approved a requirement that maintainers
that have not been active in over three to six
months be move to emeritus status.

These maintainers have not been active in over
one year.

hyperledger/toc#32

Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-18 18:43:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3699" class=".btn">#3699</a>
            </td>
            <td>
                <b>
                    Use safe accessors for RWset protos (backport #3698)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3698 done by [Mergify](https://mergify.com).


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
        Created At 2022-10-17 17:22:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3698" class=".btn">#3698</a>
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

Backport of https://github.com/hyperledger/fabric/pull/3686 with modified unit test for different proto behaviour.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-17 15:34:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3697" class=".btn">#3697</a>
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

This is an alternative solution to the problem proposed in https://github.com/hyperledger/fabric/pull/3681

Signed-off-by: Fred Partanskiy <pfi79@mail.ru>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-15 15:06:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3696" class=".btn">#3696</a>
            </td>
            <td>
                <b>
                    Add delivery client logging (backport #3692 release-2.2)
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
        Created At 2022-10-15 15:06:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3694" class=".btn">#3694</a>
            </td>
            <td>
                <b>
                    Add delivery client logging (backport #3692 release-2.4)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3692 done by [Mergify](https://mergify.com).


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
        Created At 2022-10-15 14:05:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3693" class=".btn">#3693</a>
            </td>
            <td>
                <b>
                    Add delivery client logging (backport #3692 release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3692 done by [Mergify](https://mergify.com).


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
        Created At 2022-10-15 14:05:17 +0000 UTC
    </div>
</div>

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

