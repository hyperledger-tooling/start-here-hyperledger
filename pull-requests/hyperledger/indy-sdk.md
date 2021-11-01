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
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2439" class=".btn">#2439</a>
            </td>
            <td>
                <b>
                    Add a podspec for objective-c indy wrapper in non-binary distribution
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: conanoc <conanoc@gmail.com>

Previous podspec libindy-objc.podspec has several issues:
- It is based on pre-built binary and the binaries are not provided since v1.8.2
- Old binaries do not support newer versions of swift
- Binary frameworks cannot support multiple versions of swift

Source based podspec would be more convenient because we do not have to prepare binaries and there is no version dependency for swift.
Some notes about this commit:
- The podspec filename have to be the same as the name of the framework. So, I could not keep the previous name libindy-objc.podspec.
- The lastest version of libindy is v1.16.0, but one source file of the wrapper(wrappers/ios/libindy-pod/Indy/Wrapper/IndyErrors.h) had a [bug](https://github.com/hyperledger/indy-sdk/commit/9cd1d56b6209a7152f3cd983a0d6077430f09deb#diff-a29363c28be6b462a2bb8b4797fc665cbf01c89b7ad7e58dedaaa18e4f365a36)(comma missing) and was fixed later. So, tag v1.16.0 cannot be used for ios wrapper.
- Used OpenSSL-XM(1.0.210.1) pod instead of OpenSSL(1.0.210) pod because OpenSSL is not compatible with the latest version of cocoapods. OpenSSL podspec would be better copied to indy-sdk repo with fixes done in OpenSSL-XM.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 09:03:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2438" class=".btn">#2438</a>
            </td>
            <td>
                <b>
                    docs: Update getting started dockerfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Ubuntu 16.04 still installs `Python:2.7` and `pip`. Thus, the `getting-started` docker image doesn't build as expected.
So, an update to `Ubuntu:20.04` is needed for the images to build successfully.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-30 18:13:53 +0000 UTC
    </div>
</div>

