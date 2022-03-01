---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1882" class=".btn">#1882</a>
            </td>
            <td>
                <b>
                    chore: fix licenses
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These files are auto-generated with ISC as
the default licese. Switched to Apache 2

Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 16:15:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1880" class=".btn">#1880</a>
            </td>
            <td>
                <b>
                    docs(faq): add instructions to install in Apple M1 processor (ARM-based)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Description of the installation process for Apple M1 processors.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 12:57:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1879" class=".btn">#1879</a>
            </td>
            <td>
                <b>
                    feat(cactus-api-client): common verifier-factory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Besu</span>
            </td>
            <td>
                - Adjust SocketIOApiClient and common Verifier behavior to previous one in cmd-socketio, fix related tests.
- Extract Verifier interfaces to common location to ensure interface compatibility between old and new verifier / verifier factory (both should implement same interface).
- Create new package cactus-verifier-client for common verifier related stuff, to prevent circular dependencies.
- Add verifier-factory to create verifiers by supplying it's ID only, based on initial configuration. Configuration is set in ctor, but can be read from a file as in cmd-socketio scenarious. VerifierFactory config should be compatible with existing ledgerPluginInfo.

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-23 17:50:14 +0000 UTC
    </div>
</div>

