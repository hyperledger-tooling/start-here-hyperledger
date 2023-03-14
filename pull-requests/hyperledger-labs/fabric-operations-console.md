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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/413" class=".btn">#413</a>
            </td>
            <td>
                <b>
                    fix password str validation on a dry-run request
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
- 
#### Description
Fixes password strength validation api if the request was a dry-run and the user does not exist. User does not need to exist for dry-run checks.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-13 19:16:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/412" class=".btn">#412</a>
            </td>
            <td>
                <b>
                    adding the multi instance warning on migration
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
Added migration warning text to the migration information panel.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-13 18:46:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/411" class=".btn">#411</a>
            </td>
            <td>
                <b>
                    handle req body size errors correctly
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
- bump request limit from 25MB to 100MB for fabric related apis
- adds logs when requests are terminated b/c of their size, actually it will log any body parser failure


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-10 20:31:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/410" class=".btn">#410</a>
            </td>
            <td>
                <b>
                    Allow saas consoles to test password strength
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
The test password strength api should work on saas consoles in prod.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-08 23:58:50 +0000 UTC
    </div>
</div>

