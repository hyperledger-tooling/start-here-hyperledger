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
                PR <a href="https://github.com/hyperledger/iroha/pull/2948" class=".btn">#2948</a>
            </td>
            <td>
                <b>
                    Changes in `vcpkg/build_iroha_deps.sh` file and documentation to inform users that Iroha 1 is working in Raspberry Pi 4 (from HL main repo)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Full description from https://github.com/hyperledger/iroha/pull/2944. Because of security reason those changes must be done from main hyperledger repository, not forks.
_________________________
<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

#### History
Lets start with what is not really important - history:
Few years ago I managed to build Iroha 1.1.3 on RPI3 and RPI4, I created special tutorial:
https://wiki.hyperledger.org/pages/viewpage.action?pageId=41584046
After that I was suggested to create PR (https://github.com/hyperledger/iroha/pull/728) and @lebdron created his PR (https://github.com/hyperledger/iroha/pull/864/) to make building on RPI as automatic as possible.
During those few years I was thinking that I should create similar PR for `develop` version, but it was really hard (as You see PR from @lebdron). Recently somebody from community posted message that he is using Iroha 1.5 on RPI: https://t.me/hyperledgeriroha/25004 - it added me motivation to try again...

#### Important description of change
1. `vcpkg/build_iroha_deps.sh` - to use `vcpkg` on RPI ( `aarch64` architecture ) we need `export VCPKG_FORCE_SYSTEM_BINARIES=1` before calling `vcpkg`.
2. Added information to documentation to expose that Iroha 1 can be build on RPI and build process is easy.
3. I noticed problem with building documentation (instruction: https://github.com/hyperledger/iroha/tree/main/docs):
```
make html
...
Could not import extension m2r2 (exception: No module named 'm2r2')
```
that is why I added entry to `docs/source/requirements.txt` file

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
If somebody wants to build Iroha for RPI4 - it would be easier for users. Also if somebody (who does not know Iroha) would like to find blockchain who is working on RPI - it will be easier.
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
Review process:D.
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*
Testing on RPI4 according to https://iroha.readthedocs.io/en/develop/build/index.html#linux-pre:
```
apt-get update; \
apt-get -y --no-install-recommends install \
   build-essential ninja-build \
   git ca-certificates tar curl unzip cmake \
   pkg-config zip

git clone -b rpi_fix https://github.com/baziorek/iroha.git
cd iroha
./vcpkg/build_iroha_deps.sh $PWD/vcpkg-build

cmake -B build -DCMAKE_TOOLCHAIN_FILE=$PWD/vcpkg-build/scripts/buildsystems/vcpkg.cmake . -DCMAKE_BUILD_TYPE=RELEASE -DUSE_BURROW=OFF -DUSE_URSA=OFF -DTESTING=OFF -DPACKAGE_DEB=OFF

cmake --build ./build --target all

./build/bin/irohad
# log from irohad with missing arguments was printed
```
<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*
Different description
<!-- Explain what other alternates were considered and why the proposed version was selected -->

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-15 09:21:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2947" class=".btn">#2947</a>
            </td>
            <td>
                <b>
                    [refactor]: `p2p` with guard rails
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change

Add extra guard rails to fix problems of multigenerational Iroha networks.
### Issue

None (TODO)
<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Better UX

### Possible Drawbacks

More coupled code

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-15 08:18:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2946" class=".btn">#2946</a>
            </td>
            <td>
                <b>
                    [feature] #2868: Emit iroha version and commit hash in logs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Shanin Roman <shanin1000@yandex.ru>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Emit iroha version and commit hash in logs.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closes #2868.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

More clear debugging. 

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

None.

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-14 16:25:39 +0000 UTC
    </div>
</div>

