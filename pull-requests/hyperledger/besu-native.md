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
                PR <a href="https://github.com/hyperledger/besu-native/pull/63" class=".btn">#63</a>
            </td>
            <td>
                <b>
                    release version for 0.5.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                0.5.0 release includes:
 * multipoint-ipa 
 * arm64-linux support
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-26 17:52:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/62" class=".btn">#62</a>
            </td>
            <td>
                <b>
                    remove defunct rocketchat notification webhook
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                remove former rocketchat notification url config
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-24 23:55:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/61" class=".btn">#61</a>
            </td>
            <td>
                <b>
                    Add Linux ARM64 native support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #57

Adds support for building linux arm64 libs :

* adds arn64 gravition executor to circle ci
* adds arm64 lib copy task for secp256k1 and r1, ipa-multipoint, altbn128
* uses c_lib platform-specific char type in altbn128 to avoid unsigned char problem on linux arm64 / libc6 2.28
* adds OSARCH prefixing of build artifacts to prevent lib name conflicts 
* adds linux arm64 arch detection to skip bls12-381 build (due to unsigned char type mismatch in rust)

BLS12-381 is intentionally omitted from the linux-arm64 build because:
  1. we want to switch to blst
  2. it is unnecessary to [merge unsigned char fix](https://github.com/matter-labs/eip1962/pull/19) upstream
  3. the precompile isn't currently part of any besu protocol schedule 


since this is a change to the layout of the native jars, I tested besu with 0.5.0-SNAPSHOT libs on all three platform identifiers:
linux-gnu-x86_64
```
2022-05-23 15:05:21.111-07:00 | main | INFO  | Besu | Using LibEthPairings native alt bn128
2022-05-23 15:05:21.112-07:00 | main | INFO  | Besu | Using the native implementation of the signature algorithm
2022-05-23 15:05:21.115-07:00 | main | INFO  | Besu | Starting Besu version: besu/v22.4.2-dev-7ea97fd5/linux-x86_64/openjdk-java-11
...
```

darwin (m1)
```
2022-05-23 15:10:21.616-07:00 | main | INFO  | Besu | Using LibEthPairings native alt bn128
2022-05-23 15:10:21.617-07:00 | main | INFO  | Besu | Using the native implementation of the signature algorithm
2022-05-23 15:10:21.620-07:00 | main | INFO  | Besu | Starting Besu version: besu/v22.4.2-dev-7ea97fd5/osx-aarch_64/oracle-java-17
...
```

linux-gnu-aarch64
```
2022-05-23 15:54:47.362-07:00 | main | INFO  | Besu | Using LibEthPairings native alt bn128
2022-05-23 15:54:47.389-07:00 | main | INFO  | Besu | Using the native implementation of the signature algorithm
2022-05-23 15:54:47.419-07:00 | main | INFO  | Besu | Starting Besu version: besu/v22.4.2-dev-5cdda94a/linux-aarch_64/oracle-java-17
...
```



For contrast, besu running on arm64-linux currently gives this output at startup:
```
2022-05-23 22:17:43.912+00:00 | main | INFO  | SECP256K1 | Native secp256k1 not available
2022-05-23 22:17:43.915+00:00 | main | INFO  | Besu | Using the Java implementation of alt bn128
2022-05-23 22:17:43.915+00:00 | main | INFO  | Besu | Using the Java implementation of the signature algorithm
2022-05-23 22:17:43.918+00:00 | main | INFO  | Besu | Starting Besu version: besu/v22.4.1/linux-aarch_64/openjdk-java-11
...
2022-05-23 22:17:44.467+00:00 | main | INFO  | AbstractAltBnPrecompiledContract | Native alt bn128 not available
2022-05-23 22:17:44.468+00:00 | main | INFO  | AbstractAltBnPrecompiledContract | Native alt bn128 not available
2022-05-23 22:17:44.469+00:00 | main | INFO  | AbstractAltBnPrecompiledContract | Native alt bn128 not available
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-21 08:58:40 +0000 UTC
    </div>
</div>

