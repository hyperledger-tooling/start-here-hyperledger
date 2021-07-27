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
                PR <a href="https://github.com/hyperledger/iroha/pull/1294" class=".btn">#1294</a>
            </td>
            <td>
                <b>
                    [wsv_checker]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - [RDB] integration
- build tests
- build tests
- build tests
- fixup!
- Cache overload check
- Amount last dot character fixup
- amount test
- transfer asset test
- formatting
- not ready tests
- tests built
- tests built
- merge result fix
- builded
- fixup
- fixup
- tests fixup
- tests
- build
- formatting
- fixup
- clang10 fixup
- [SE] fixup
- [SE] thread pool tasks counter
- [SE] thread pool busy fixup
- merge fixup
- [RDB] tests fixes
- [RDB] maybe fix
- test fixes
- test fixes
- maybe fix
- maybe fix
- formatting
- [Test] error code check off
- [wsv_checker]
- [wsv_checker] some static_assert-s to rocksdb_common
- [wsv_checker] works with rocksdb through the only one iteration pass
- [wsv_checker] works with postgres, can check_equals()

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-26 10:37:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1291" class=".btn">#1291</a>
            </td>
            <td>
                <b>
                    [GHA] chat-opt from main to support/1.2.x [DO NOT SQUASH]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - [GHA] chat-ops to main
- [GHA] better chat-ops
- [GHA] Separate workflows by inkoking events
- [GHA][Docker] fix clang in iroha-builder
- [GHA] on pull request get /build spec from commit message
- [GHA] Use Dockerhub organization 'iroha1' for forks
- [GHA] clean-up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 13:35:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1290" class=".btn">#1290</a>
            </td>
            <td>
                <b>
                    PR from fork to main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: kuvaldini <ivan@kuvaldini.pro>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

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
        Created At 2021-07-23 06:29:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1289" class=".btn">#1289</a>
            </td>
            <td>
                <b>
                    OOB Query Permission Checks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">api-changes</span><span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Egor Ivkov <e.o.ivkov@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->
Closes #1156 

### Description of the Change
OOB Query Permissions:
1. Access only data of this account
2. Access only data of the account's domain

