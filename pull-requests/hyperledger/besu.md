---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3059" class=".btn">#3059</a>
            </td>
            <td>
                <b>
                    Remove redundant method and associated tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger/besu/issues/3038

Signed-off-by: Simon Dudley <simon.dudley@consensys.net>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-15 04:55:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3058" class=".btn">#3058</a>
            </td>
            <td>
                <b>
                    [2982] Handle operation not permitted exception (firewall)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Frank Li <b439988l@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Hide these exceptions to DEBUG logging level as per https://github.com/hyperledger/besu/issues/2982

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #2982

## Changelog

Don't need changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-15 02:31:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3057" class=".btn">#3057</a>
            </td>
            <td>
                <b>
                    Feature/keep peers on dns fail
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
* Address dns discovery failures by *not* overwriting the dns peers list when discovery returns an empty list.  
* Add a cli parameter `--Xp2p-dns-discovery-server` to override the default dns server if the dns default dns server is unreliable or does not serve TCP dns requests

example using cloudflare DNS:
`besu --Xp2p-dns-discovery-server=1.1.1.1`

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-13 04:23:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3055" class=".btn">#3055</a>
            </td>
            <td>
                <b>
                    fix toml parsing of Long option types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Fix toml config file parsing for options that map to type Long or long.  Previously setting a value in toml config for a long option type would result in, e.g. :
```org.apache.tuweni.toml.TomlInvalidTypeException: Value of 'Xbonsai-maximum-back-layers-to-load' is a integer```


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-12 22:15:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3054" class=".btn">#3054</a>
            </td>
            <td>
                <b>
                    Add Diego López León to maintainers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Antoine Toulme <antoine@lunar-ocean.com>

## PR description

