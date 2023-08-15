---
layout: default
title: anoncreds-rs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-rs
---

# anoncreds-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/232" class=".btn">#232</a>
            </td>
            <td>
                <b>
                    Hashmap uniformization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is somewhat of a continuation to the discussion in #228 . 

It allows both FFI and native code to use the services API in an organic manner through the use of generics, particularly referring to instances where there are containers of references in FFI, but in native code the container would be over owned types.

Also, the first commit simplifies the `TailsFileReader`; some lints were getting triggered and I figured I might as well do that while I was at it. If it's a problem to have both of these things in the same PR I can create a separate one for the first commit and cherry-pick the others in a separate PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-15 16:23:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/231" class=".btn">#231</a>
            </td>
            <td>
                <b>
                    fix: JS wrapper updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some updates to JavaScript wrappers to match main `branch` status:

- update React Native wrapper to match changes merged after #226. It also fixes an error in `UpdateRevocationStatusList` for NodeJS
- update both NodeJs and React Native according to #229. In that PR I've seen that `FfiCredRevInfo` structure has not been changed, even if `tails_path` is not used anymore. @andrewwhitehead is this on purpose or should be removed from there as well?

I went a bit more further and updated minimum node version to 18, which is in fact the minimum _usable_ version due to the known performance issue of `ref-napi` (which is patched). node 16 will reach its EOL next month anyway.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-12 21:24:23 +0000 UTC
    </div>
</div>

