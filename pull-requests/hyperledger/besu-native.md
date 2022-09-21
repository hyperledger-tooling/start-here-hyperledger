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
                PR <a href="https://github.com/hyperledger/besu-native/pull/88" class=".btn">#88</a>
            </td>
            <td>
                <b>
                    prepare for 0.6.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                set next snapshot version
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 17:01:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/85" class=".btn">#85</a>
            </td>
            <td>
                <b>
                    Restore Mac ECDSA libs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Restore the generation of the two ECDSA libs in the new darwin-<arch> format.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 06:02:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/84" class=".btn">#84</a>
            </td>
            <td>
                <b>
                    0.6.1 release version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                0.6.1 release includes:

* Update to jna 5.12.1
* Add linux arm64 build of bls12-381 
* Restrict builds of blake2f to x86-64 

Signed-off-by: garyschulte <garyschulte@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 05:36:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/82" class=".btn">#82</a>
            </td>
            <td>
                <b>
                    Disable arm blake2b
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Benchmarking shows the blake on arm code is slower than the java versions running on arm, so don't build it.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 03:53:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/81" class=".btn">#81</a>
            </td>
            <td>
                <b>
                    Copy linux BLS lib
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Copy the eth_pairings.so lib into the jar resources directory.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 03:01:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/80" class=".btn">#80</a>
            </td>
            <td>
                <b>
                    Build BLS-12 on linux arm
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Build BLS-12 for linux arm.  Also has the altbn128 libs.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-20 19:01:39 +0000 UTC
    </div>
</div>

