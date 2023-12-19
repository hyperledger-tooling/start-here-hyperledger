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
                PR <a href="https://github.com/hyperledger/besu-native/pull/131" class=".btn">#131</a>
            </td>
            <td>
                <b>
                    Linking error potential fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description
This pull request addresses a critical linking error encountered in the Hyperledger Besu native library. The issue came to light following a modification in the method invocation within the `PedersenHasher` class, where `LibIpaMultipoint.commit` was changed to `LibIpaMultipoint.commit_root`. As a result of this change, a `java.lang.UnsatisfiedLinkError` is triggered when calling the `commit_root` method, with the error message: `'byte[] org.hyperledger.besu.nativelib.ipamultipoint.LibIpaMultipoint.commit_root(byte[])'`.

### Proposed Fix
The fix proposed in this pull request involves renaming the `commit_root` method from snake_case to camelCase. This renaming aims to:

- Align with Java's standard naming conventions.
- Potentially resolve the linking issues that are currently being faced.

### Context
While other methods in the `LibIpaMultipoint` class, such as `commit` and `pedersenHash`, continue to operate as expected, it is believed that the naming convention employed for `commit_root` may be contributing to the linking error.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-18 15:49:16 +0000 UTC
    </div>
</div>

