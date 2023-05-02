---
layout: default
title: bevel-operator-fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/bevel-operator-fabric
---

# bevel-operator-fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/bevel-operator-fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel-operator-fabric/pull/165" class=".btn">#165</a>
            </td>
            <td>
                <b>
                    added k8s-gateway-api support 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--  Thanks for sending a pull request!
-->
#### What this PR does / why we need it:
#### Which issue(s) this PR fixes:
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #160`, or `Fixes https://github.com/hyperledger/bevel-operator-fabric/issues/160`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #160
#### Special notes for your reviewer:
@dviejokfs as discussed, have implemented gateway-api but have not removed istio support. Also , note that this feature does not cover the grpc proxy configuration yet that might be required by the fabric-operations console.But , everything else seems to be working fine
#### Does this PR introduce a user-facing change?
<!--
If no, just write "NONE" in the release-note block below.
If yes, a release note is required:
Enter your extended release note in the block below. If the PR requires additional action from users switching to the new release, include the string "action required".
-->
```release-note
Yes. k8s-gateway-api must be installed in the cluster and a GatewayClass must be configured beforehand.
```
#### Additional documentation, usage docs, etc.:
<!--
This section can be blank if this pull request does not require a release note.
When adding links which point to resources within git repositories, like
supporting documentation, please reference a specific commit and avoid
linking directly to the master branch. This ensures that links reference a
specific point in time, rather than a document that may change over time.
-->
```docs
Setup gateway-api:

https://gateway-api.sigs.k8s.io/guides/#installing-gateway-api

Install CRD's from the experimental channel from the link above

Follow any of the implementation given here in the doc and have a GatewayClass configured with  any proxy of your choice (Eg. traefik, istio etc)

https://gateway-api.sigs.k8s.io/implementations/
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-30 07:24:01 +0000 UTC
    </div>
</div>

