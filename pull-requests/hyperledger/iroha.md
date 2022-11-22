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
                PR <a href="https://github.com/hyperledger/iroha/pull/2961" class=".btn">#2961</a>
            </td>
            <td>
                <b>
                    [fix] #2541 "deserialization failed" on default configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sirawit Techavanitch sirawitt42@gmail.com
### Description of the Change

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->
### Issue
`--entrypoint irohad`  has produced `deserialization failed` bug and the docker command to start the Iroha container passes an invalid env name in this PR change the env name to align with old docs and `--entrypoint irohad` can't be used


- Fixes #2541 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

- Iroha container can run normally with the command from documents
- compatible with postgres config and rockdb config

### Possible Drawbacks

**Changed**  
- hyperledger/iroha on docker hub need to be update
- env in` entrypoint.sh ` has been changed and  `--entrypoint irohad` can't be used

**Additions **
- sample config.postgres.docker has been added to directory /example
- sample config.rockdb.docker has been added to directory/example

**Deletions**
- none

### Usage Examples or Tests *[optional]*
run with `config.postgres.docker`
![image](https://user-images.githubusercontent.com/31649128/203050574-44c01ec7-aada-4fe5-a860-3c97199ada81.png)

run with `config.rockdb.docker
`![image](https://user-images.githubusercontent.com/31649128/203051207-3cb44688-d1bc-4c72-9997-a624e2e62846.png)

### Alternate Designs *[optional]*

- none
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-22 03:59:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2959" class=".btn">#2959</a>
            </td>
            <td>
                <b>
                    [backport]:  `p2p` and `stable` changes from `rc10`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Daniil Polyakov <arjentix@gmail.com><!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Cherry picked commits + rebuild of `p2p` backport to LTS

### Issue

None

### Benefits

More developments. 

### Possible Drawbacks

Possible binary incompatibility. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-21 07:31:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2958" class=".btn">#2958</a>
            </td>
            <td>
                <b>
                    [documentation] Fix #2957, update the MAINTAINERS.md file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR contains a new maintainer list, feel free to point out who should be added or removed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-21 07:24:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2956" class=".btn">#2956</a>
            </td>
            <td>
                <b>
                    [refactor] #1868: Prevent validated transactions from being sent between peers
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

Add `CandidateBlock` which is send between peers, `revalidation` required to obtain `ValidBlock` for `CandidateBlock`.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closes #1868.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Don't rely on programmer to do revalidation and make it unavoidable through strong typing.  

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

None.

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

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
        Created At 2022-11-18 16:02:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2953" class=".btn">#2953</a>
            </td>
            <td>
                <b>
                    [refactor]: Add `storage` folder into gitignore
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Vladimir Pesterev <pesterev@pm.me>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

This PR hides from Git the annoying `storage/` folder, which appears after every running of the Iroha.

### Issue

None

### Benefits

It slightly improves the developer experience using the Iroha locally. 

### Possible Drawbacks

None
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-16 17:51:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2951" class=".btn">#2951</a>
            </td>
            <td>
                <b>
                    [fix] #2850: Fix deserialization/decoding of `Fixed`
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

Check that `Fixed` is not negative during decoding/deserialization. 

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closes #2850.

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Corrent decoding/deserialization behavior.

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

None.

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

```
cargo test --package iroha_primitives --lib -- fixed::tests --nocapture
```

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-16 12:48:57 +0000 UTC
    </div>
</div>

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

