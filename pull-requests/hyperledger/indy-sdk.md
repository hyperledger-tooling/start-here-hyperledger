---
layout: default
title: indy-sdk
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-sdk
---

# indy-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2485" class=".btn">#2485</a>
            </td>
            <td>
                <b>
                    [#2484] Provide a Java version of the Getting Started Walkthrough
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
        Created At 2022-02-23 14:04:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2483" class=".btn">#2483</a>
            </td>
            <td>
                <b>
                    Fixes pip bootstrap error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The pipeline is failing in the build-image-python step.
Pip is complaining about the wrong url. 
```
 #6 [3/4] RUN curl -fsSL -o- https://bootstrap.pypa.io/pip/get-pip.py | python3.6
#6 sha256:ec08f7fc3ed30f11c7a36d067994d6e26242634d813008d8a05d9731c2997e56
#6 0.432 ERROR: This script does not work on Python 3.6 The minimum supported Python version is 3.7. Please use https://bootstrap.pypa.io/pip/3.6/get-pip.py instead.
#6 ERROR: executor failed running [/bin/sh -c curl -fsSL -o- https://bootstrap.pypa.io/pip/get-pip.py | python3.6]: exit code: 1
```
This PR should fix that.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-23 08:50:43 +0000 UTC
    </div>
</div>

