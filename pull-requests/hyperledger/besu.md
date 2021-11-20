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
                PR <a href="https://github.com/hyperledger/besu/pull/3087" class=".btn">#3087</a>
            </td>
            <td>
                <b>
                    Rename BftForkSpec to ForkSpec and make it generic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                ## PR description
This was split out of #3069. Changes the BftForkSpec to more generic concept so it can be reused in the QBFT migration.

* Rename BftForkSpec to ForkSpec
* Move from consenus.common.bft package in the consensus.common package
* Allow it to hold any value not just a BftConfigOption
* Rename getConfigOption to getValue

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 04:01:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3086" class=".btn">#3086</a>
            </td>
            <td>
                <b>
                    Removing the orion acceptance tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ORION is getting deprecated. There is no need to run these acceptance
tests any more.

Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

Fixes [3030](https://github.com/hyperledger/besu/issues/3030)

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 15:59:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3085" class=".btn">#3085</a>
            </td>
            <td>
                <b>
                    Adding support for NO_COLOR environment variable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding support of the NO_COLOR environment variable as described in
the [NO_COLOR](https://no-color.org/) standard.

The new behaviour looks like this:
1) Both NO_COLOR is not set and color-enabled options is not set => colors
will be enabled (by default we have colors on)

2) NO_COLOR is not set but color-enabled option is set to false =>
colors will be disabled (we can disable colors using an option)

3) NO_COLOR is set to any value and color-enabled option is not used =>
colors will be disabled (we can disable colors using an environment
variable this is new!)

4) NO_COLOR is set to any value but color-enabled option is set to true
=> colors will be enabled (an option has precedence over the environment
variable)

Signed-off-by: Jiri Peinlich <jiri.peinlich@gmail.com>

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

Fixes issue [1756](https://github.com/hyperledger/besu/issues/1756)

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 15:18:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3082" class=".btn">#3082</a>
            </td>
            <td>
                <b>
                    Fix admin_nodeInfo when response has jdk8 optional values
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

We were not handling JDK8 (de)serialization properly in our RPC services. This PR is using jackson-jdk8 module to handle Optional (de)serialization for responses.

This will ensure that serialization maps the value of Optional to null, if no value is present, or the wrapped value if present.

It does not make sense for the QBFT config to return null for the validator address and start block, so we are not including it into the json when these values are not present.

## Fixed Issue(s)
N/A

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-17 23:19:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3077" class=".btn">#3077</a>
            </td>
            <td>
                <b>
                    Step3 snap sync as client
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

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-17 14:38:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3076" class=".btn">#3076</a>
            </td>
            <td>
                <b>
                    Stream JSON RPC responses to avoid creating big JSON string in memory…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                … for large responses

Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

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
        Created At 2021-11-17 10:26:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3075" class=".btn">#3075</a>
            </td>
            <td>
                <b>
                    (internal) Refactor 'onchain' to 'flexible' where applicable
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
Pure variable/CLI option naming changes

## Fixed Issue(s)
Fixes #2960 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-17 06:14:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3073" class=".btn">#3073</a>
            </td>
            <td>
                <b>
                    Vert.x upgrade
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

Upgrades vert.x dependency. 

Notable areas of impact:

- Getting connections from an HTTP client is in itself asynchronous, so another layer of futures is added.
- The way keypairs are added to the JWTAuthProvider is different, and now they are configured using PEM strings.
- JWT attributes and principal fields are changed, for example exp (expiry) is a user attribute, not a principal property.


## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-16 19:23:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3071" class=".btn">#3071</a>
            </td>
            <td>
                <b>
                    Making sure that the resolved DNS lists get used in full
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

Previously we would always process the list of DNS resolved peers from the beginning. We would
at most only try `maxConnections` valid elements from the list and never try more. So the each
time we might be trying the same 25 peers, we connect with them and then drop them. This PR
firstly shuffles the peers list each time before applying it and then also takes from the list for
as long as there are free peers slots available as opposed to guess the limit upfront and hope
that all the peers connect.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-16 10:03:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3069" class=".btn">#3069</a>
            </td>
            <td>
                <b>
                    Qbft migration protocol schedule
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Create a combined protocol schedule for the QBFT migration that combines all the milestones from the delegate besu controllers protocol schedules.

fixes #2998  

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-16 03:30:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3068" class=".btn">#3068</a>
            </td>
            <td>
                <b>
                    Add Simon Dudley as a maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Simon has made significant [commits](https://github.com/hyperledger/besu/pulls?q=is%3Apr+author%3Asiladu) improving the quality and features of besu, this PR adds him as a maintainer.

Voting ends 2 weeks from the publication of this PR or once a majority of the maintainers vote.

For more information on this process see the Becoming a Maintainer section in the MAINTAINERS.md file.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-15 21:25:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3067" class=".btn">#3067</a>
            </td>
            <td>
                <b>
                    Prepare for 21.10.3-SNAPSHOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prepare snapshot 21.10.3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-15 20:33:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3066" class=".btn">#3066</a>
            </td>
            <td>
                <b>
                    21.10.2 release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                21.10.2 release
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-15 19:15:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3065" class=".btn">#3065</a>
            </td>
            <td>
                <b>
                    baseFee as Wei instead of long
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

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2785
## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-15 18:04:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3064" class=".btn">#3064</a>
            </td>
            <td>
                <b>
                    Adding filechannel name to the exception
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

Updating exception to contain some information about what file had problem with I/O. I got this exception several times on a disk that was not an SSD and without this information it was difficult to find out what the problem was. 

<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-15 17:29:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3061" class=".btn">#3061</a>
            </td>
            <td>
                <b>
                    [MINOR] typo - connection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

fixed a typo

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-15 10:34:57 +0000 UTC
    </div>
</div>

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

