---
layout: default
title: aries-askar
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-askar
---

# aries-askar <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-askar){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/204" class=".btn">#204</a>
            </td>
            <td>
                <b>
                    Add DB benchmark
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a benchmark using [`criterion`](https://github.com/bheisler/criterion.rs) to benchmark DB performance,
specifically when the DB has a large number of profiles/items/items_tags.

Benchmark is heavily based on `tests/store_key.rs`

Please feel free to be extremely pedantic (`-Wclippy::pedantic -Wclippy::nursery`)

Related to #195 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-17 09:07:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/202" class=".btn">#202</a>
            </td>
            <td>
                <b>
                    chore(js): update version to dev.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates the version of the JS wrappers for Askar to a new dev version.

I was a bit confused by the versions as the Python and Cargo versions were already set to 0.3, but no release was made yet. 

@andrewwhitehead are we good to make a release in the main branch for the Python and Rust binaries? Then we can merge this PR and release it, as this depends on the 0.3 library being released now


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-13 03:51:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/201" class=".btn">#201</a>
            </td>
            <td>
                <b>
                    Update python wrapper version to 0.3.0
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
        Created At 2023-11-11 01:02:38 +0000 UTC
    </div>
</div>

