---
layout: default
title: fabric-operations-console
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operations-console
---

# fabric-operations-console <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operations-console){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/108" class=".btn">#108</a>
            </td>
            <td>
                <b>
                    lint code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement 

#### Description
- linted code based on es lint rules

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-14 20:34:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/107" class=".btn">#107</a>
            </td>
            <td>
                <b>
                    use the same major and minor versions for upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

- use the same major and minor versions for upgrade

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-14 20:16:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/106" class=".btn">#106</a>
            </td>
            <td>
                <b>
                    add react route for exporting identities via link
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

- New feature

#### Description
adds a route to download the identities. visiting `/export-identities` will immediately prompt for a local download of your wallet.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-13 21:38:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/105" class=".btn">#105</a>
            </td>
            <td>
                <b>
                    update release notes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                updating release notes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 19:07:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/104" class=".btn">#104</a>
            </td>
            <td>
                <b>
                    fix version compare logic with double digit str
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
The version comparison logic did not work correctly when comparing 1 double digit version to a single digit version.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 18:56:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/103" class=".btn">#103</a>
            </td>
            <td>
                <b>
                    1208-releasenotes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- release notes

#### Description
- updated release notes


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 21:55:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/102" class=".btn">#102</a>
            </td>
            <td>
                <b>
                    Auto upgrade version fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Bug fix

#### Description
- the auto upgrade fabric logic was upgrading from versions that were okay. it was upgrading all orderers to the highest available major fabric version, unless they were already at the highest level (within the same major version).


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 18:59:15 +0000 UTC
    </div>
</div>

