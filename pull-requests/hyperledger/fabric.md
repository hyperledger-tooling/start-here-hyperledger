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
                PR <a href="https://github.com/hyperledger/fabric/pull/3822" class=".btn">#3822</a>
            </td>
            <td>
                <b>
                    Add V2_5 application capability to configtx.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add V2_5 application capability to configtx.yaml.

Resolves #3815 

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-30 22:43:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3821" class=".btn">#3821</a>
            </td>
            <td>
                <b>
                    Add purgeInterval to core.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Users that need to purge private data may want to purge more frequently that the default of every 100 blocks. Expose purgeInterval configuration setting in core.yaml.

Resolves #3816 

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-30 22:39:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3820" class=".btn">#3820</a>
            </td>
            <td>
                <b>
                    Private data purge logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add logging to record number of private data purges. This may be used as an audit log or for troubleshooting.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-30 22:31:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3819" class=".btn">#3819</a>
            </td>
            <td>
                <b>
                    [WIP] Update purge private data tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Check that no purged data appears in block event replays

Signed-off-by: James Taylor <jamest@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-30 17:14:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3813" class=".btn">#3813</a>
            </td>
            <td>
                <b>
                    [WIP] Update purge private data integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ensure previously purge private data can be recreated without being purged

Signed-off-by: James Taylor <jamest@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-29 17:35:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3810" class=".btn">#3810</a>
            </td>
            <td>
                <b>
                    Transfer leadership before submitting to raft library (backport #3651)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Improvement (improvement to code)

#### Description
Backport #3651 changes wrt leadership transfer

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>
Co-authored-by: Yacov Manevich <yacovm@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-26 12:00:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3808" class=".btn">#3808</a>
            </td>
            <td>
                <b>
                    [WIP] Update purge private data integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Test whether a new peer is able to reconcile from a purged peer

Signed-off-by: James Taylor <jamest@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-24 16:52:24 +0000 UTC
    </div>
</div>

