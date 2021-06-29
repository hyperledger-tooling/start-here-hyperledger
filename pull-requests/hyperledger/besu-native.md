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
                PR <a href="https://github.com/hyperledger/besu-native/pull/41" class=".btn">#41</a>
            </td>
            <td>
                <b>
                    enable builds native M1/arm64 crypto libs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Build darwin-arm64 native crypto libraries 

* bump circle-ci Xcode version
* add both x86 and arm64 arch CFLAGS when building on darwin
* bump jna to 5.8.0 
* bump tuweni to 2.0.0
* fix matter-labs/eip1562 build
* submodule updates to latest
* cargo universal binaries for osx:
  * bump rust version to support aarch64-apple-darwin
  * update circle-ci osx build env to include rust toolchains for x86_64 and aarch64
  * target multiple architectures for cargo builds on osx
  * use lipo to build universal lib from single-arch artifacts

Fixes #40 

darwin artifacts prior (from arm64):
```
besu-native git:(master) ✗ file secp256k1/build/lib/libsecp256k1.0.dylib
secp256k1/build/lib/libsecp256k1.0.dylib: Mach-O 64-bit dynamically linked shared library arm64
```
		
darwin artifacts new (from arm64):
```
➜  besu-native git:(darwin-arm64) find . -name '*dylib' |grep "build/lib" |xargs file
./secp256k1/build/lib/libsecp256k1.dylib:    Mach-O universal binary with 2 architectures: [x86_64:Mach-O 64-bit dynamically linked shared library x86_64] [arm64:Mach-O 64-bit dynamically linked shared library arm64]
./secp256k1/build/lib/libsecp256k1.dylib (for architecture x86_64):     Mach-O 64-bit dynamically linked shared library x86_64
./secp256k1/build/lib/libsecp256k1.dylib (for architecture arm64):      Mach-O 64-bit dynamically linked shared library arm64

./secp256k1/build/lib/libsecp256k1.0.dylib:  Mach-O universal binary with 2 architectures: [x86_64:Mach-O 64-bit dynamically linked shared library x86_64] [arm64:Mach-O 64-bit dynamically linked shared library arm64]
./secp256k1/build/lib/libsecp256k1.0.dylib (for architecture x86_64):   Mach-O 64-bit dynamically linked shared library x86_64
./secp256k1/build/lib/libsecp256k1.0.dylib (for architecture arm64):    Mach-O 64-bit dynamically linked shared library arm64

./altbn128/build/lib/libeth_altbn128.dylib:  Mach-O universal binary with 2 architectures: [x86_64:Mach-O 64-bit dynamically linked shared library x86_64] [arm64:Mach-O 64-bit dynamically linked shared library arm64]
./altbn128/build/lib/libeth_altbn128.dylib (for architecture x86_64):   Mach-O 64-bit dynamically linked shared library x86_64
./altbn128/build/lib/libeth_altbn128.dylib (for architecture arm64):    Mach-O 64-bit dynamically linked shared library arm64

./bls12-381/build/lib/libeth_pairings.dylib: Mach-O universal binary with 2 architectures: [x86_64:Mach-O 64-bit dynamically linked shared library x86_64] [arm64:Mach-O 64-bit dynamically linked shared library arm64]
./bls12-381/build/lib/libeth_pairings.dylib (for architecture x86_64):  Mach-O 64-bit dynamically linked shared library x86_64
./bls12-381/build/lib/libeth_pairings.dylib (for architecture arm64):   Mach-O 64-bit dynamically linked shared library arm64
```


depends on https://github.com/matter-labs/eip1962/pull/18

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 23:36:53 +0000 UTC
    </div>
</div>

