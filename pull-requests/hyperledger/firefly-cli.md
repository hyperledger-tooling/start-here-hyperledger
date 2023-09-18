---
layout: default
title: firefly-cli
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-cli
---

# firefly-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/259" class=".btn">#259</a>
            </td>
            <td>
                <b>
                    Separate build and release jobs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Apparently Goreleaser is now picky about doing builds against commits that don't match the tag that it's expecting. The version of Goreleaser that we're using was recently upgraded which caused this change. Previously, (I'm not sure why) we were running Goreleaser on every PR whether we were doing a release or not. This PR separates the jobs and just runs make on PRs and will run goreleaser anytime we tag a new release. This should unblock our PR backlog.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 17:04:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/257" class=".btn">#257</a>
            </td>
            <td>
                <b>
                    Adding FIREFLY_HOME env variable (optional)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-17 22:48:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/256" class=".btn">#256</a>
            </td>
            <td>
                <b>
                    Tobytobias
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-16 16:13:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/255" class=".btn">#255</a>
            </td>
            <td>
                <b>
                    Update MAINTAINERS.md and CODEOWNERS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-13 19:24:56 +0000 UTC
    </div>
</div>

