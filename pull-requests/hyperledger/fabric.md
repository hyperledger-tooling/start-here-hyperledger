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
                PR <a href="https://github.com/hyperledger/fabric/pull/4181" class=".btn">#4181</a>
            </td>
            <td>
                <b>
                    Add RELEASING.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                RELEASING.md describes the release process.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-25 20:48:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4178" class=".btn">#4178</a>
            </td>
            <td>
                <b>
                    Release commit for v2.2.11
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update release notes and doc for v2.2.11.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-21 15:48:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4177" class=".btn">#4177</a>
            </td>
            <td>
                <b>
                    Re-add Go to fabric-tools image (backport #4176)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4176 done by [Mergify](https://mergify.com).


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

Additionally, on Mergify [dashboard](https://dashboard.mergify.com) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-20 12:18:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4176" class=".btn">#4176</a>
            </td>
            <td>
                <b>
                    Re-add Go to fabric-tools image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since the images are no longer based on the golang alpine images, need to manually install go to the fabric-tools image. go is needed for users that use fabric-tools image to package go chaincodes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 19:06:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4175" class=".btn">#4175</a>
            </td>
            <td>
                <b>
                    Revert "Fix firewall warnings for integration tests on Mac"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit 412f3661cb05061a0a9413d16b24f5326f07b3fa.

The change caused integration tests to fail on a number of developer macs (both amd64 and arm64).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 14:33:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4174" class=".btn">#4174</a>
            </td>
            <td>
                <b>
                    Update dependencies (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update dependencies to match the known good levels in release-2.5. This will simplify maintenance and support between the two LTS releases and resolve vulnerability issues in these dependencies.

- github.com/docker/docker
- github.com/opencontainers/runc
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 14:16:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4173" class=".btn">#4173</a>
            </td>
            <td>
                <b>
                    Orderer v3: remove sys chan from registrar
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

Remove the system channel from the multichannel.Registrar

#### Related issues

#3515 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 14:04:38 +0000 UTC
    </div>
</div>

