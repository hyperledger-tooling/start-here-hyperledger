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
                PR <a href="https://github.com/hyperledger/fabric/pull/3349" class=".btn">#3349</a>
            </td>
            <td>
                <b>
                    Additional TLS troubleshooting information (backport #3346)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3346 done by [Mergify](https://mergify.com).


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
        Created At 2022-04-22 11:58:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3348" class=".btn">#3348</a>
            </td>
            <td>
                <b>
                    Additional TLS troubleshooting information (backport #3346)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3346 done by [Mergify](https://mergify.com).


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
        Created At 2022-04-22 11:58:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3347" class=".btn">#3347</a>
            </td>
            <td>
                <b>
                    Additional TLS troubleshooting information (backport #3346)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3346 done by [Mergify](https://mergify.com).


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
        Created At 2022-04-22 11:58:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3346" class=".btn">#3346</a>
            </td>
            <td>
                <b>
                    Additional TLS troubleshooting information
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add additional TLS troubleshooting information to the TLS doc.
Also remove outdated information about Fabric v1.1.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 21:53:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3344" class=".btn">#3344</a>
            </td>
            <td>
                <b>
                    Replace inclusive language statement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Replace the existing inclusive language statement in the Fabric
doc contribution guide with the inclusive language statement recommended by Hyperledger TSC.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 04:33:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3343" class=".btn">#3343</a>
            </td>
            <td>
                <b>
                    Add ed25519 support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- New feature

#### Description

Due to some considering NIST curves insecure and
Golang having ed25519 native support, there was
not a reason for not implementing in Fabric.

Tests cases for ed25519 were also added. Since
ed25519 key derivation is not called by any
function, I left as a TODO.

As I am working on ed25519 support for node fabric-gateway,
I needed to add ed25519 support for cryptogen also,
aiming to pass tests with certificates containing
ed25519 keys. Since the node fabric-gateway tests
generate their crypto material with cryptogen, I
adapted cryptogen to support ed25519 keys.

#### Additional details

Some tests concerning ed25519 key generation and certificate parsing
were added.

#### Related issues

<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 18:08:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3339" class=".btn">#3339</a>
            </td>
            <td>
                <b>
                    Log warning for a non existent block delivery failure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

Improve error message when delivery service is asked for a block that doesn't yet exist on the node to make it more clear for users or support personnel.

#### Related issues
Fixes https://github.com/hyperledger/fabric/issues/3320


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-18 13:46:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3338" class=".btn">#3338</a>
            </td>
            <td>
                <b>
                    Updated dockerfile with new build arg
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Bug fix

#### Description

Added a new arg to pass in machine architecture details

#### Related issues

#3337 


Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-18 13:17:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3335" class=".btn">#3335</a>
            </td>
            <td>
                <b>
                    Handle empty policies when traversing the policy tree in discovery policy analysis (backport #3334)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3334 done by [Mergify](https://mergify.com).


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
        Created At 2022-04-18 10:17:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3334" class=".btn">#3334</a>
            </td>
            <td>
                <b>
                    Handle empty policies when traversing the policy tree in discovery policy analysis
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Discovery policy analysis engine assumed that the inner policy passed to it is of the correct type and cannot be empty.
Added a nil check and a test.

Change-Id: Ia6eaf0211d8d9f4b7f2881547934dc32c725a458
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-18 08:31:01 +0000 UTC
    </div>
</div>

