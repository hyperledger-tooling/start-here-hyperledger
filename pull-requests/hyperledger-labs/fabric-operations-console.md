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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/294" class=".btn">#294</a>
            </td>
            <td>
                <b>
                    Various fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
- fix the policy error on the review step of the create wizard if multiple orderer orgs were selected
- fix graphic/image sizes (the size changed due to differences between esbuild and react-scripts)
- fix button widths, prevent overlap


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-09 20:20:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/293" class=".btn">#293</a>
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
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description
Updated release notes.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 20:33:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/292" class=".btn">#292</a>
            </td>
            <td>
                <b>
                    fix back buttons on create channel wizard
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

- Bug fix

#### Description
Some back buttons on the create wizard would put the user on the wrong step.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 19:49:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/291" class=".btn">#291</a>
            </td>
            <td>
                <b>
                    fix svg images to work with the esbuild svg plugin
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

- Bug fix

#### Description
The new esbuild builder broke most of the svg images. This fixes our svg files to be compatible.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 19:33:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/290" class=".btn">#290</a>
            </td>
            <td>
                <b>
                    fix channel list when single orderer is selected
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

- Bug fix

#### Description
Fix the channel tiles when a single orderer is selected. (drill down)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 18:17:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/288" class=".btn">#288</a>
            </td>
            <td>
                <b>
                    Add empty state to orderer drilldown
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
- add empty channel state text/img on drill down from orderer cluster tile if there are no channels


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-05 20:17:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/286" class=".btn">#286</a>
            </td>
            <td>
                <b>
                    Replace react-scripts with esbuild
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (improvement to code, performance, etc)

#### Description
Due to security concerns, painfully slow updates, slow build times, broken caching/chunking features and other headaches, I've ditched `react-scripts` and replaced it with `esbuild`. Building the project can still be done with `npm run build`, but be sure to install/update your environment with the new dependencies that this PR brings. Use `npm ci` to install.


- build times are drastically reduced! 
  - react-scripts-> 5 minutes, 48 seconds
  - esbuild -> 22 seconds



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-04 20:19:59 +0000 UTC
    </div>
</div>

