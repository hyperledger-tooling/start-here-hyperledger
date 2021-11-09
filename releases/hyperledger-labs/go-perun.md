---
layout: default
title: go-perun
parent: Hyperledger Labs
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger-labs/go-perun
---

# go-perun <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/go-perun){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Hyperion
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.8.0
                </span>
            </td>
            <td>
                Reorg-resistance for the Ethereum backend and support for external Watchtowers.

### Added

- :sparkles: **Ethereum backend: Reorg resistance** #19: The Ethereum backend now lets the user specify after how many blocks a transaction or an event should be considered confirmed.
- :sparkles: **Watcher interface** #172: The watcher logic is now injectable. The adjudicator takes a watcher instance as a setup parameter. This enables using remote watcher services. A local watcher implementation is provided.

### Changed

- :arrow_up: Update go to v1.17 and go-ethereum to v1.10.12.
- :white_check_mark: Extend support for additional blockchain backends by revising the generic tests (e.g., #225, #227, #228).
- :children_crossing: Improve usability (e.g., #124, #144, #196, #204, #240).

### Fixed
- :bug: Improve stability (e.g., #129, #134, #148, #191, #207, #218).
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/go-perun/releases/tag/v0.8.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-11-09 13:06:10 +0000 UTC
    </span>
</div>

