---
layout: default
title: indy-plenum
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-plenum
---

# indy-plenum <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-plenum){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1541" class=".btn">#1541</a>
            </td>
            <td>
                <b>
                    Publishing artifacts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements the publishing of the artifacts to the [JFrog Artifactory of Hyperledger.](https://hyperledger.jfrog.io/ui/repos/tree/General/indy).

The PR currently works for ubuntu 16.04 only.

A successful run of the GitHub action with publishing the artifacts to the JFrog Artifactory of Hyperledger can be found [here](https://github.com/udosson/indy-plenum/actions/runs/807114267).

An update of the Docker image was necessary to include `zstd` which is required to pass a cache created by a container to a job that natively runs on ubuntu.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 14:52:05 +0000 UTC
    </div>
</div>

