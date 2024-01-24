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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/597" class=".btn">#597</a>
            </td>
            <td>
                <b>
                    fix mutual tls reqs with axios http lib
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
- fixes https requests that require mutual tls. Such as the orderer's channel participation apis. These APIs were failing because our `request` module replacement, `axios`, was not sending the client side tls cert.

- fixes our error response handling of the channel participation api `getOSNChannel`. will now correctly indicate an error occured.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-24 18:17:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/596" class=".btn">#596</a>
            </td>
            <td>
                <b>
                    API key test cases from console
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Test update

#### Description
API key test cases from console

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-24 06:55:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/593" class=".btn">#593</a>
            </td>
            <td>
                <b>
                    bump release notes
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
update release notes


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-19 20:53:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/592" class=".btn">#592</a>
            </td>
            <td>
                <b>
                    prevent the axios wrapper from deleting body arg
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
- The axios wrapper introduced in `1.0.8-5` was copying the `body` filed to `data`, and then deleting `body`. The api would succeed, but later when the code tried to reference `body` it would have issues because it is now empty. This error would surface in the UI with newly created components having blank names/tiles. Other internal fields were also missing.
- also fixes some npm dependency cves


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-19 18:37:39 +0000 UTC
    </div>
</div>

