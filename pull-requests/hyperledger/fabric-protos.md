---
layout: default
title: fabric-protos
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-protos
---

# fabric-protos <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-protos){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/149" class=".btn">#149</a>
            </td>
            <td>
                <b>
                    smartbft configuration protobuf message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                added configuration options for smartbft consenter

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-09 11:49:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/148" class=".btn">#148</a>
            </td>
            <td>
                <b>
                    Fix Go bindings workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Moved FABRIC_PROTOS_GO_APIV2_DEPLOY_KEY env to the correct step

Signed-off-by: James Taylor <jamest@uk.ibm.com>

<!--- IMPORTANT: DO NOT modify or disable lint rules without agreeing changes in an issue first! -->
<!--- Any changes to lint rules and breaking change detection should be made in a separate pull  -->
<!--- request with an associated issue.                                                          -->
<!--- Please include a link to the issue in the pull request and DO NOT adjust lint rules to fix -->
<!--- build breaks when submitting any other pull requests.                                      -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-07 14:05:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/147" class=".btn">#147</a>
            </td>
            <td>
                <b>
                    Revert to using FABRIC_PROTOS_GO_APIV2_DEPLOY_KEY
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The last successfull push to fabric-protos-go-apiv2 was before the update to the PUBLISH_GO_V2 secret so switching back to FABRIC_PROTOS_GO_APIV2_DEPLOY_KEY

Also moved the deploy key setup to a seperate step which should hopefully fix the apiv2 tagging

Signed-off-by: James Taylor <jamest@uk.ibm.com>

<!--- IMPORTANT: DO NOT modify or disable lint rules without agreeing changes in an issue first! -->
<!--- Any changes to lint rules and breaking change detection should be made in a separate pull  -->
<!--- request with an associated issue.                                                          -->
<!--- Please include a link to the issue in the pull request and DO NOT adjust lint rules to fix -->
<!--- build breaks when submitting any other pull requests.                                      -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-07 12:08:54 +0000 UTC
    </div>
</div>

