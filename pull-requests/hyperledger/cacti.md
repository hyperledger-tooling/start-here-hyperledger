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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3174" class=".btn">#3174</a>
            </td>
            <td>
                <b>
                    feat(connector-besu): add gRPC support for operations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. The Besu connector now can be reached via the gRPC interface.
2. The same operations are exposed as via HTTP+SocketIO
3. gRPC supports bi-directional streaming so the block watching is also
supported and test coverage verifies that it works.
4. To see an example of how to use the gRPC client of the Besu connector
read the source code of the test case that provides the verification that
the functionality works:
```
packages/cactus-test-plugin-ledger-connector-besu/src/test/typescript/
integration/grpc-services/connector-besu-grpc-services.test.ts
```

Depends on #3173

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
        Created At 2024-04-04 05:51:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3173" class=".btn">#3173</a>
            </td>
            <td>
                <b>
                    feat(cmd-api-server): add gRPC plugin auto-registration support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. The API server supports gRPC endpoints, but plugins are not yet able
to register their own gRPC services to be exposed the same way that was
already possible for HTTP endpoints to be registered dynamically. This
was due to an oversight when the original contribution was made by Peter
(who was the person making the oversight - good job Peter)
2. The functionality works largely the same as it does for the HTTP
endpoints but it does so for gRPC services (which is the equivalent of
endpoints in gRPC terminology, so service === endpoint in this context.)
3. There are new methods added to the public API surface of the API server
package which can be used to construct gRPC credential and server objects
using the instance of the library that is used by the API server.
This is necessary because the validation logic built into grpc-js fails
for these mentioned objects if the creds or the server was constructed
with a different instance of the library than the one used by the API
server.
4. Different instance in this context means just that the exact same
version of the library was imported from a different path for example
there could be the node_modules directory of the besu connector and also
the node_modules directory of the API server.
5. Because of the problem outlined above, the only way we can have functioning
test cases is if the API server exposes its own instance of grpc-js.

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
        Created At 2024-04-04 05:33:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3170" class=".btn">#3170</a>
            </td>
            <td>
                <b>
                    refactor(ledger-browser): rename ledger browser
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                    refactor(ledger-browser): rename ledger browser
    - delete solid.js version
    - rename package
    - fix type errors
    - bump vite from 5.0.12 to 5.0.13 in /packages/cacti-ledger-browser-react
    
    Closes: #3156
    
    Signed-off-by: Tomasz Awramski <tomasz.awramski@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 18:32:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3168" class=".btn">#3168</a>
            </td>
            <td>
                <b>
                    ci(github): refactor ActionLint job to use the official installer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Previously we just winged it with a bash script downloading another
bash script to unzip the actionlint binaries.
2. From now on we'll use the GitHub action from the marketplace which
has a lot of configuration options exposed in a convenient way such as
what type of warnings to ignore, what version of actionlint to install,
etc.

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
        Created At 2024-04-03 14:56:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3167" class=".btn">#3167</a>
            </td>
            <td>
                <b>
                    ci(ci.sh): fix Docker Compose presence check - migrate to sub-command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. The old way to use docker compose was through the standalone binary
`docker-compose`
2. This was working for a while but now the auto-upgrades that we cannot
seem to avoid have caught up with us and broke ci.sh in the GitHub action
runners because the standalone binary is no longer available at all and
therefore the migration must happen.
3. Point 2 is just a theory but one that is considered to be very likely
correct.
4. It is to be seen if we'll have any other downstream issues such as the
tests failing in other ways due to this underlying docker change.

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
        Created At 2024-04-02 15:57:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3166" class=".btn">#3166</a>
            </td>
            <td>
                <b>
                    test(test-tooling): remove deleted test case from list of tests to run
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. When we removed the RustC compiler class and the backing container,
we also deleted the test cases referencing that code, but we forgot to
remove the test case inclusion from the TAP config.

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
        Created At 2024-04-02 06:09:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3165" class=".btn">#3165</a>
            </td>
            <td>
                <b>
                    refactor(connector-besu): tx poll per second not at full CPU speed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Prior to this change the polling function that waits for transactions
to be confirmed was running in  while loop without any delay, meaning that
the code that fetches the latest block is executing thousands of times
each second (or however fast the CPU in the machine/network connection are).
2. Now there is a second delay between each execution of the loop so that
we are not hammering the node of the ledger we are connected to.
3. This also has the added benefit of the test cases using this method
using much less CPU power.

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
        Created At 2024-04-02 03:54:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3164" class=".btn">#3164</a>
            </td>
            <td>
                <b>
                    test(connector-besu): migrate OpenAPI validation test case to Jest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
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
        Created At 2024-04-02 03:40:09 +0000 UTC
    </div>
</div>

