---
layout: default
title: indy-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-node
---

# indy-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node/pull/1719" class=".btn">#1719</a>
            </td>
            <td>
                <b>
                    GHA Optimization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As discussed in #1693 this PR fixes the multiple installs in the test slices by moving the installation of the pip packages into the container build.
It als incorporates the #1716  in  the ubuntu20 branch.
As the container is special for a specific commit it is therefore tagged with the commit hash and deleted afterwards.
The script in the workflow folder is getting the package id from the container tag to delete it with api calls. 
The Linting can be moved outside of a container and therefore reducing the runtime.

Changes to remove_test_image job the need to be made to be used in the organiszation repo (the api calls need to be changed to fit the organisation not the user  part). 
But doing them now would fail the pipeline.
Will do that and sqash it after PR is approved.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-09 15:15:47 +0000 UTC
    </div>
</div>

