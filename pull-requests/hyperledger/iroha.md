---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3356" class=".btn">#3356</a>
            </td>
            <td>
                <b>
                    [refactor]: Block and sumeragi refactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

I was poking around the codebase and refactored a few things:
* with `ProofBuilder` we're assured that proof always has at least one signatures
* with `BlockBuilder` only block that is chained and signed is called a block. Intermediate stages are encapsulated with the builder
* with `Candidate<B>` there is less code duplication

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 07:10:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3351" class=".btn">#3351</a>
            </td>
            <td>
                <b>
                    [refactor] #3349: Remove `EvaluateOnHost` from smart contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Evaluation of expressions on the host is unnecessary so it's been moved into the smart contract itself. `wsv` is only used in one expression evaluation and that is `Expression::Query`. Had we not had this expression, every expression could be evaluated deterministically(whatever the current state of the world may be)

This should not bloat the binary once dynamic linking is in place because evaluation will be taking place in the dynamically linked wasm not the smart contract itself

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3349

### Benefits

* the less interaction with the host the better the performance

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 17:17:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3346" class=".btn">#3346</a>
            </td>
            <td>
                <b>
                    [refactor] #3273: Move to tokio actors in p2p::peer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

- Remove broker 
- Switch from using `iroha_actor` to tokio actors

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

Closes #3273.

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

- Actor is encapsulated insise it's `run` function so it's possible to modify it's state without enum.
- Flexibility in terms how actors communicate with each other (mpsc channels, oneshot channels, ...) this way it's possible to omit communication deadlock.
- Possible to use multiple channels and set priorities on them.
 
### Disadvantages

Solution feels a bit more verbose, but it ~ the same size in LoC.

Direct usage of `select!` can be tricky.

### Alternative design

We can use something like `actix` as actor framework, but it has almost the same api as `iroha_actor` so only benefits will be that it is more battle tested solution.

### Additional comments

I measured tps-benchmark before and after change and there is no significant difference in performance.

```text
Before:
    time:   [1813.8 tps 1925.7 tps 2036.7 tps]
After:
    time:   [2041.3 tps 2252.5 tps 2458.0 tps]
```

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 16:46:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3345" class=".btn">#3345</a>
            </td>
            <td>
                <b>
                    [fix]: Iroha 1: Mac: Repair benchmark 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">1.x</span><span class="chip">build</span><span class="chip">1.5</span>
            </td>
            <td>
                ## Description
