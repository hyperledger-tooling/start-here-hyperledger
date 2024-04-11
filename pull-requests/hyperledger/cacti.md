---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3175" class=".btn">#3175</a>
            </td>
            <td>
                <b>
                    feat(cactus-core): add ConnectRPC service interface and type guard
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Define the types and type guard needed for the API server to be able to
recognize plugins that have implemented a ConnectRPC interface for their
operations.

Also, these types will be used by the plugins themselves to mark the
implementations as valid for ConnectRPC usage.

ConnectRPC is very similar to gRPC but has some nice features in addition
to it such as the HTTP 2 and HTTP 1.1 proxying through express and
fastify HTTP server instances.

For further details see this link:
https://connectrpc.com/

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-04 06:28:52 +0000 UTC
    </div>
</div>

