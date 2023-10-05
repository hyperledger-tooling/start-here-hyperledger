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
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/195" class=".btn">#195</a>
            </td>
            <td>
                <b>
                    Bump version to v0.3.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump version to v0.3.2 for future release.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-29 15:44:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/194" class=".btn">#194</a>
            </td>
            <td>
                <b>
                    Update releasing.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add details about npm tagging per release branch,
thanks to @bestbeforetoday.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-29 15:38:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/193" class=".btn">#193</a>
            </td>
            <td>
                <b>
                    Tag NPM packages from 0.1.x branch as either v1-latest or v1-unstable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Pushed commits to the main branch published NPM packages tagged as `unstable`, and release tags on the main branch published NPM packaged tagged as `latest`. This conflicted with NPM packages published from the 0.2.x branch and meant that the target Fabric version for the NPM package currently tagged `latest` varied depending on which branch had a release created most recently. The `latest` tag should always correspond to the current Fabric LTS release since it is the default version installed if a specific version is not specified.

Also update .gitignore to exclude files that should not be checked in.

Contributes to #191

<!--- IMPORTANT: DO NOT modify or disable lint rules without agreeing changes in an issue first! -->
<!--- Any changes to lint rules and breaking change detection should be made in a separate pull  -->
<!--- request with an associated issue.                                                          -->
<!--- Please include a link to the issue in the pull request and DO NOT adjust lint rules to fix -->
<!--- build breaks when submitting any other pull requests.                                      -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-29 09:44:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/192" class=".btn">#192</a>
            </td>
            <td>
                <b>
                    Tag NPM packages from main branch as either next or next-unstable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Pushed commits to the main branch published NPM packages tagged as `unstable`, and release tags on the main branch published NPM packaged tagged as `latest`. This conflicted with NPM packages published from the 0.2.x branch and meant that the target Fabric version for the NPM package currently tagged `latest` varied depending on which branch had a release created most recently. The `latest` tag should always correspond to the current Fabric LTS release since it is the default version installed if a specific version is not specified.

Closes #191

<!--- IMPORTANT: DO NOT modify or disable lint rules without agreeing changes in an issue first! -->
<!--- Any changes to lint rules and breaking change detection should be made in a separate pull  -->
<!--- request with an associated issue.                                                          -->
<!--- Please include a link to the issue in the pull request and DO NOT adjust lint rules to fix -->
<!--- build breaks when submitting any other pull requests.                                      -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-29 09:38:33 +0000 UTC
    </div>
</div>

