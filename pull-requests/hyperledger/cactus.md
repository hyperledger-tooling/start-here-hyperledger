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
                PR <a href="https://github.com/hyperledger/cactus/pull/1954" class=".btn">#1954</a>
            </td>
            <td>
                <b>
                    fixing issue #1613 with typos of diagram
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
        Created At 2022-03-30 00:59:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1953" class=".btn">#1953</a>
            </td>
            <td>
                <b>
                    ci(tools): fix iroha AIO image build flake on CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Tests</span>
            </td>
            <td>
                Install git into the builder image directly from the git-core ppa
so that we get the latest available instead of what's in Ubuntu
by default. This means that insteadd of 2.2x we get 2.35 as of
the time of this writing which is exactly what we needed to
fix the problem with the build of vcpkg (which itself is a build
dependency of iroha).
The older git version was not supporting a certain commit ref
syntax/mechanism that some vcpkg dependencies were declared
with and this is where the build would error out.
With the new git version used inside the build image, the problem
no longer exists.

Note: Also upgraded the version of iroha to be used to v1.4.0
because it contains some bug-fixes that we needed for certain
connector features IIRC (don't remember the details though...)

Fixes #1566

Fixes #1262

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-29 22:52:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1948" class=".btn">#1948</a>
            </td>
            <td>
                <b>
                    fix(security): ensure node-forge > 1.3.0 for CVE-2022-24772
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Security</span><span class="chip">P1</span>
            </td>
            <td>
                This is a temporary fix until our direct dependencies get patched
which we can update for ourselves. In the meantime this will force
the (currently considered) secure versions of node-forge to be used.
 
Fixes #1947

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>   

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 18:05:22 +0000 UTC
    </div>
</div>

