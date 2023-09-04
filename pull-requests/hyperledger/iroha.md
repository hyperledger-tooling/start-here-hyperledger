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
                PR <a href="https://github.com/hyperledger/iroha/pull/3862" class=".btn">#3862</a>
            </td>
            <td>
                <b>
                    Trying to upgrade libraries in VCPKG
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">version bump</span><span class="chip">1.x</span><span class="chip">1.5</span>
            </td>
            <td>
                ## Description
In PR https://github.com/hyperledger/iroha/pull/3852/ I needed to revert upgrading VCPKG. It caused libraries to downgrade. So now we need to try to upgrade libraries manually one by one.

Corrections (marked as [x] when CI passed):
- [x] iroha-ed25519 (no updates)
- [x] protobuf 3.15.8 -> 3.21.12
- [x] abseil 2021-03-24 -> 20230125.0
- [x] benchmark 1.5.2 -> 1.7.1
- [x] gflags 2.2.2-1 -> 2.2.2#5
- [x] nlohmann-json 3.9.1 -> 3.11.2
- [x] rapidjson 2020-09-14 -> 2022-06-28#3
- [x] rxcpp 4.1.0-1 -> 4.1.1#1
- [x] rocksdb 6.14.6 -> 7.9.2
- [ ] fmt 7.1.3#4 -> 9.1.0#1 - PROBLEM
- [ ] spdlog 1.8.5#2 -> 1.11.0 - PROBLEM
- [ ] gtest 1.10.0#4 -> 1.13.0 - PROBLEM
- [ ] grpc 1.37.0#1 -> 1.51.1 - PROBLEM
- [ ] soci[boost,postgresql] - PROBLEM
- [ ] prometheus-cpp 0.12.2 -> 1.1.0 - PROBLEM
- [ ] boost-* - PROBLEM

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits
Newer packages - it will compile longer, less bugs, more security etc.

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

