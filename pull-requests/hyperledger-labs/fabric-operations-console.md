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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/465" class=".btn">#465</a>
            </td>
            <td>
                <b>
                    fix safe URL vaildation for legacy field "caport"
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
The safe-url validation code was not working correctly if the legacy field `caport` was used. This only effects the `/v2/` APIs.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 21:04:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/464" class=".btn">#464</a>
            </td>
            <td>
                <b>
                    fixes orderer details panel not loading b/c bad id
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
Fixed the id error on the orderer details page.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-01 16:49:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/463" class=".btn">#463</a>
            </td>
            <td>
                <b>
                    sync component data after fabric upgrade
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
When upgrading fabric, new features might become available. we need to sync the component data after a fabric upgrade.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-28 20:23:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/462" class=".btn">#462</a>
            </td>
            <td>
                <b>
                    fix doc links for different console builds
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
- Fix links to console documentation that were dependent on what type of console build it was.
- removed some dead code


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-28 20:14:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/461" class=".btn">#461</a>
            </td>
            <td>
                <b>
                    Adds new fields to component data to replace the "location" field
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
Add new fields to indicate what type of console deployed a component, what type of cluster is hosting the component, and an explicit field to indicate if the component was imported to the console or not.  These fields replace the `location` data field, which became a mess from trying to do 3 separate jobs.

fields:
- `location` - this is now legacy
- `imported` - boolean - true if the console imported this peer/orderer/ca/msp, else false. 
- `cluster_type` - string - indicates if the cluster hosting the peer/orderer/ca is regular kubernetes, openshift, etc ("k8s", "openshift")
- `console_type` - string - indicates what type of console build created this component ("hlfoc", "ibp", "support", or "software")


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-27 18:50:15 +0000 UTC
    </div>
</div>

