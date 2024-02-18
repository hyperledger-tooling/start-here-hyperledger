---
layout: default
title: besu-native
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu-native
---

# besu-native <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-native){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/151" class=".btn">#151</a>
            </td>
            <td>
                <b>
                    chore!: Modify functionality of `commitRoot` to use `groupToField`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Rationale

For the Java library, this will eventually reduce the API surface needed. `commitRoot` will essentially become a call to `commitToScalar` + `groupToField`.

This issue expands on the rationale: https://github.com/crate-crypto/rust-verkle/issues/86

---

There are some geth and go-verkle PRs which would be good to merge before merging this (Leaving this as a Draft while those are open)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-18 00:21:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/150" class=".btn">#150</a>
            </td>
            <td>
                <b>
                    fix native-build.sh update rust version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                quick fix @matkt 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-12 20:34:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/149" class=".btn">#149</a>
            </td>
            <td>
                <b>
                    Add update sparse commitment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding updateSparseCommitment with test. This can be merged after https://github.com/hyperledger/besu-native/pull/146

Closes https://github.com/hyperledger/besu-native/issues/129
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-12 17:58:22 +0000 UTC
    </div>
</div>

