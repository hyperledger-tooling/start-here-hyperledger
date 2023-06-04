---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2253" class=".btn">#2253</a>
            </td>
            <td>
                <b>
                    1.0.0-rc2 Updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @WadeBarnes -- advice needed.

With this PR, we update the "version.py" and "openapi" versions to "1.0.0-rc2", which I don't we want to leave in place.

Here are some things we can do:

- After this PR is merged, add another that changes the "main" branch version to what it usually is -- "0.8.1" (the last released version).  That's the state we are usually in between releases.
   - Side Issue: Should we change this practice and after a release, change the version references in the code to what we expect the next release to be -- e.g. "0.8.2-latest" or something like that.
- Merge this PR into a new branch "1.0.0" and we use that for future "1.0.0-rcX" tags.  As part of making subsequent 1.0.0-rcX tags, we merge main into the 1.0.0 branch.  That means that 1.0.0 is a clone of main for tags, updated with the types of changes that are in this PR.

I kind of lean towards the "1.0.0" branch, but you know this stuff way better than I.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-01 23:16:47 +0000 UTC
    </div>
</div>

