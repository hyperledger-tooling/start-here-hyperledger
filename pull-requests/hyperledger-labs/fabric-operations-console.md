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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/428" class=".btn">#428</a>
            </td>
            <td>
                <b>
                    Fix safelist port
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
Fixes the unsafe url error from the new safe-url validation when creating a peer or os. the port and hostname are in separate fields in this api and had to be combined to pass validation .


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 17:13:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/427" class=".btn">#427</a>
            </td>
            <td>
                <b>
                    Pen test Input Validation update
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
<!--- Describe your changes in detail, including motivation. -->
Pen test Input Validation update

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 12:06:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/426" class=".btn">#426</a>
            </td>
            <td>
                <b>
                    update activity tracker doc
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
Update the doc on activity tracker and allow it to be turned on* via the setting.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 20:22:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/425" class=".btn">#425</a>
            </td>
            <td>
                <b>
                    pen test CSP Header updation
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

pen test CSP Header updation


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-28 12:17:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/424" class=".btn">#424</a>
            </td>
            <td>
                <b>
                    the safe list now records/vaildates ports too
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
Security improvement, instead of only validating the hostname is known when performing proxy requests, we will now validate that the hostname and port are known.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 20:46:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/423" class=".btn">#423</a>
            </td>
            <td>
                <b>
                    don't return sso error in response on failed login
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
Hides the details of a sso login failure from surfacing on the UI. the error is still logged. this was recommended by our pentesters.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-23 19:47:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/422" class=".btn">#422</a>
            </td>
            <td>
                <b>
                    make the backend validate email & clean up frontend
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
- adds basic email validation on api that changes contact email address
- switches front end code to use v3 api on settings edit
- removes redundant code


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-23 19:13:20 +0000 UTC
    </div>
</div>

