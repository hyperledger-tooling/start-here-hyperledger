---
layout: default
title: besu
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    22.7.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.7.0
                </span>
            </td>
            <td>
                ### Release Notes
22.7.0 is our Quarterly release with some big fixes over the previous 22.4.4. This is a recommended update for all users on public networks and those using Bonsai. This release also make many improvements to underlying peering code for better peering on public networks. There are a number of fixes around Merge-related code and the robustness of Besu as a whole.

With the stability of Bonsai in 22.7.0 and some planned optimizations, we are anticipating changing it to the default storage format at some point in the future. We will have more to share on this in the coming months, but nothing more at this time.

This update also includes tweaks and optimizations for memory management, RocksDB, peering default values, and more. See the changelog below and in the last few release candidates for more details.

### Bug Fixes

- Empty headers are now accepted correctly (per Ethereum p2p Spec) when in a range of headers #4189 
- Transaction handling will now function correctly when the TTD boundary has been crossed in a Merged network (used to require a restart) #4186 
- Pandas will now only print once when Merging, not on every startup (sorry panda fans) #4194 
- Fix for ENR request order handling when peering #4179 

### Optimizations, Features, & Improvements

- New flag (`--engine-rpc-enabled`) for forcing the Engine API to be present on a network with no TTD set #4190 
- Upgrade to Gradle 7.5 #4196 
- Upgrade spotless to 6.8.0 #4195 
- Changes to peer handling with DNS peers for peering improvements #4178

**Download links**
- https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.7.0/besu-22.7.0.tar.gz / sha256: `af21104a880c37706b660aa816e1c38b2b3f603a97420ddcbc889324b71aa50e`
- https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.7.0/besu-22.7.0.zip / sha256: `5b1586362e6e739c206c25224bb753a372bad70c0b22dbe091f9253024ebdc45`
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/22.7.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-08-03 16:31:28 +0000 UTC
    </span>
</div>