Also removed a duplicate query -> therefore API will change slightly.
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Benefits
Planned feature
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

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
        Created At 2021-07-22 17:02:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1288" class=".btn">#1288</a>
            </td>
            <td>
                <b>
                    A script to request tags of docker repository from DockerHub using curl and jq
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### output looks like
```
image_hash  <-   tags
sha256:1e86973fc07b5a0b39fa9380df4b3946617730bbce6a1bd41cecf20c5e4a64a2 <- "commit-f0089944cd8198f80152b46ff054fef97474e691-debug","commit-f008994-debug","8c1d840a6e2db587f14955c11b71dcf4d09ef2eabb4500a213b8318cae16d5d6-debug","main-debug"
sha256:21697738ffb1ba3550db5e0ec501fa98f37a0339767bf4a079501f5225f7c8ba <- "commit-2813fe07ae6fba7c023dcc4a470dbfb50a6070a7","commit-2813fe0","8c4ec0ddc055c7777b502b5eae152bfc35e9a7b69707380bdc38f08613c7b34e"
sha256:23bb7afb808cefac211fe947945dcfb89ce044fd28af42b5ef41fbd9ad460259 <- "3680302fd93d8654b5a95fc32211f393c7b45d777748e027b5bbddd79b22f305"
sha256:5b097d332454ca951e1b88c9dc0565b72f59438796af6aaf9ad2a489391b690b <- "commit-3af0b2b154c70235dd0c9c2d284bbe9a5df3f8db-debug","commit-3af0b2b-debug","de2b6aa8c04f08132382131616e89855ff10cffbff1c2aad6ebcaa8e706c5b0d-debug","pr-1271-debug"
sha256:5f5f8cf09edc080a1879e9993e35e4965f797018a834afc96a6bd51173833ce9 <- "commit-90289a0f77a6c68e509de65ffdae6eb6013057de-debug","commit-90289a0-debug","0421393f53f9e25655e605ae29bf99ef726ea807692803770e3664f88d0668bf-debug","pr-1282-debug"
sha256:66f39fd71e3796e192649e2decc511c5ff8e88b0b6dfec6006dfabe611951344 <- "commit-1f0d32ceef3a4d0edbded98d1e4bcdab26a312b1","commit-1f0d32c","21000bb8fd15070d820b2b923bb30e520dbb539232be34d4fccf490cac86a7f3"
sha256:6f458682901353f69ccd0d86b492ddef7285ea7be2db03b67ec90456b4befd24 <- "66abe378038753d369710f97b7def657ccf14ec00b190cf326092d07ec0a074f"
sha256:7c02a230269e9f46c0316378b4646e5503aed98c7f24ed3be6fd9cd5b58801fc <- "commit-cff0c1f36192f9ecb6d1abc45507ea719492c378","commit-cff0c1f","8adc8583f7c24eca0e52a04165d414f498fc7d7c9dcba47aaa06c9850c47a2d1"
sha256:7f8a3031e7d68dc362bf77f413e578b11473f9f3c6044a1ec59deef026c62cff <- "commit-803e6413382bfbd78ef9bee65b1e7f05c949a845","commit-803e641","e7d67a7ea02f7b614c40080324204737cb30d9ee69cf0ca4b7bcb67c4f87dbe7"
sha256:87757b8493c07a1b5a5c3f0ce6de7195100639f32dc3356b62d8b8857b0c0bc0 <- "commit-51fc6d5f4fce838c1b162b62eac21e5b6104bd0a-debug","commit-51fc6d5-debug","71f4b168ab67658a26460147c94c60ac9290d3b43eef626b35c5a2389bcfa4b3-debug","support-1.2.x-debug"
sha256:8deef94ab93eeee3c959a0f9c653c2049785ac698855141cfbcbcef38c668331 <- "commit-581ce647641d9c0bae2743bd97e1a7dcb496e0d3-debug","commit-581ce64-debug","538e0ad273c532adca4ab5c6e3a6d7f4e2b47461607f9228beb69c5313c41cd3-debug"
sha256:9559e5d69b754089d40d2ee785cbebb5bf808d386444f1e180dd1296cd08e0fc <- "commit-89616c90720eca37f3d5837e84d0dc624fd51943-debug","commit-89616c9-debug","af721062cd63da350da9b7adb5666c3a045a4115e3601b66f85ac822333f44a8-debug","pr-1286-debug"
sha256:959b68f116e58dc00a40360cc7170cd460fcbd1639b1e1ce160fa36b0c7935fb <- "commit-b33ffbe1fb797e52cbd0675e67be5d6f862ae567-debug"
sha256:9d00fde72ca6d0c63db59c068b35f18b4376361df59c0f70b804818970286f7c <- "commit-e24fa546a50fa4c29b4027162b184aed62f7e3b1-debug","commit-e24fa54-debug","cf2ebda6617ba36bce116faa23186faae731861a04fcc4d4b6294d64ea91b795-debug"
sha256:9d50220f6df0613ca4dba115cfa23166badf32380d198b8eae553927b31c8a3c <- "bf03c555955ea263288ee8ab24278a8cb1769610ed98790702e6702f5e558a7f-debug"
sha256:9fda5aac9a07b8019e2aefa091575d3beda8d543b23a4049b911ba9debaa736a <- "commit-c8891dadd557bf44cd2f045062729a9c888c3b9f-debug","commit-c8891da-debug","06c9306a3e0f446c9d895a103c284e13cbf0cadf83711fcb4269f808aa2964ec-debug","nightly-debug"
sha256:a030a402edb61b3c49bdaaac712fc42783604536017d95e9de87a1c33a41eeca <- "develop-build","x86_64-develop-build"
sha256:a56d73015ac90181210f517b1f6bc0c71a9ffd806eb9f9605d90587d1f7c9d8b <- "6c92dd33a53f99bb8d6030d08b968d7b3611c14a25484f815dd537027b595329-debug"
sha256:b9722dad4ee92ba4ac9a607590ca46382a15ca850fa953745c67670aab0e4569 <- "commit-2813fe07ae6fba7c023dcc4a470dbfb50a6070a7-debug","commit-2813fe0-debug","1287e561e45df8b264bdac86888fc1cc286d353522c72094c4ff9004eddd189f-debug"
sha256:ca2151be2e58db3bf0125f4cf30f8c7cd2e6397097d6aceebb2ff3f867725407 <- "commit-c8891dadd557bf44cd2f045062729a9c888c3b9f","commit-c8891da","a169143bf72210539609a2947b0a6bc7df8791933989a3442c39b0a424f633b2","nightly"
sha256:cc97f298894519e3406cbe6a3a811961d88fb5c6e8f5598dabdefddf236e21da <- "commit-f0089944cd8198f80152b46ff054fef97474e691","commit-f008994","5a0d65bbda78f0b63d1f646fe707cbad0c267be87e2fa541e9749ec0776dbc62","main"
sha256:d5893edf8fd5e158e4c2ff03ead8053d231e79b75f901364ab5e73f341c891b7 <- "commit-803e6413382bfbd78ef9bee65b1e7f05c949a845-debug","commit-803e641-debug","7415309f526d4db3842db6209cc2453248b0146b765224b390fb1516fd8fe6e7-debug"
sha256:d5f9decfc23b0f479d2a465ee9a3081226e41720e40a287c258685a86f4e5163 <- "commit-cff0c1f36192f9ecb6d1abc45507ea719492c378-debug","commit-cff0c1f-debug","a7d5d3db16f274c697601039c252f37c718f3a45cf1baa2a2642248bcac4836b-debug"
sha256:d7992da09e80467676cdb519169bd8234438400fa44323fc70e9e89c08557952 <- "commit-51fc6d5f4fce838c1b162b62eac21e5b6104bd0a","commit-51fc6d5","66bbbb504030431fa678b459477c36636141f35d413991684e63e5be9c43f5eb","support-1.2.x"
sha256:db419b018b577bd2160ddfe45b1ea7ae028d0a3bb3d07422641c526f0e8acb45 <- "commit-0c25f6c8889e9306719da651ddfc32c3c4cb7969-debug","commit-0c25f6c-debug","d909d72050b2685f61a1a3dbcdaae42a167e247a64ade07c6ca0c7957983af4e-debug","pr-1287-debug"
sha256:dfb8e348a5a3ea4a743d7e7ec449b257b64cd01dd34c0795c0a73cb902c07241 <- "x86_64-main"
sha256:e4ec207099567191dd7f2b5597bcedd0671042f124cddc7f7132328ca3ce6554 <- "commit-d0c2c39f00a0e472251076b623094a1d79a9aa8a","commit-d0c2c39","790991bf5c41376a7acaa618e7bb07c50aa062e3ca7334fac3ca1a61504bb4ff","gha-metrics"
sha256:e5d59451601d0530d6b8c9674a86e62e97eea866988539b8f18c9901e7b4b043 <- "commit-d0c2c39f00a0e472251076b623094a1d79a9aa8a-debug","commit-d0c2c39-debug","8566955a6b8199ec19fcfe95fbb5d353c2d8cbd326d715a9139faa236d8eed8a-debug","gha-metrics-debug"
sha256:e6ea4a634148ac8c1cdf9e66b12be016486545e8b81c531fb6b4bc633d535aa3 <- "commit-b33ffbe1fb797e52cbd0675e67be5d6f862ae567","commit-b33ffbe","7cce673dc6bb80840b53ead2f453b9c5ef011ba79896404b126340ab27ae78a5"
sha256:ed91f38e7041c2a009b726e86848b85af9543146ca2d31aa29fbaaa173a18278 <- "commit-f0089944cd8198f80152b46ff054fef97474e691-clang10-debug","commit-f008994-clang10-debug","pr-1286-clang10-debug","8250ae6bd39c3eb299e5b695cc340a564a1c289ee09a1e7c2dd5d1911335427d-clang10-debug"
sha256:edee8cf7ec0dfa72abc653b926369e7249bea99747b95d38db395fedfaea501b <- "commit-9dce5a4704996959a4458eefa522728e4661dadd-debug","commit-9dce5a4-debug","610e86dbcf39a7168f5d754b40d63d955243d38f6ef2520af9b11eee9f3660c0-debug"
sha256:f20f720cf03d7a284ca95f6c1b528ba0a5058e003d693c73048203694c760c89 <- "commit-45ad048f87cd012b892d8869bba989fdc02a65e6-clang10-debug","commit-45ad048-clang10-debug","pr-1284-clang10-debug","9074817440ba6e8ced4c333d8ce33ca419084e04a7fc635dfa79108932254efd-clang10-debug"
sha256:f4f285005400777bfd61b609f361280bd905b94dfcde4c5ea498e668db3f51f1 <- "commit-1f0d32ceef3a4d0edbded98d1e4bcdab26a312b1-debug","commit-1f0d32c-debug","60f78b7ae5703ab7a1d274823fc9c6fc4e638f24e95c462ddd2018d8161b6f74-debug"
```

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

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
        Created At 2021-07-22 12:12:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1287" class=".btn">#1287</a>
            </td>
            <td>
                <b>
                    Feature: ordering service cache size limit + metrics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change
Adds Ordering Service cache size limitation.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

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
        Created At 2021-07-22 07:05:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1286" class=".btn">#1286</a>
            </td>
            <td>
                <b>
                    TEST CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                /build clang

Signed-off-by: kuvaldini <ivan@kuvaldini.pro>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

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
        Created At 2021-07-22 06:25:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1285" class=".btn">#1285</a>
            </td>
            <td>
                <b>
                    [GHA] test build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

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
        Created At 2021-07-21 21:44:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1284" class=".btn">#1284</a>
            </td>
            <td>
                <b>
                    [GHA][Docker] fix clang in iroha-builder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: kuvaldini <ivan@kuvaldini.pro>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 21:31:19 +0000 UTC
    </div>
</div>

