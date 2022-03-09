---
layout: default
title: indy-plenum
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-plenum
---

# indy-plenum <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-plenum){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1588" class=".btn">#1588</a>
            </td>
            <td>
                <b>
                    ReleaseWF and version bump
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addition of the new release workflow, which will publish Github prereleases as prereleases to pypi and releases as releases.

The version bump is opening a PR with the changes done by the `buildscripts/ubuntu-2004/prepare-package.sh` script,
which is taking the version number from the `.github/actions/set-version/action.yaml`. 

To bump the version on normal pushes to the `ubuntu-20.04-upgrade` branch the `push_pr.yaml` has been changed that it will not trigger when the version bump PR (which is only changing the `'plenum/__version_.json'`)  is openend and merged.

Signed-off-by: pSchlarb <p.schlarb@esatus.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-09 15:47:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1587" class=".btn">#1587</a>
            </td>
            <td>
                <b>
                    Enforce LF for VScode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: pSchlarb <p.schlarb@esatus.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-04 10:44:49 +0000 UTC
    </div>
</div>

