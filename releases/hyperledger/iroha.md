---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Hyperledger Iroha v1.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    1.6.0
                </span>
            </td>
            <td>
                Here are the changes compared to HL Iroha 1.5 (since 10th May 2022):

# Features
1. Added iroha-cpp library. This was done according to Hyperledger Mentorship 2022: [Implement iroha-cpp library for Hyperledger Iroha 1](https://wiki.hyperledger.org/display/INTERN/Implement+iroha-cpp+library+for+Hyperledger+Iroha+1): https://github.com/hyperledger/iroha/pull/2660 by @andprogrammer (mentors were: @baziorek and @Pawlak00)
2. Extended commands AddAssetQuantity and SubtractAssetQuantity with optional parameter "description". This was done according to Hyperledger Mentorship 2023: [Iroha 1: Enhance query functionality by introducing supplementary, optional parameters to extend the versatility and customization capabilities of queries within the Hyperledger Iroha 1 blockchain](https://wiki.hyperledger.org/pages/viewpage.action?pageId=80778614): https://github.com/hyperledger/iroha/pull/4003 by @dominious1 (mentors were: @baziorek , @andprogrammer, @6r1d and @appetrosyan)
3. Feature/proposal batches: https://github.com/hyperledger/iroha/pull/2357 by @iceseer 
4. Feature/db cache multi layer: https://github.com/hyperledger/iroha/pull/2387 by @iceseer 
5. Feature/single pointer cache ref: https://github.com/hyperledger/iroha/pull/2364 by @iceseer 
6. Allow configuring max past time of transaction created_time #1776  by @baziorek 

# Fixes:
1. Fix/rdb burrow storage tests #2243 by @iceseer 
2. Synchronizer fix to store not more than 1000 blocks #2269 by @iceseer
3. No cache synchronization on round switch and Send/Recv packets size become 128 Mb https://github.com/hyperledger/iroha/pull/2218 by @iceseer
4. Fix/transfer asset permitions #2720 by @iceseer 
5. Fix/unkai unexpected symbol check #2731 by @iceseer 
7. Fix/gRPC drop stream bugfix #2749 by @iceseer 
8. Many devops fixes of CI by @safinsaf : (17 Pull Requests or commits)
9. Fix compilation: https://github.com/hyperledger/iroha/pull/2902 by @baziorek 

# Documentation changes:
1. https://github.com/hyperledger/iroha/issues/2446 by @6r1d
2. https://github.com/hyperledger/iroha/pull/2448 by @6r1d
3. https://github.com/hyperledger/iroha/pull/2448 by @6r1d
4. https://github.com/hyperledger/iroha/pull/2475 by @baziorek 
5. https://github.com/hyperledger/iroha/pull/2739 by @baziorek 
6. https://github.com/hyperledger/iroha/pull/2739 by @LiraLemur 
7. https://github.com/hyperledger/iroha/pull/2739 by @cavalryjim
8. https://github.com/hyperledger/iroha/issues/1920 by @6r1d
13. Added information how to built Iroha 1 on Raspberry Pi 4: https://github.com/hyperledger/iroha/pull/2948 by @baziorek 
14. Maintainer list update: https://github.com/hyperledger/iroha/issues/2957 by @6r1d
15. https://github.com/hyperledger/iroha/issues/2579 by @6r1d
16. https://github.com/hyperledger/iroha/pull/3034 by @6r1d
17. https://github.com/hyperledger/iroha/pull/3057 by @omahs
18. https://github.com/hyperledger/iroha/issues/3070 by @6r1d
19. https://github.com/hyperledger/iroha/issues/3079 by @6r1d
20. https://github.com/hyperledger/iroha/pull/3086 by @6r1d
21. https://github.com/hyperledger/iroha/issues/4055 by @6r1d

# What's Changed (all commits)
-------------------
* [skip ci] Retire inactive maintainers by @ryjones in https://github.com/hyperledger/iroha/pull/2082
* Feature/dops 1651/enable fork build by @safinsaf in https://github.com/hyperledger/iroha/pull/2046
* Fix GHA security issue by @safinsaf in https://github.com/hyperledger/iroha/pull/2155
* [Draft] Iroha forks allow build by @safinsaf in https://github.com/hyperledger/iroha/pull/2019
* Fix security issues, remove build from commit option by @safinsaf in https://github.com/hyperledger/iroha/pull/2189
* Bump protobuf from 3.5.1 to 3.15.0 in /docs/source by @dependabot in https://github.com/hyperledger/iroha/pull/1900
* Update Develop by @safinsaf in https://github.com/hyperledger/iroha/pull/2275
* Bump babel from 2.5.3 to 2.9.1 in /docs/source by @dependabot in https://github.com/hyperledger/iroha/pull/1549
* Fix permissions for windows build job by @safinsaf in https://github.com/hyperledger/iroha/pull/2286
* Update develop from main by @safinsaf in https://github.com/hyperledger/iroha/pull/2300
* Fix status checks by @safinsaf in https://github.com/hyperledger/iroha/pull/2375
* Develop to main v1.6-rc.1 by @iceseer in https://github.com/hyperledger/iroha/pull/2405
* [documentation] #2446: improve issue templates by @6r1d in https://github.com/hyperledger/iroha/pull/2448
* [documentation] hyperledger#2446 adds a spoiler to issue templates by @6r1d in https://github.com/hyperledger/iroha/pull/2459
* Updates to requirements by @bhaskarvilles in https://github.com/hyperledger/iroha/pull/1964
* Bump mistune from 2.0.1 to 2.0.3 in /docs/source by @dependabot in https://github.com/hyperledger/iroha/pull/2570
* Develop to main by @iceseer in https://github.com/hyperledger/iroha/pull/2739
* Feature/dops 1957/reduce ci runs by @safinsaf in https://github.com/hyperledger/iroha/pull/2755
* Reduce CI runs by @safinsaf in https://github.com/hyperledger/iroha/pull/2759
* Bump protobuf from 3.15.0 to 3.18.3 in /docs/source by @dependabot in https://github.com/hyperledger/iroha/pull/2783
* Brand new bug report template by @AlexStroke in https://github.com/hyperledger/iroha/pull/2812
* Fix/gRPC drop stream bugfix by @iceseer in https://github.com/hyperledger/iroha/pull/2749
* [documentation] Fix #1920 by @6r1d in https://github.com/hyperledger/iroha/pull/2860
* Allow configuring max past time of transaction `created_time` by @baziorek in https://github.com/hyperledger/iroha/pull/1776
* Follow-up: #1776: Configurable max past created hours - changed type by @baziorek in https://github.com/hyperledger/iroha/pull/2901
* Repaired building iroha according to instruction: Added patch file to make sure abseil library is building without changes by @baziorek in https://github.com/hyperledger/iroha/pull/2902
* Add Iroha select label and restore temporary changes by @safinsaf in https://github.com/hyperledger/iroha/pull/2903
* Repaired building iroha according to instruction: Added patch file to repair building of benchmark library: std::numeric_limits requires <limits> header by @baziorek in https://github.com/hyperledger/iroha/pull/2906
* Remove cache from main workflow by @safinsaf in https://github.com/hyperledger/iroha/pull/2908
* Implement iroha-lib separate module for Hyperledger Iroha 1 by @andprogrammer in https://github.com/hyperledger/iroha/pull/2660
* Added more descriptive Readme file. by @andprogrammer in https://github.com/hyperledger/iroha/pull/2935
* Changes in `vcpkg/build_iroha_deps.sh` file and documentation to inform users that Iroha 1 is working in Raspberry Pi 4 (from HL main repo) by @baziorek in https://github.com/hyperledger/iroha/pull/2948
* [documentation] Fix #2957, update the MAINTAINERS.md file by @6r1d in https://github.com/hyperledger/iroha/pull/2958
* Bump certifi from 2017.11.5 to 2022.12.7 in /docs/source by @dependabot in https://github.com/hyperledger/iroha/pull/2997
* [documentation] #2579: mention Iroha 2 in Iroha docs by @outoftardis in https://github.com/hyperledger/iroha/pull/3034
* doc: correct typos in `readme.md` by @omahs in https://github.com/hyperledger/iroha/pull/3057
* [documentation] #3070: mention reduced dev activity by @6r1d in https://github.com/hyperledger/iroha/pull/3071
* [documentation] #3079: reintroduce m2r2 dependency by @6r1d in https://github.com/hyperledger/iroha/pull/3080
* [documentation] #3079: update the dependencies further by @6r1d in https://github.com/hyperledger/iroha/pull/3086
* Fix in iroha-cpp library + added example of few transactions (HL branch -> develop) by @baziorek in https://github.com/hyperledger/iroha/pull/3148
* [CI]: New PR template by @appetrosyan in https://github.com/hyperledger/iroha/pull/3322
* Update vcpkg from last release by @safinsaf in https://github.com/hyperledger/iroha/pull/3332
* [fix]: Iroha 1: Mac: Repair benchmark  by @baziorek in https://github.com/hyperledger/iroha/pull/3345
* Develop2master 3081 corrections by @baziorek in https://github.com/hyperledger/iroha/pull/3328
* Update MAINTAINERS.md by @6r1d in https://github.com/hyperledger/iroha/pull/3460
* Develop to Master by @safinsaf in https://github.com/hyperledger/iroha/pull/3081
* Bump tornado from 5.1 to 6.3.2 in /docs/source by @dependabot in https://github.com/hyperledger/iroha/pull/3531
* Spelling Mistake by @tarunjainsagar in https://github.com/hyperledger/iroha/pull/3532
* Bump pipreqs from 0.4.9 to 0.4.12 in /docs/source by @dependabot in https://github.com/hyperledger/iroha/pull/3664
* [chore]: #3679 add @DCNick3 to the MAINTAINERS.md by @6r1d in https://github.com/hyperledger/iroha/pull/3680
* Bump pygments from 2.7.4 to 2.15.0 in /docs/source by @dependabot in https://github.com/hyperledger/iroha/pull/3728
* Bump certifi from 2022.12.7 to 2023.7.22 in /docs/source by @dependabot in https://github.com/hyperledger/iroha/pull/3746
* Bump tornado from 6.3.2 to 6.3.3 in /docs/source by @dependabot in https://github.com/hyperledger/iroha/pull/3812
* #3836: Add Bogdan Yamkovoy to MAINTAINERS.md file by @6r1d in https://github.com/hyperledger/iroha/pull/3842
* Trying to fix sfinae problems by reverting vcpkg upgrade (Iroha 1) by @baziorek in https://github.com/hyperledger/iroha/pull/3852
* Trying to upgrade libraries in VCPKG by @baziorek in https://github.com/hyperledger/iroha/pull/3862
* Merge Iroha1 `develop` into `main` by @6r1d in https://github.com/hyperledger/iroha/pull/3960
* [documentation] #4055: Add ReadTheDocs config by @6r1d in https://github.com/hyperledger/iroha/pull/4056
* [documentation] #3945: Update MAINTAINERS.md by @6r1d in https://github.com/hyperledger/iroha/pull/3946
* [chore]: #4102 Update issue templates by @6r1d in https://github.com/hyperledger/iroha/pull/4103
* Trying to repair dependency which stopped working (protoc for golang) by @baziorek in https://github.com/hyperledger/iroha/pull/4173
* Introduce an optional title parameter to the AddAssetQuantity and SubtractAssetQuantity, enhancing functionality within Iroha Core for improved message communication. Ensure corresponding handling capabilities in Iroha CLI for seamless integration. by @dominious1 in https://github.com/hyperledger/iroha/pull/4003
* fix variable error by @xiaolou86 in https://github.com/hyperledger/iroha/pull/4020
* [Confluence Documentation] Update message AddAssetQuantity and SubtractAssetQuantity with extra optional parameter by @dominious1 in https://github.com/hyperledger/iroha/pull/4032
* [chore] #4231: Update MAINTAINERS by @6r1d in https://github.com/hyperledger/iroha/pull/4232
* [chore] #4255: Update Maintainers, add Sato-san by @6r1d in https://github.com/hyperledger/iroha/pull/4254
* Fixing warning in command SubtractAssetQuantity, removing unnecessarily includes, small documentation change by @baziorek in https://github.com/hyperledger/iroha/pull/4251
* Changed "some-host" to "localhost" in example/config.docker by @baziorek in https://github.com/hyperledger/iroha/pull/4281

## New Contributors
* @bhaskarvilles made their first contribution in https://github.com/hyperledger/iroha/pull/1964
* @andprogrammer made their first contribution in https://github.com/hyperledger/iroha/pull/2660
* @omahs made their first contribution in https://github.com/hyperledger/iroha/pull/3057
* @tarunjainsagar made their first contribution in https://github.com/hyperledger/iroha/pull/3532
* @dominious1 made their first contribution in https://github.com/hyperledger/iroha/pull/4003
* @xiaolou86 made their first contribution in https://github.com/hyperledger/iroha/pull/4020

**Full Changelog**: https://github.com/hyperledger/iroha/compare/1.5.0...1.6.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/iroha/releases/tag/1.6.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-02-14 11:21:12 +0000 UTC
    </span>
</div>

