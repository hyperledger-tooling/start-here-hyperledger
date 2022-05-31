---
layout: default
title: cello
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/cello
---

# cello <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cello){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Continue basic blockchain deployment works
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.0.0-alpha2
                </span>
            </td>
            <td>
                ## What's Changed
* Defang stalebot by @ryjones in https://github.com/hyperledger/cello/pull/25
* Fix the image path by @yeasy in https://github.com/hyperledger/cello/pull/26
* Removed the read only header in the doc by @litong01 in https://github.com/hyperledger/cello/pull/28
* Fix the image path by @yeasy in https://github.com/hyperledger/cello/pull/27
* [CE-713] Fabric Operator zip structure README by @Man-Jain in https://github.com/hyperledger/cello/pull/29
* [Close #32] Add bug issue & pull request template by @hightall in https://github.com/hyperledger/cello/pull/33
* [Close #32] Add bug issue & pull request template by @hightall in https://github.com/hyperledger/cello/pull/34
* [Close #37] Move make check into template by @hightall in https://github.com/hyperledger/cello/pull/38
* [Fix #35] Remove unused images download operation by @hightall in https://github.com/hyperledger/cello/pull/36
* [Fix #39] Add curl install for ansible agent by @hightall in https://github.com/hyperledger/cello/pull/40
* In product mode, api engine docs can not find static files by @hightall in https://github.com/hyperledger/cello/pull/41
* [CE-715]Fixed the fabric operator image path issue by @litong01 in https://github.com/hyperledger/cello/pull/45
* [Fix #47] Fix node status check crash for k8s agent by @hightall in https://github.com/hyperledger/cello/pull/48
* [Fix #42] Fix nginx server media url not working by @hightall in https://github.com/hyperledger/cello/pull/43
* [Fix #50] Add api engine service port into dashboard by @hightall in https://github.com/hyperledger/cello/pull/51
* [Close #53] Refine bug report issue template by @hightall in https://github.com/hyperledger/cello/pull/55
* [CE-716]Fixed the role binding issue by @litong01 in https://github.com/hyperledger/cello/pull/56
* [Fix #52] Fix k8s 1.16 later version not support. by @hightall in https://github.com/hyperledger/cello/pull/57
* [#issue-59] Ansible agent can not support fabric 1.4.3 by @litong01 in https://github.com/hyperledger/cello/pull/60
* Bump mongoose from 4.13.11 to 5.7.5 in /build_image/dockerhub/v0.9.0-beta/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/58
* [#61]Fixed operation CA example cr yaml file by @litong01 in https://github.com/hyperledger/cello/pull/62
* [#63]Removed the few extra spaces from the example yaml by @litong01 in https://github.com/hyperledger/cello/pull/64
* [Close #66] Add netlify.toml config file by @hightall in https://github.com/hyperledger/cello/pull/67
* [#70]Fixed the capability version string by @litong01 in https://github.com/hyperledger/cello/pull/71
* [#54]Remove the create button in node page when the user is operator by @fengyangsy in https://github.com/hyperledger/cello/pull/82
* [#80] Ansible agent fails create daemonset on k8s 1.16 by @litong01 in https://github.com/hyperledger/cello/pull/81
* Update Kubernetes Agent for dockerhub by @Man-Jain in https://github.com/hyperledger/cello/pull/74
* Imporve Agent to Create/Delete Node and Update UI by @Man-Jain in https://github.com/hyperledger/cello/pull/76
* Improves Kubernetes Operator Agent Documentation by @Man-Jain in https://github.com/hyperledger/cello/pull/78
* [Close #83] Fix netlify build function failed by @hightall in https://github.com/hyperledger/cello/pull/84
* Add build status badge by @ryjones in https://github.com/hyperledger/cello/pull/86
* Remove Gerrit references by @ryjones in https://github.com/hyperledger/cello/pull/88
* [CE-718] Correct license by @ryjones in https://github.com/hyperledger/cello/pull/89
* Fix Prettier error by @ryjones in https://github.com/hyperledger/cello/pull/92
* Bump mongoose from 4.13.11 to 5.7.5 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/91
* Bump mixin-deep from 1.3.1 to 1.3.2 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/93
* Bump lodash.merge from 4.6.1 to 4.6.2 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/95
* Bump stringstream from 0.0.5 to 0.0.6 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/96
* Bump sshpk from 1.13.1 to 1.16.1 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/94
* Bump js-yaml from 3.11.0 to 3.13.1 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/97
* Bump protobufjs from 5.0.2 to 5.0.3 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/99
* Bump lodash from 4.17.5 to 4.17.15 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/98
* Update packages by @ryjones in https://github.com/hyperledger/cello/pull/103
* Remove the v0.9.0-beta dockefiles as we have v0.9.0 already. by @yeasy in https://github.com/hyperledger/cello/pull/105
* update url for downloading fabric artifacts(fix #109) by @dexhunter in https://github.com/hyperledger/cello/pull/110
* Documented requirements on persistent storage by @craig8 in https://github.com/hyperledger/cello/pull/117
* Clean up docker build for api-engine by @yeasy in https://github.com/hyperledger/cello/pull/120
* Update dependency versions by @yeasy in https://github.com/hyperledger/cello/pull/122
* modified base_name to basename by @MintCollie in https://github.com/hyperledger/cello/pull/124
* Update api-engine dockerfile for dockerhub build by @yeasy in https://github.com/hyperledger/cello/pull/128
* Fix issue #125 by @litong01 in https://github.com/hyperledger/cello/pull/134
* fix(swagger): disable manual parameter for swagger doc by @hightall in https://github.com/hyperledger/cello/pull/133
* More fixes to the build broken issue #125 by @litong01 in https://github.com/hyperledger/cello/pull/137
* Move onto Azure DevOps by @litong01 in https://github.com/hyperledger/cello/pull/140
* Optimize build process by @litong01 in https://github.com/hyperledger/cello/pull/142
* Restructure Fabric k8s operator by @litong01 in https://github.com/hyperledger/cello/pull/144
* Update documentation by @ryjones in https://github.com/hyperledger/cello/pull/145
* Update documents by @spartucus in https://github.com/hyperledger/cello/pull/148
* improvement: upgrade umi version to 3.0 by @hightall in https://github.com/hyperledger/cello/pull/153
* improvement: upgrade antd version to 4 by @hightall in https://github.com/hyperledger/cello/pull/155
* fix: fix new node operation page can't work by @hightall in https://github.com/hyperledger/cello/pull/158
* Fixed fabric operator default settings by @litong01 in https://github.com/hyperledger/cello/pull/159
* Fixed issue report in #165 by @litong01 in https://github.com/hyperledger/cello/pull/166
* Bump express-jwt from 5.3.1 to 6.0.0 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/164
* Bump lodash from 4.17.15 to 4.17.19 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/167
* feat: add menuconfig support for server deployment config by @hightall in https://github.com/hyperledger/cello/pull/170
* fix: fix .config file content can not load for kconfig by @hightall in https://github.com/hyperledger/cello/pull/173
* docs: add document for menuconfig makefile command by @hightall in https://github.com/hyperledger/cello/pull/175
* feat: add basic framework for k8s rest agent by @hightall in https://github.com/hyperledger/cello/pull/177
* Bump elliptic from 6.5.2 to 6.5.3 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/178
* Bump mongodb from 2.2.36 to 3.1.13 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/181
* add docker rest api agent by @dexhunter in https://github.com/hyperledger/cello/pull/180
* Add hyperledger fabric image by @yeasy in https://github.com/hyperledger/cello/pull/185
* Update docker rest api 1 by @dexhunter in https://github.com/hyperledger/cello/pull/193
* Add dockerfile to agent-docker and Fix some bugs by @XuHugo in https://github.com/hyperledger/cello/pull/192
* Bump dot-prop from 4.2.0 to 4.2.1 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/195
* Bump bl from 1.2.2 to 1.2.3 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/194
* Bump ini from 1.3.5 to 1.3.8 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/199
* Cryptogen by @XuHugo in https://github.com/hyperledger/cello/pull/198
* Configtx by @XuHugo in https://github.com/hyperledger/cello/pull/202
* Bump socket.io from 2.3.0 to 2.4.0 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/206
* Models by @XuHugo in https://github.com/hyperledger/cello/pull/208
* Organization by @XuHugo in https://github.com/hyperledger/cello/pull/209
* Node by @XuHugo in https://github.com/hyperledger/cello/pull/210
* Network by @XuHugo in https://github.com/hyperledger/cello/pull/211
* Agent by @XuHugo in https://github.com/hyperledger/cello/pull/212
* Update Maintainers by @yeasy in https://github.com/hyperledger/cello/pull/215
* Clean the potential existing msp and tls paths by @yeasy in https://github.com/hyperledger/cello/pull/214
* Fix cello-hlf image dockerfile by @yeasy in https://github.com/hyperledger/cello/pull/216
* Node cfg by @XuHugo in https://github.com/hyperledger/cello/pull/218
* add update function for docker agent by @dexhunter in https://github.com/hyperledger/cello/pull/217
* Bump pug-code-gen from 2.0.2 to 2.0.3 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/224
* Nodecreate1 by @XuHugo in https://github.com/hyperledger/cello/pull/226
* Nodecreate2 by @XuHugo in https://github.com/hyperledger/cello/pull/227
* Nodecreate3 by @XuHugo in https://github.com/hyperledger/cello/pull/228
* Bump elliptic from 6.5.3 to 6.5.4 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/229
* [#230]add register page by @fengyangsy in https://github.com/hyperledger/cello/pull/231
* Automatic port assignment  by @XuHugo in https://github.com/hyperledger/cello/pull/232
* [#234]Add setting password to registration page by @fengyangsy in https://github.com/hyperledger/cello/pull/235
* [#236]Add the input organization name box to the login page by @fengyangsy in https://github.com/hyperledger/cello/pull/237
* Bump y18n from 3.2.1 to 3.2.2 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/238
* Add login and register interfaces by @XuHugo in https://github.com/hyperledger/cello/pull/240
* Bump nodemailer from 4.7.0 to 6.4.16 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/241
* Networkcreate by @XuHugo in https://github.com/hyperledger/cello/pull/242
* [#224 Add networklist page] by @fengyangsy in https://github.com/hyperledger/cello/pull/245
* Create organization and create node at the same time by @XuHugo in https://github.com/hyperledger/cello/pull/246
* Retire maintainer Tong Li by @yeasy in https://github.com/hyperledger/cello/pull/243
* Bump ws from 7.4.2 to 7.4.6 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/247
* [#248 Add create network page] by @fengyangsy in https://github.com/hyperledger/cello/pull/249
* create network and start by @XuHugo in https://github.com/hyperledger/cello/pull/250
* Fix #256 api-engine syntax error by @zhuyuanmao in https://github.com/hyperledger/cello/pull/257
* add repolint.json and fix incompatibility by @dexhunter in https://github.com/hyperledger/cello/pull/253
* [#issue-258]Modify the request address of the UI by @fengyangsy in https://github.com/hyperledger/cello/pull/259
* add portmap for docker agent by @dexhunter in https://github.com/hyperledger/cello/pull/255
* Channel by @XuHugo in https://github.com/hyperledger/cello/pull/260
* Bump lodash from 4.17.19 to 4.17.21 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/261
* Bump socket.io-parser from 3.3.0 to 3.3.2 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/262
* Debug the registration part of the front end by @XuHugo in https://github.com/hyperledger/cello/pull/263
* fix #264: fix swagger api doc loading error. by @zhuyuanmao in https://github.com/hyperledger/cello/pull/265
* The user logs in through the front page by @XuHugo in https://github.com/hyperledger/cello/pull/266
* Users use the front page to log in to cello by @XuHugo in https://github.com/hyperledger/cello/pull/267
* Channel by @XuHugo in https://github.com/hyperledger/cello/pull/270
* Use the front page to delete the agent by @XuHugo in https://github.com/hyperledger/cello/pull/271
* Modify the agent through the front page by @XuHugo in https://github.com/hyperledger/cello/pull/273
* Start cello using docker compose by @XuHugo in https://github.com/hyperledger/cello/pull/274
* Channel create endpoint by @zhuyuanmao in https://github.com/hyperledger/cello/pull/272
* Bump rsa from 4.6 to 4.7 in /src/api-engine by @dependabot in https://github.com/hyperledger/cello/pull/277
* Bump urllib3 from 1.26.2 to 1.26.5 in /src/api-engine by @dependabot in https://github.com/hyperledger/cello/pull/275
* Bump pyyaml from 5.3.1 to 5.4 in /src/api-engine by @dependabot in https://github.com/hyperledger/cello/pull/276
* Bump django from 3.1.3 to 3.1.12 in /src/api-engine by @dependabot in https://github.com/hyperledger/cello/pull/278
* Bump djangorestframework from 3.11.0 to 3.11.2 in /src/api-engine by @dependabot in https://github.com/hyperledger/cello/pull/281
* Bump jinja2 from 2.11.2 to 2.11.3 in /src/api-engine by @dependabot in https://github.com/hyperledger/cello/pull/282
* fix #279: fix relationship between channel and organization. by @zhuyuanmao in https://github.com/hyperledger/cello/pull/283
* Bump tar from 4.4.13 to 4.4.15 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/284
* Return value format by @XuHugo in https://github.com/hyperledger/cello/pull/285
* [#issue-286]Modify the agent management page by @fengyangsy in https://github.com/hyperledger/cello/pull/287
* [Issue #288]Modify the color of components by @fengyangsy in https://github.com/hyperledger/cello/pull/289
* Bump path-parse from 1.0.6 to 1.0.7 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/291
* fix agent bug by @XuHugo in https://github.com/hyperledger/cello/pull/292
* Modify node by @XuHugo in https://github.com/hyperledger/cello/pull/294
* [#issue-297]Modify page display and mock data by @fengyangsy in https://github.com/hyperledger/cello/pull/298
* Optimize network module by @XuHugo in https://github.com/hyperledger/cello/pull/299
* [#issue-300]Modify registration, login, and user roles by @fengyangsy in https://github.com/hyperledger/cello/pull/301
* Fix #290 Can not get JWT token from obtain_jwt_token view by @zhuyuanmao in https://github.com/hyperledger/cello/pull/296
* fix login by @XuHugo in https://github.com/hyperledger/cello/pull/303
* [#issue-302]add fabric cmdline lib by @tianxuanhong in https://github.com/hyperledger/cello/pull/304
* use threads to start nodes by @XuHugo in https://github.com/hyperledger/cello/pull/306
* added channel updating operation by @zhuyuanmao in https://github.com/hyperledger/cello/pull/307
* [#issue-313] cmdline lib function list and getinfo has no info return by @tianxuanhong in https://github.com/hyperledger/cello/pull/314
* add fabric tools by @XuHugo in https://github.com/hyperledger/cello/pull/310
* Bump tar from 4.4.15 to 4.4.19 in /build_image/dockerhub/v0.9.0/user-dashboard by @dependabot in https://github.com/hyperledger/cello/pull/312
* [#issue-317] cmdLineLib of chaincode operation by @tianxuanhong in https://github.com/hyperledger/cello/pull/318
* [#issue-320] lifecycle_query_installed&lifecycle_get_installed_package by @tianxuanhong in https://github.com/hyperledger/cello/pull/321
* [#issue-322]Modify the agent,network and node list to display abnorma… by @fengyangsy in https://github.com/hyperledger/cello/pull/323
* [#issue-319] There is a risk of obtaining expired information by @tianxuanhong in https://github.com/hyperledger/cello/pull/324
* create channel by @XuHugo in https://github.com/hyperledger/cello/pull/325
* [#issue-326] cmdlinelib feature of approveformyorg && queryapproved f… by @tianxuanhong in https://github.com/hyperledger/cello/pull/327
* [#issue-330] cmdlinelib implement of lifecycle_check_commit_readiness… by @tianxuanhong in https://github.com/hyperledger/cello/pull/331
* Bump sqlparse from 0.4.1 to 0.4.2 in /src/api-engine by @dependabot in https://github.com/hyperledger/cello/pull/329
* add template profile by @XuHugo in https://github.com/hyperledger/cello/pull/334
* [#issue-332] lifecycle_query_committed && invoke function by @tianxuanhong in https://github.com/hyperledger/cello/pull/333
* Bump django from 3.1.12 to 3.1.13 in /src/api-engine by @dependabot in https://github.com/hyperledger/cello/pull/335
* Implemented channel creating operation with peer channel cli. by @zhuyuanmao in https://github.com/hyperledger/cello/pull/328
* Download binary files in docker image building process.  by @zhuyuanmao in https://github.com/hyperledger/cello/pull/337
* LSI-32: Compiled code must not be in source repos by @ryjones in https://github.com/hyperledger/cello/pull/336
* Added ports number mapping feature when the agent created nodes. by @zhuyuanmao in https://github.com/hyperledger/cello/pull/339
* set source of pip by @XuHugo in https://github.com/hyperledger/cello/pull/342
* Refactor configtx and configtxgen by @zhuyuanmao in https://github.com/hyperledger/cello/pull/344
* Create a docker network by @zhuyuanmao in https://github.com/hyperledger/cello/pull/345
* Refactor channel creating and channel cmd. by @zhuyuanmao in https://github.com/hyperledger/cello/pull/346
* Change Fabric nodes naming  by @zhuyuanmao in https://github.com/hyperledger/cello/pull/347
* Correct the org field name and remove unused fields by @zhuyuanmao in https://github.com/hyperledger/cello/pull/348
* Add api requests examples in postman json format. by @zhuyuanmao in https://github.com/hyperledger/cello/pull/349
* Update quick start part of README by @zhuyuanmao in https://github.com/hyperledger/cello/pull/350
* Add postman collection and Update Channel model by @zhuyuanmao in https://github.com/hyperledger/cello/pull/352
* [#issue-353]Add Channel Page by @fengyangsy in https://github.com/hyperledger/cello/pull/354
* [#issue-355] There has a bug of Call cmd, need to be fixed by @tianxuanhong in https://github.com/hyperledger/cello/pull/356
* Let `make clean` clean db files by @yeasy in https://github.com/hyperledger/cello/pull/357
* [#issue-360]Add page to create channel by @fengyangsy in https://github.com/hyperledger/cello/pull/361
* Update maintainers by @yeasy in https://github.com/hyperledger/cello/pull/362
* Add API Response wrappers. by @zhuyuanmao in https://github.com/hyperledger/cello/pull/359
* [#363]Modify the page that created the node by @fengyangsy in https://github.com/hyperledger/cello/pull/364
* [#issue-365] Change the administrator to admin by @tianxuanhong in https://github.com/hyperledger/cello/pull/366
* [#issue-368] chaincode files upload by @tianxuanhong in https://github.com/hyperledger/cello/pull/369
* [#issue-374]network create failed: The front-end parameters are incon… by @fengyangsy in https://github.com/hyperledger/cello/pull/378
* [#issue-379] realize the chain code package function by @tianxuanhong in https://github.com/hyperledger/cello/pull/380
* [#issue-370]Modify front-end login module by @fengyangsy in https://github.com/hyperledger/cello/pull/371
* [#issue-373]Modify front-end channel module by @fengyangsy in https://github.com/hyperledger/cello/pull/375
* [#issue-385]Fix the problem of getting token by @fengyangsy in https://github.com/hyperledger/cello/pull/386
* [#issue-383]make dashboard image by @fengyangsy in https://github.com/hyperledger/cello/pull/384
* [#issue-387] implement chaincode install function by @tianxuanhong in https://github.com/hyperledger/cello/pull/388
* [#issue-389] implement query_installed & get_installed_package function by @tianxuanhong in https://github.com/hyperledger/cello/pull/391
* [#issue-393] implement lifecycle_approve_for_my_org function by @tianxuanhong in https://github.com/hyperledger/cello/pull/394
* [#issue-395] implement query_approved and check_commit_readiness func… by @tianxuanhong in https://github.com/hyperledger/cello/pull/396
* [#issue-402] implement commit function and modify channel config policy. by @tianxuanhong in https://github.com/hyperledger/cello/pull/403
* [#issue-406]Deleted the judgment of repeated password input in the re… by @fengyangsy in https://github.com/hyperledger/cello/pull/407
* [#issue-404]Add delete network function by @fengyangsy in https://github.com/hyperledger/cello/pull/405
* [#issue-408] implement chaincode list & query_committed function by @tianxuanhong in https://github.com/hyperledger/cello/pull/409
* [#issue-410]Add chaincode management page by @fengyangsy in https://github.com/hyperledger/cello/pull/411
* [#issue-412]Delete the dockefile of 0.9.0 version by @fengyangsy in https://github.com/hyperledger/cello/pull/413
* Remove hardcode for publishing ports of HLF nodes.  by @zhuyuanmao in https://github.com/hyperledger/cello/pull/400
* Fix node status after calling endpoints of node and network by @zhuyuanmao in https://github.com/hyperledger/cello/pull/420
* [#issue-423]Add upload chain code page by @fengyangsy in https://github.com/hyperledger/cello/pull/424
* Modify makefile by @zhuyuanmao in https://github.com/hyperledger/cello/pull/426
* Map api-engine data in docker container to local VM volume by @zhuyuanmao in https://github.com/hyperledger/cello/pull/425
* Fix node operations by @zhuyuanmao in https://github.com/hyperledger/cello/pull/428
* Fix node delete endpoint. by @zhuyuanmao in https://github.com/hyperledger/cello/pull/431
* Fix voulume mapping by @zhuyuanmao in https://github.com/hyperledger/cello/pull/430
* Add node status field to the response Node. by @zhuyuanmao in https://github.com/hyperledger/cello/pull/427
* Add node status field to get nodes list api response. by @zhuyuanmao in https://github.com/hyperledger/cello/pull/433
* [#issue-434] Add warning when deleting nodes by @fengyangsy in https://github.com/hyperledger/cello/pull/435
* [#issue-436]Add display node status by @fengyangsy in https://github.com/hyperledger/cello/pull/437
* Refine HLF node status by @zhuyuanmao in https://github.com/hyperledger/cello/pull/438
* Support M1 chip development. by @zhuyuanmao in https://github.com/hyperledger/cello/pull/444
* Clean api-engine and agent code. by @zhuyuanmao in https://github.com/hyperledger/cello/pull/446

## New Contributors
* @ryjones made their first contribution in https://github.com/hyperledger/cello/pull/25
* @yeasy made their first contribution in https://github.com/hyperledger/cello/pull/26
* @litong01 made their first contribution in https://github.com/hyperledger/cello/pull/28
* @Man-Jain made their first contribution in https://github.com/hyperledger/cello/pull/29
* @hightall made their first contribution in https://github.com/hyperledger/cello/pull/33
* @dependabot made their first contribution in https://github.com/hyperledger/cello/pull/58
* @fengyangsy made their first contribution in https://github.com/hyperledger/cello/pull/82
* @dexhunter made their first contribution in https://github.com/hyperledger/cello/pull/110
* @craig8 made their first contribution in https://github.com/hyperledger/cello/pull/117
* @MintCollie made their first contribution in https://github.com/hyperledger/cello/pull/124
* @spartucus made their first contribution in https://github.com/hyperledger/cello/pull/148
* @zhuyuanmao made their first contribution in https://github.com/hyperledger/cello/pull/257
* @tianxuanhong made their first contribution in https://github.com/hyperledger/cello/pull/304

**Full Changelog**: https://github.com/hyperledger/cello/commits/v1.0.0-alpha2
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/cello/releases/tag/v1.0.0-alpha2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-05-19 18:47:51 +0000 UTC
    </span>
</div>

