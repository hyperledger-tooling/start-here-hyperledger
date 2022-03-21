---
layout: default
title: indy-vdr
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-vdr
---

# indy-vdr <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-vdr){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/85" class=".btn">#85</a>
            </td>
            <td>
                <b>
                    Feature/general indy resolver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Builds upon #80 

- Adds a VDR API with a general DID resolver. Network configuration can be taken from a Github Repo or a local folder structure
- Initial support for multiple ledgers and DID resolution with indy-vdr-proxy

The VDR API uses Async/Await and is therefore not suited for FFI, but I'll look into it.

I think it would help to create a `did-indy` branch to have smaller PRs at some point :) 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 16:32:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/84" class=".btn">#84</a>
            </td>
            <td>
                <b>
                    did:indy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Replaces #80 

## Support for additional optional fields in `nym` and `get_nym` requests
- `nym` request has optional `diddoc_content` field
- `get_nym` request has optional `seq_no` and `timestamp` fields
- Builder functions, ffi and wrappers are adapted accordingly
- Proxy allows `seq_no` and `timestamp` query params for `/nym` request

## Resolver
- Add resolver library with `PoolResolver` and `PoolRunnerResolver` (using callbacks for FFI)
- Add resolver to Python wrapper and test
- `PoolRunnerResolver` does not work with legacy resolution using attrib endpoint, since I can't get nested pool requests to work
- `PoolRunnerResolver` needs refactoring and proper error handling. I don't know how to handle/bubble up errors in closures  best

## Miscellaneous
- Removed `chrono` dependency in favor for `time-rs`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-15 11:06:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/83" class=".btn">#83</a>
            </td>
            <td>
                <b>
                    build: android and ios
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Previous PR was from the wrong branch

- Builds an xcframework based on static libraries for every architecture
- Builds an `libs` folder for Android containing every static libraries for every architecture

closes #77 

Signed-off-by: Berend Sliedrecht <berend@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-15 09:09:02 +0000 UTC
    </div>
</div>