# More information:
I was using the tutorial (as inspiration): https://stackoverflow.com/questions/72588408/vcpkg-how-to-edit-package-file-when-compilation-fails-when-installing-package
1. First I've build all packages with VCPKG in newest versions (details: https://github.com/hyperledger/iroha/pull/3852)
2. Then I used older version of vcpkg (+ packages).
3. I've created repository in `./vcpkg-build`
4. For each patch I've used the function:
```
function update_library
{
    # this function should be run in vcpkg-build directory, where sub-repository is initialised 
    # according to: https://stackoverflow.com/questions/72588408/vcpkg-how-to-edit-package-file-when-compilation-fails-when-installing-package
    library_name=$1
    source_directory_name_to_copy_files='vcpkg-build_newest' # remember to set proper name
    echo "Trying to update: $library_name, from version: $(./vcpkg list | grep $library_name)"
    
    rm ports/${library_name}/*
    cp ../${source_directory_name_to_copy_files}/ports/${library_name}/* ports/${library_name}/
    git add ports/${library_name}/
    git status
    git diff --cached > ../vcpkg/patches/upgrade_${library_name}_to_.patch
    git reset --hard
}
# example:
update_library protobuf
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-02 09:26:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3859" class=".btn">#3859</a>
            </td>
            <td>
                <b>
                    BACKPORT [fix] #3853: Compare permission token payload as JSON
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

Backport of #3855 

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3853

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
        Created At 2023-09-01 10:09:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3855" class=".btn">#3855</a>
            </td>
            <td>
                <b>
                    [fix] #3853: Compare permission token payload as JSON
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

1. `StringWithJson` should implement `PartialEq` comparison as JSON
this was causing bugs when `iroha-java` would serialize token payload vs when `iroha` `serde` would do so 
2. remove `DefaultValidator` struct from `iroha_validator`
it's been used incorrectly, because the delegated method must always call back into original validator whereas calling into `DefaultValidator` would prevent this. Interestingly, removing `DefaultValidator` didn't increase code duplication which was the argument for introducing it in the first place
3. removed `DoesAccountHavePermissionToken`
As is discussed in #3857 the comparison of `PermissionToken`s on the host side is broken and cannot be relied upon. Additionally, there is little reason to think it measurably optimizes the operation of finding a token for an account especially since it's only executed from the validator
4. discovered #3857

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3853 

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
        Created At 2023-08-31 12:12:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3854" class=".btn">#3854</a>
            </td>
            <td>
                <b>
                    [refactor] #2573: Use a more efficient representation for immutable bytes values
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Introduce an `ImmutableBytes` type that is a newtype around `Box<[u8]>` and use it in `PublicKey`, `PrivateKey`, `Signature` and `Multihash` objects.

While `PublicKey` and `PrivateKey` can be further specialized, as their size can be known without storing separately, this is not true for `Signature`, as it can take any user-provided slice as its payload. `Multihash` can also be specialized, but it's used as a temporary representation, so it is not really helpful in reducing resident memory consumption.

### Linked issue

Closes #2573

### Benefits

- This uses 8 bytes less memory for every `PublicKey`, `PrivateKey`, `Signature`and `Multihash` objects

### Checklist


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-31 11:24:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3852" class=".btn">#3852</a>
            </td>
            <td>
                <b>
                    Trying to fix sfinae problems by reverting vcpkg upgrade (Iroha 1)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">version bump</span><span class="chip">1.x</span><span class="chip">build</span><span class="chip">config-changes</span><span class="chip">CI</span><span class="chip">1.5</span><span class="chip">Dev defect</span>
            </td>
            <td>
                ## Description
Some time ago vcpkg package manager was bumped to newest version (commit: https://github.com/hyperledger/iroha/commit/fdc2c1edbc6ce091f6550f8426cda0c8902b7983). It caused dependencies to upgrade a lot so project stopped to compile. I was able to fix compilation of binaries (commit: https://github.com/hyperledger/iroha/commit/3b40f2243f6e2860971c8dce03796fb6ba48a093) but I was unable to fix compilation of tests (SFINAE problem) after some time of trying.

So I decided that we need to make project compiling with not the most professional way, but it should work (and be first step for more professional way). The way is to revert those commits:
1. https://github.com/hyperledger/iroha/commit/fdc2c1edbc6ce091f6550f8426cda0c8902b7983
2. https://github.com/hyperledger/iroha/commit/3b40f2243f6e2860971c8dce03796fb6ba48a093

After those reverts it compiled locally (I used docker: `docker run -it --name='Ubuntu_under_test_22.04' -v ${PWD}/./:/home/ --workdir=/home/ ubuntu:22.04` with `g++ (Ubuntu 11.4.0-1ubuntu1~22.04) 11.4.0`) - both binaries and tests compiled with commands:
```
cmake -B build -DCMAKE_TOOLCHAIN_FILE=$PWD/vcpkg-build/scripts/buildsystems/vcpkg.cmake . -DCMAKE_BUILD_TYPE=RELEASE   -GNinja -DUSE_BURROW=OFF -DUSE_URSA=OFF -DTESTING=ON -DPACKAGE_DEB=OFF  # testing ON
cmake --build ./build --target all  # target = all
``` 

**For now I want to check if CI is compiling, that is why the PR is not ready for review yet.**

## Difference between versions
1. Old version of vcpkg:
```
$ ./vcpkg-build/vcpkg version
Vcpkg package management program version 2021-01-13-unknownhash
$ git log -1
commit e8dbfcf6797a270ed5be8550248f7fe4fe5dec79 (HEAD)
Author: Matthias C. M. Troffaes <matthias.troffaes@gmail.com>
Date:   Tue May 4 07:14:55 2021 +0100

    [ffmpeg] soxr dependency fix (#17299)
    
    * [ffmpeg] soxr only makes sense with swresample, so add as dependency
    
    * [ffmpeg] bump port version
    
    * [ffmpeg] x-add-version
```
2. New version of vcpkg:
```
$ ./vcpkg-build_newest/vcpkg version
vcpkg package management program version 2023-02-16-12e657924d99511514c0287ca5ce46882d3657c7
$ git log -1
commit a7b6122f6b6504d16d96117336a0562693579933 (HEAD, tag: 2023.02.24)
Author: Frank <65999885+FrankXie05@users.noreply.github.com>
Date:   Sat Feb 25 06:08:21 2023 +0800

    [fmilib] Change to the github and update to fix bug of libexpat (#29805)
```

### Version compare in table (generated by ChatGpt, so there can be mistakes):
| Library              | Before Upgrade | After Upgrade |
|----------------------|----------------|---------------|
| abseil               | 2021-03-24     | 20230125.0    |
| benchmark            | 1.5.2          | 1.7.1         |
| boost-accumulators   | 1.75.0         | 1.81.0#2      |
| boost-algorithm      | 1.75.0         | 1.81.0#2      |
| boost-align          | 1.75.0         | 1.81.0#2      |
| boost-any            | 1.75.0         | 1.81.0#2      |
| boost-array          | 1.75.0         | 1.81.0#2      |
| boost-asio           | 1.75.0#1       | 1.81.0#2      |
| boost-assert         | 1.75.0         | 1.81.0#2      |
| iroha-ed25519         | 2.0.1          | 2.0.1        |
| liblzma              | 5.2.5#2        | 5.4.1#1       |
| libpq                | 12.2#16        | 14.4#3        |
| libpq[openssl]       | ...            | ...           |
| libpq[zlib]          | ...            | ...           |
| lz4                  | ...            | 1.9.4#1       |
| nlohmann-json        | 3.9.1          | 3.11.2        |
| openssl              | 1.1.1k         | 3.0.8         |
| prometheus-cpp       | 0.12.2         | 1.1.0         |
| prometheus-cpp[compression] | ...      | ...          |
| prometheus-cpp[pull] | ...            | ...           |
| protobuf             | 3.15.8         | 3.21.12       |
| rapidjson            | 2020-09-14     | 2022-06-28#3  |
| re2                  | 2020-10-01     | 2023-02-01    |
| rocksdb              | 6.14.6         | 7.9.2         |
| rocksdb[zlib]        | ...            | ...           |
| rxcpp                | 4.1.0-1        | 4.1.1#1       |
| soci                 | 4.0.1#3        | 4.0.3         |
| soci[boost]          | ...            | ...           |
| soci[postgresql]     | ...            | ...           |
| spdlog               | 1.8.5#2        | 1.11.0        |
| upb                  | 2020-12-19#1   | 2022-06-21    |
| upb[codegen]         | ...            | ...           |
| vcpkg-cmake-config   | 2021-02-26#1   | 2022-02-06#1  |
| vcpkg-cmake-get-vars | ...            | 2022-12-16    |
| vcpkg-cmake          | 2021-02-28#1   | 2022-12-22    |
| zlib                 | 1.2.11#10      | 1.2.13        |
| zstd                 | 1.4.9          | 1.5.4         |

[vcpkg_libraries_new.txt](https://github.com/hyperledger/iroha/files/12482605/vcpkg_libraries_new.txt)
[vcpkg_libraries_old.txt](https://github.com/hyperledger/iroha/files/12482606/vcpkg_libraries_old.txt)

# Future plans:
If my fix works packages can be upgraded one by one until we face the SFINAE problem again - that package/packages would stay in older version. Of course this can be done in another PR.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Iroha 1 starts compilling again and another release 1.6 would be possible.
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
        Created At 2023-08-30 21:02:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3851" class=".btn">#3851</a>
            </td>
            <td>
                <b>
                    BACKPORT [fix] #3843: Allow genesis to execute any ISI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3843

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
        Created At 2023-08-29 12:11:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3850" class=".btn">#3850</a>
            </td>
            <td>
                <b>
                    [fix] #3843: Allow genesis to execute any ISI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3843 

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
        Created At 2023-08-29 12:05:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3847" class=".btn">#3847</a>
            </td>
            <td>
                <b>
                    [fix] #3762: Fix `irrefutable_let_patterns` in the `#[model]` macro
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description
Slightly amended `#[derive(FromVariant)]` macro to account for the degenerate case of a single variant enum, thus fixing the lint.
<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3762. <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits
No annoying warnings
<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
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
        Created At 2023-08-28 15:05:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3846" class=".btn">#3846</a>
            </td>
            <td>
                <b>
                    BACKPORT [fix] #3843: Treat genesis account as owner during validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3843

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
        Created At 2023-08-28 14:00:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3844" class=".btn">#3844</a>
            </td>
            <td>
                <b>
                    [fix] #3843: Fix genesis validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3843

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
        Created At 2023-08-28 13:54:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3842" class=".btn">#3842</a>
            </td>
            <td>
                <b>
                    #3836: Add Bogdan Yamkovoy to MAINTAINERS.md file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: 6r1d <vic.6r1d@gmail.com>

## Description

### Linked issue

Closes #3836

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Requested by TOC

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-28 06:24:57 +0000 UTC
    </div>
</div>

