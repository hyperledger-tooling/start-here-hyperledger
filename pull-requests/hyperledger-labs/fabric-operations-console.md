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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/451" class=".btn">#451</a>
            </td>
            <td>
                <b>
                    limit length of text in channel tile
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
 - cuts off the orderer names on channel tiles if they are over 42 characters. Full names can still be viewed in the table layout.
 - updates release notes


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 16:15:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/449" class=".btn">#449</a>
            </td>
            <td>
                <b>
                    fix associate orderer modal regression
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
Fixes the associate identity with orderer modal bug introduced in build -40. The identity drop down was not loading.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 14:39:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/448" class=".btn">#448</a>
            </td>
            <td>
                <b>
                    decompress component docs during migration to edit
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
During migration the  component documents need to be decompressed so we can actually edit the docs. New fields get added.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 22:35:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/447" class=".btn">#447</a>
            </td>
            <td>
                <b>
                    Fix NodeRestApi lib performance
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
More speed/network improvements to minimize requests made by the front end.
- removed the function that calls the get-ALL-component-details api over and over for 1 component
- hooked up the skip cache param in more places
- can now filter multiple node types at once, so you don't have to call get-all-components multiple times when multiple component types are requested
- now absorbs any deployer error if the API asks for `deployment_attrs` on a component, but it was unable to get them, AND cached responses were not allowed (the error is still logged, but the api no longer returns a error response w/503 code)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 19:31:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/446" class=".btn">#446</a>
            </td>
            <td>
                <b>
                    fix join peer to channel regression
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
- Doc update

#### Description
- Fixes the client side error when joining a peer to a channel introduced in build -40.
- adds new client side timeout
- updates stitch documentation from changes added by build -40


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 16:03:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/445" class=".btn">#445</a>
            </td>
            <td>
                <b>
                    fix react warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Lint fix

#### Description
Just some react warnings I noticed.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 00:51:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/444" class=".btn">#444</a>
            </td>
            <td>
                <b>
                    fix blank cluster type
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
Cluster types were sometimes blank.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 00:02:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/443" class=".btn">#443</a>
            </td>
            <td>
                <b>
                    fix logic on orderer modals, speed improvement
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
- Improvement (improvement to code, performance, etc)

#### Description

lots of performance improvements that are mainly on the orderer modals (the side panel when viewing an orderer), but these changes will bleed over to other pages as well.

- fixed a race condition + nearly infinite loop where page spins getting the fabric version over and over, it would eventually settle after hundreds of requests
- parallelize getting root certs from CAs
- removed redundant API calls getting component details over and over
- removed the recursive behavior on the get-component-details function
- on the orderer modal, it now only calls APIs for functions that are needed for the particular modal function that was opened
- when walking the system channel to discover channel's (for the delete orderer-modal), it will now reuse the socket with the orderer and fetch the blocks in sequence, instead of opening and closing a socket for each block

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-11 23:03:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/442" class=".btn">#442</a>
            </td>
            <td>
                <b>
                    add migration field on existing components
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
Add migration field to components on the original console.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-10 20:05:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/441" class=".btn">#441</a>
            </td>
            <td>
                <b>
                    conform "\"k8s\"" to "k8s" in cluster type api
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
Better parsing on the cluster type api to handle double quotes around the cluster type value. So this converts ` "\"k8s\""` to simply `"k8s"`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-10 19:38:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/440" class=".btn">#440</a>
            </td>
            <td>
                <b>
                    Fix timeouts & streamline requests
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
- conformed client timeouts to be used consistently, filled in some fabric calls that did not have custom timeouts
  - some timeout values for certain http requests have changed
- when checking a OS cluster for channel participation apis (aka osn admin features), the requests will now be sent in parallel 
- avoids sending back a 408 http code to the browser to prevent automatic retries, uses 504 instead
  - this dramatically improves performance on requests to non responsive endpoints
- lowered the number of retries for component status call requests
- increased the number of retries for component status call requests when components have just been created
- increased the interval on the client logs to store them less often, to minimize traffic

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-07 20:02:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/439" class=".btn">#439</a>
            </td>
            <td>
                <b>
                    fix node ou parsing
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
The node ou parsing was not consistent. Sometimes the code expected a string, other times boolean. Added a helper function to conform and handle both cases.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-07 16:17:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/438" class=".btn">#438</a>
            </td>
            <td>
                <b>
                    decompress docs before migration edits settings
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
The migration code that edits the settings doc prior to migration needs to decompress the backup data first. otherwise the edits do not happen and the new console is thrown into shenanigans. 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-06 19:14:47 +0000 UTC
    </div>
</div>

