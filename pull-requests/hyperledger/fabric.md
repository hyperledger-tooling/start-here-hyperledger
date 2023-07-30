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
                PR <a href="https://github.com/hyperledger/fabric/pull/4338" class=".btn">#4338</a>
            </td>
            <td>
                <b>
                    Update docs requirements to latest v1 Sphinx for dep vulnerabilities (backport #4337)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4337 done by [Mergify](https://mergify.com).


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
        Created At 2023-07-28 17:20:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4337" class=".btn">#4337</a>
            </td>
            <td>
                <b>
                    Update docs requirements to latest v1 Sphinx for dep vulnerabilities
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code, performance, etc)
- Documentation update

#### Description

Updates the version of Sphinx used to generate the Fabric Documentation to v7.1 from v1.8.2, which was released many years ago.  

**This is a new PR; the other one was getting messy.**

#### Additional details

Along the way, it addresses two security vulnerabilities that have been discovered for Pygments. I tested it by running `make docs` in my local clone of the fabric repo and then checking the resultant output using Chrome on my Mac laptop.  It looked identical to https://hyperledger-fabric.readthedocs.io/

#### Related issues

As per https://github.com/hyperledger/fabric/issues/4333.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-28 14:34:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4330" class=".btn">#4330</a>
            </td>
            <td>
                <b>
                    Remove ReplicationBackgroundRefrshInterval
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It's not used anymore.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-27 13:48:21 +0000 UTC
    </div>
</div>

