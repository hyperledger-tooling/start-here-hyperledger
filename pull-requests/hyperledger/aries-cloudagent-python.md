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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2258" class=".btn">#2258</a>
            </td>
            <td>
                <b>
                    Updating Maintainers list to be accurate and using the TOC format
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-08 17:14:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2255" class=".btn">#2255</a>
            </td>
            <td>
                <b>
                    Resolve definitions.py fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Include searching by the module base package when resolving plugin definitions location.

Fixes #2224 

This still depends on the module package names and file system paths matching up, which is not guaranteed. But without adding additional configuration in the plugin registry, I think this is all we can do.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 22:56:19 +0000 UTC
    </div>
</div>

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

