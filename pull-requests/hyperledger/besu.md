---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3330" class=".btn">#3330</a>
            </td>
            <td>
                <b>
                    21.10.9 update hashes to match regenerated artefacts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Besu CI pipeline was re-run on the same commit, generating the same artefact with a different hash

Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

See https://app.circleci.com/pipelines/github/hyperledger/besu?branch=release-21.10.x&filter=all 
^ looking at this - pipeline for commit 8f465c0 was run twice. 7 days ago and 2 days ago.
Since the commit is the same https://github.com/hyperledger/besu/commit/8f465c0faf568b395c8e271c6caff6f79d77a7a7
I'm updating the hashes.
Also ref https://github.com/hyperledger/homebrew-besu/pull/70

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 04:29:58 +0000 UTC
    </div>
</div>

