---
layout: default
title: ursa
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/ursa
---

# ursa <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/ursa){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/ursa/pull/216" class=".btn">#216</a>
            </td>
            <td>
                <b>
                    Added Github Actions pipeline
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Runs a CI pipeline for incoming PRs and merges to main.
  - audit
  - build
  - check
  - clippy
  - docs
  - format
  - tests
- Removed some files that I assumed are not used (please give this a careful review as I am not fully aware of the history of these files).
- Does not include the release to crates.io just yet.
- Moved the `ursa_` packages to an Ursa folder to keep the root a bit cleaner. They kept the `ursa_` prefix as we might want to release them as seperate packages, although some of them are empty.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-24 19:06:59 +0000 UTC
    </div>
</div>

