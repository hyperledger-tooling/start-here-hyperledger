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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/189" class=".btn">#189</a>
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
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description
Updated release notes


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-22 14:19:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/188" class=".btn">#188</a>
            </td>
            <td>
                <b>
                    change version to fabric version
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
More consistent text...


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-22 13:29:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/187" class=".btn">#187</a>
            </td>
            <td>
                <b>
                    Apollo test case fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ketul Shah <shah.ketul@ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Test update

#### Description
<!--- Describe your changes in detail, including motivation. -->
1 - Updated login feature file to login with automation user set in parameter
2 - Updated scenario to select Fabric Version with matching text instead of exact matching the version
3 - Added new step definition for above two points
4 - Added logging statement in login functions for pipeline execution troubleshooting for prod
5 - Added automation default password parameter in protractor.conf file


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-22 13:24:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/186" class=".btn">#186</a>
            </td>
            <td>
                <b>
                    allow editing the "ledger" fabric yml config_override field
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

- New feature

#### Description
Allow editing the `ledger` config field in a peer config yaml.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 23:28:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/185" class=".btn">#185</a>
            </td>
            <td>
                <b>
                    import orderers one by one
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
The old code was firing all the import orderer node reqs at once, this PR will send them one at a time.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 23:25:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/184" class=".btn">#184</a>
            </td>
            <td>
                <b>
                    fix merge logic - missing channel if the last node didnt have it
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Varad Ramamoorthy <varad@us.ibm.com>

- Bug fix

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 19:37:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/183" class=".btn">#183</a>
            </td>
            <td>
                <b>
                    Ask all nodes for aggregated channel list
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Bug fix
Query all nodes for the list of channels so that the Orderer Details shows consolidated channel list
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 18:09:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/182" class=".btn">#182</a>
            </td>
            <td>
                <b>
                    remove product label text selection logic via api
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
- this will fix the product label text on the login panel after resetting a password.
- instead of selecting from different label strings by waiting for an API response, we will just replace the string by editing the `messages.json` file when we build the front end


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 18:04:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/181" class=".btn">#181</a>
            </td>
            <td>
                <b>
                    Bump node v12 to v16
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
Moving from node v12 to node v16


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-18 18:23:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/180" class=".btn">#180</a>
            </td>
            <td>
                <b>
                    Create channel wizard osnadmin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature

#### Description
Extends create channel wizard to support channels via channel participation APIs using osnadmin features in Fabric.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-15 19:29:25 +0000 UTC
    </div>
</div>