Diego has made significant [commits](https://github.com/hyperledger/besu/pulls?q=is%3Apr+author%3Adiega) improving the quality and features of besu, this PR adds him as a maintainer.

Voting ends 2 weeks from the publication of this PR or once a majority of the maintainers vote.

For more information on this process see the Becoming a Maintainer section in the MAINTAINERS.md file.

## Fixed Issue(s)

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-12 21:06:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3052" class=".btn">#3052</a>
            </td>
            <td>
                <b>
                    add Fabio as a maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Fabio has made significant [commits](https://github.com/hyperledger/besu/pulls?q=is%3Apr+author%3Afab-10) improving the quality and features of besu, this PR adds him as a maintainer.

Voting ends 2 weeks from the publication of this PR or once a majority of the maintainers vote.

For more information on this process see the Becoming a Maintainer section in the MAINTAINERS.md file.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-12 19:24:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3051" class=".btn">#3051</a>
            </td>
            <td>
                <b>
                    Retrieve ENR via RPC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Lehrner <daniel.lehrner@consensys.net>

## PR description
Adds the Ethereum Node Record to the `admin_nodeInfo` RPC call. This is not final and could be changed as an alternative solution could be to create a new endpoint.

## Fixed Issue(s)
fixes #3050 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-12 14:46:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3049" class=".btn">#3049</a>
            </td>
            <td>
                <b>
                    3038 clean up
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cleanup for https://github.com/hyperledger/besu/issues/3038 (following the first related PR https://github.com/hyperledger/besu/pull/3043)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-12 10:56:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3048" class=".btn">#3048</a>
            </td>
            <td>
                <b>
                    Create stub ForkingBesuControllerBuilder with no migration capabilities
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Paving the way for the work on IBFT2 to QBFT migration.

- Created `startBlock` option for `QbftConfig`
- Created skeleton `ForkingBesuControllerBuilder`

fixes #2997
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-12 03:24:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3047" class=".btn">#3047</a>
            </td>
            <td>
                <b>
                    add more logging for get blocks form peers task
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #3010

Signed-off-by: Stefan Pingel <stefan.pingel@consensys.net>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-12 01:19:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3043" class=".btn">#3043</a>
            </td>
            <td>
                <b>
                    Require blockheader mode validators
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A runtime is thrown at startup if this requirement is not met.

A second PR will remove some now redundant complexity in ForkingValidatorProvider

https://github.com/hyperledger/besu/issues/3038
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 12:38:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3042" class=".btn">#3042</a>
            </td>
            <td>
                <b>
                    deprecation: replace calls to isEqualToComparingFieldByField 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span><span class="chip">TeamRevenant</span>
            </td>
            <td>
                with usingRecursiveComparison().isEqualTo

Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Simple find and replace. 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 06:57:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3041" class=".btn">#3041</a>
            </td>
            <td>
                <b>
                    Updating the jacoco toolVersion
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Jacoco failed to instrument some tests using the old version of the tool
when build under jdk17

Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

Fixes #3040

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 06:26:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3039" class=".btn">#3039</a>
            </td>
            <td>
                <b>
                    Shift Optimization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Reduce shift calculations to shifts that may have an actual result.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>


## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 05:50:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3037" class=".btn">#3037</a>
            </td>
            <td>
                <b>
                    Maintainers: move to emeritus x 3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

I propose moving the following maintainers to Emeritus status, pursuant to the inactivity clause. These maintainers have had no activity during Q3 2021 (since July 2021):
* @edwardmac - last commit was in Nov 2020
* @rain-on - last commit was in Mar 2021
* @davemec - last commit was in May 2021

We very much appreciate their contributions but moving their status to emeritus (and thus revoking PR approval privileges) is in the interest of an orderly project. If any of these maintainers express in this PR that they intend to make contributions in the next quarter, then they will not be moved to emeritus status.
I propose this vote be open until either an absolute majority of active maintainers (13) votes for the same outcome, or until two weeks has passed (25 Nov 2021), after which a voting majority will determine the outcome (with a tie resulting in no change).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 04:32:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3036" class=".btn">#3036</a>
            </td>
            <td>
                <b>
                    [MINOR] updated comment and added link to generateId code in Tessera
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">privacy</span><span class="chip">TeamRevenant</span>
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Added link to relevant Tessera code for generating privacy group ID

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 01:58:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3035" class=".btn">#3035</a>
            </td>
            <td>
                <b>
                    Fix sepolia copypasta
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
fix incorrect discovery port on geth sepolia config


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 19:36:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3034" class=".btn">#3034</a>
            </td>
            <td>
                <b>
                    Update Sepolia bootnode, peer logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
* update sepolia bootnode to reflect EF's new sepolia boot node
* add peer details to debug logging


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 17:11:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3033" class=".btn">#3033</a>
            </td>
            <td>
                <b>
                    Fix dns discovery issue 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

We are creating but not starting the dns discovery daemon. After this modification the node find peers instantly.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 16:58:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3032" class=".btn">#3032</a>
            </td>
            <td>
                <b>
                    improve perf trace
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 13:10:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3031" class=".btn">#3031</a>
            </td>
            <td>
                <b>
                    [MINOR] add download link for 21.10.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

added download link and hash for 21.10.1

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 08:27:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3027" class=".btn">#3027</a>
            </td>
            <td>
                <b>
                    [3026] Updating version of disovery dependency 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
The discovery dependency is responsible for handling the v5 version of the discovery process of peers. This PR is updating the version to the latest. The project changed versioning after 0.5.0. The following version was 21.10.0 as can be seen on
the [release page](https://github.com/ConsenSys/discovery/releases).
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3027 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 10:33:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3025" class=".btn">#3025</a>
            </td>
            <td>
                <b>
                    [3011] Calling SignatureAlgorithmFactory::resetInstance before test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
The NodeKeyTest might fail in case the SignatureAlgorithmFactory has an
instance already set from some previous test.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
fixes #3011 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 10:23:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3024" class=".btn">#3024</a>
            </td>
            <td>
                <b>
                    Prepare for 21.10.2-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

gradle.properties to 21.10.2-SNAPSHOT version
and added placeholder in changelog

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 04:48:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3023" class=".btn">#3023</a>
            </td>
            <td>
                <b>
                    Release 21.10.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 01:57:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3022" class=".btn">#3022</a>
            </td>
            <td>
                <b>
                    Maintainer: add Taccat Isid 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

I propose to add @taccatisid as a Besu project maintainer.

@taccatisid has contributed with many high quality commits:

Here are their past contributions on Besu project
- https://github.com/hyperledger/besu/pull/2644
- https://github.com/hyperledger/besu/pull/2674
- https://github.com/hyperledger/besu/pull/2717
- https://github.com/hyperledger/besu/pull/2805
- https://github.com/hyperledger/besu/pull/2956

<!-- for non-code contributors -->
@taccatisid also contributed with many high quality actions:

Quality code reviews eg 
- https://github.com/hyperledger/besu/pull/2994
- https://github.com/hyperledger/besu/pull/2971

Voting ends 2 weeks from the publication of this PR or once a majority of the maintainers [vote](https://github.com/hyperledger/besu/blob/main/MAINTAINERS.md#maintainers-approval-process).

For more information on this process see the Becoming a Maintainer section in the MAINTAINERS.md file.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 20:38:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3021" class=".btn">#3021</a>
            </td>
            <td>
                <b>
                    Fix a double execution of the same method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

description in https://github.com/hyperledger/besu/issues/3020

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #3020

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 18:09:46 +0000 UTC
    </div>
</div>

