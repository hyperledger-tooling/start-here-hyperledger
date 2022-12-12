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
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/121" class=".btn">#121</a>
            </td>
            <td>
                <b>
                    refactor(javascript): better response type inference
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Small improvement to type response type inference for requests. Using the `infer` key we don't have to make the __responseType__ property public.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-12 12:02:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/119" class=".btn">#119</a>
            </td>
            <td>
                <b>
                    Update build actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update to node16-compatible versions of actions
- Use cargo-cross to build linux binaries
- Add linux/arm64 build
- Use Python 3.8 over 3.6 for testing (3.6 is no longer easily available)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-06 19:49:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-vdr/pull/118" class=".btn">#118</a>
            </td>
            <td>
                <b>
                    Add android build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Will build the android wrapper using cross
  - The default image used by cross has some issues so it has to be specified in the `Cross.toml` file that we use the `main` tag for every image.
- Will create an artifact called `android-jniLibs` (open for better naming), which is a combination of the architectures that are being created. Android uses this structure to have "one" package for every architecture.

Workflow has been tested, without the `publish-release` input. Result can be found here: https://github.com/blu3beri/indy-vdr/actions/runs/3628442119
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-06 10:29:07 +0000 UTC
    </div>
</div>

