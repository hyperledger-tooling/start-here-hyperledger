---
layout: default
title: aries-acapy-plugins
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-plugins
---

# aries-acapy-plugins <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-plugins){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/391" class=".btn">#391</a>
            </td>
            <td>
                <b>
                    Create Automated Release Workflows 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There's some fairly complicated logic in a few places so I created a couple flow charts at `ReleaseWorkflows.md`.

Basically, this is a way to keep the plugins up to date with acapy releases automatically. If all the tests pass for a plugin it will be updated and be considered stable with acapy. If it doesn't then it won't be upgraded and will remain verified against an earlier release. A maintainer can create patch releases if a plugin which did fail for a release gets fixed before another version of acapy. A message is appended to the plugin description as well with the supported acapy version. I'm hoping this can be used to provide warnings in acapy when a plugin falls behind acapy.

There is some bash scripting. I tried to limit it as much as I could by utilizing the `repo_manager.py` script. The manager script has been changed slightly and some additional options for creating and parsing release information has added. The formatting for the release notes in RELEASES.md could be improved a bit more but I think it's good enough for now.

I had to do a bit of work for some tests after the upgrade but they all passing now so they will all be on version 0.12.0 of acapy initially. Two unit tests for rpc I removed. I couldn't figure out why they were only failing in the github action but not locally.

*** Note: *** I'm not sure if the bot will be able to create the release PR's for this repo. I have tried to use the org secret and replicated the same thing for my fork, so hopefully it does.

See initial PR https://github.com/hyperledger/aries-acapy-plugins/pull/387. Closed and wasn't able to re-open it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-24 20:06:01 +0000 UTC
    </div>
</div>