Currently `develop` is failling to build on MacOS, after enabling build on MacOS (https://github.com/hyperledger/iroha/commit/829357fb7dd81498fa052cefdee337ac8bc90ce3), that is why I'm trying to fix its by doing something similar to:
https://github.com/hyperledger/iroha/pull/2906/

Hopefully it will fix the compilation error:
https://github.com/hyperledger/iroha/pull/3081#issuecomment-1485817640
```
[5/22] /Library/Developer/CommandLineTools/usr/bin/clang++ -DHAVE_POSIX_REGEX -DHAVE_STD_REGEX -DHAVE_STEADY_CLOCK -I/Users/qwerty/workdir/iroha/vcpkg-build/buildtrees/benchmark/src/eeee844489-b89864c19e.clean/include -I/Users/qwerty/workdir/iroha/vcpkg-build/buildtrees/benchmark/src/eeee844489-b89864c19e.clean/src -I/Users/qwerty/workdir/iroha/vcpkg-build/buildtrees/benchmark/src/eeee844489-b89864c19e.clean/src/../include -fPIC  -std=c++11  -Wall  -Wextra  -Wshadow  -Wshorten-64-to-32  -fstrict-aliasing  -Wno-deprecated-declarations  -Wstrict-aliasing  -Wthread-safety -O3 -DNDEBUG  -Werror  -Wno-deprecated -arch x86_64 -isysroot /Library/Developer/CommandLineTools/SDKs/MacOSX13.1.sdk -mmacosx-version-min=12.6 -MD -MT src/CMakeFiles/benchmark.dir/complexity.cc.o -MF src/CMakeFiles/benchmark.dir/complexity.cc.o.d -o src/CMakeFiles/benchmark.dir/complexity.cc.o -c /Users/qwerty/workdir/iroha/vcpkg-build/buildtrees/benchmark/src/eeee844489-b89864c19e.clean/src/complexity.cc
FAILED: src/CMakeFiles/benchmark.dir/complexity.cc.o 
/Library/Developer/CommandLineTools/usr/bin/clang++ -DHAVE_POSIX_REGEX -DHAVE_STD_REGEX -DHAVE_STEADY_CLOCK -I/Users/qwerty/workdir/iroha/vcpkg-build/buildtrees/benchmark/src/eeee844489-b89864c19e.clean/include -I/Users/qwerty/workdir/iroha/vcpkg-build/buildtrees/benchmark/src/eeee844489-b89864c19e.clean/src -I/Users/qwerty/workdir/iroha/vcpkg-build/buildtrees/benchmark/src/eeee844489-b89864c19e.clean/src/../include -fPIC  -std=c++11  -Wall  -Wextra  -Wshadow  -Wshorten-64-to-32  -fstrict-aliasing  -Wno-deprecated-declarations  -Wstrict-aliasing  -Wthread-safety -O3 -DNDEBUG  -Werror  -Wno-deprecated -arch x86_64 -isysroot /Library/Developer/CommandLineTools/SDKs/MacOSX13.1.sdk -mmacosx-version-min=12.6 -MD -MT src/CMakeFiles/benchmark.dir/complexity.cc.o -MF src/CMakeFiles/benchmark.dir/complexity.cc.o.d -o src/CMakeFiles/benchmark.dir/complexity.cc.o -c /Users/qwerty/workdir/iroha/vcpkg-build/buildtrees/benchmark/src/eeee844489-b89864c19e.clean/src/complexity.cc
/Users/qwerty/workdir/iroha/vcpkg-build/buildtrees/benchmark/src/eeee844489-b89864c19e.clean/src/complexity.cc:85:10: error: variable 'sigma_gn' set but not used [-Werror,-Wunused-but-set-variable]
  double sigma_gn = 0.0;
         ^
1 error generated.
ninja: build stopped: subcommand failed
```

<!-- Just describe what you did. -->
Fixed build (hopefully, because I don't have MacOS), according to the instruction:
https://stackoverflow.com/questions/72588408/vcpkg-how-to-edit-package-file-when-compilation-fails-when-installing-package

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue
https://github.com/hyperledger/iroha/pull/3081
<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits
Successful build on MacOS
<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 15:39:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3342" class=".btn">#3342</a>
            </td>
            <td>
                <b>
                    [chore]: add @0x009922 to the CODEOWNERS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                *Not much to say here.*
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 08:04:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3340" class=".btn">#3340</a>
            </td>
            <td>
                <b>
                    [fix] #2581: reduce noise in logs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

I've researched for possible ways on how to configure logging in `warp`. I found that it's not easy.

Provided warp's tracing filter has hard-coded log levels. To implement something similar, but with patched levels, we need to implement `Filter`. This is not possible because [library authors decided](https://github.com/seanmonstar/warp/issues/555#issuecomment-622568143) that this should be kept internally and consumers should build their filters in a "convenient" way with `warp::any()`.

So, we decided to exclude `/health` route from logging at all, as this is the primary issue.

Also, I found that `WasmSmartContract` debug repr was not that is expected, and fixed it.

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #2581  <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

- less noise in logs
- less noise in TRACE logs (fixed WASM debug repr)

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 13:26:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3339" class=".btn">#3339</a>
            </td>
            <td>
                <b>
                    Revert "BACKPORT [fix] #3330: Fix `untagged` enum de-serialization with `u128` leaves"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Reverts hyperledger/iroha#3338
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 08:41:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3338" class=".btn">#3338</a>
            </td>
            <td>
                <b>
                    BACKPORT [fix] #3330: Fix `untagged` enum de-serialization with `u128` leaves
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Fixed deserialization of `#[serde(untagged)]` enums with `u128` leaf types. 

### Linked issue

Closes #3330  <!-- Replace with an actual number,  -->

### Benefits

Can use `u128` in `Expression` and `FilterOpt`. 

### Checklist

- [X] I've read `CONTRIBUTING.md`
- [X] I've used the standard signed-off commit format (or will squash just before merging)
- [X] All applicable CI checks pass (or I promised to make them pass later)
- [X] (optional) I've written unit tests for the code changes
- [x] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 20:18:06 +0000 UTC
    </div>
</div>

