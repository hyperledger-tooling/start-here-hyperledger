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
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/157" class=".btn">#157</a>
            </td>
            <td>
                <b>
                    Update Go bindings build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Go publish step is not currently deleting files, which it should
e.g. the now unused .whitelist file in fabric-protos-go

The repos used to publish the Go bindings should not have issue
tracking turned on so adding GitHub settings.yml file to make sure
the correct settings stay in place

Also merged the two Go workflows into one to remove some of the
duplication

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-18 18:24:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/156" class=".btn">#156</a>
            </td>
            <td>
                <b>
                    Bump version to 0.3.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also add missing maven link to RELEASING.md

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
        Created At 2022-11-18 14:20:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/153" class=".btn">#153</a>
            </td>
            <td>
                <b>
                    Prepare 0.3.0 release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also updates RELEASING.md with latest instructions

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
        Created At 2022-11-17 13:57:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/152" class=".btn">#152</a>
            </td>
            <td>
                <b>
                    Fix installDeployKey.sh
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Remove illegal option -o pipefail

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
        Created At 2022-11-17 12:50:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/151" class=".btn">#151</a>
            </td>
            <td>
                <b>
                    Ensure build fails if deploy key is not installed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
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
        Created At 2022-11-17 10:01:07 +0000 UTC
    </div>
</div>

