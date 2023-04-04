---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/790" class=".btn">#790</a>
            </td>
            <td>
                <b>
                    post_message migration [Issue #772]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves: Issue https://github.com/hyperledger/aries-vcx/issues/772 - Move out post_message to shared_vcx

###Short summary
-Migrated httpclient.rs file to shared_vcx directory
-The issue requested that the post_message() function be moved, but there were other items within httpclient.rs that post_message() depended upon.
-aries-vcx is successfully compiling with the changes provided.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 19:37:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/789" class=".btn">#789</a>
            </td>
            <td>
                <b>
                    Fix iOS wrapper, connectionHandle
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix in the iOS wrapper, connectionHandle parameter as Number* instead of VcxHandle
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 07:52:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/788" class=".btn">#788</a>
            </td>
            <td>
                <b>
                    CI: Read tag 'skip-ci' to skip majority of ci jobs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">skip-ci</span>
            </td>
            <td>
                - CI update: If `skip-ci` is present on pull request, expensive jobs are skipped (reduces total CPU time from ~4 hours to 40 min) and CI duration to 38 mins
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 08:00:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/787" class=".btn">#787</a>
            </td>
            <td>
                <b>
                    Refactor/replacing messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">skip-ci</span>
            </td>
            <td>
                Draft for the new `messages` crate integration.

Status:
    - [x] Integrated in `aries_vcx` - compiles
    - [x] Integrated in `libvcx` - compiles
    - [x] Integrated in the Rust agent - compiles.
    - [x] Integrated in the UniFFI wrapper - does not compile.
    - [x] Integrated in the napi-rs wrapper - compiles. 
    - [ ] Test backwards compatibility when aries_vcx is used for a server.
    - [ ] Test backwards compatibility when aries_vcx is used for a client.

#### UniFFI
The UniFFI wrapper doesn't compile because of a data type change in some parts of the code where instead of a `String` a `Url` is expected now. I tried to implement the `Url` in the UDL file, but it seems like adding an external type requires it's entire definition, as well as the definition of it's subtypes. And at some point, the `Url` depends on `std::net::Ipv4Addr` and `std::net::Ipv6Addr` which are wrappers over static arrays, which don't seem to be supported in UniFFI.

#### NOTE: 
This PR is simply to get rid of the old messages and implement the new ones. It's not performant, readable, or anything like that. I cut as many corners as I could because the real work will come with the `aries_vcx` and its state machines refactor. The goal here is to have things working as before, nothing more.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 14:16:45 +0000 UTC
    </div>
</div>

