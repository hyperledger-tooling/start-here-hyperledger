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
                PR <a href="https://github.com/hyperledger/besu/pull/2452" class=".btn">#2452</a>
            </td>
            <td>
                <b>
                    Fix vulnerabilities from openjdk-11 base image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR aims to fix the Issue [2451](https://github.com/hyperledger/besu/issues/2451) reported about base image vulnerabilities.

Now scan report does not show any high vulnerabilities:
```
docker scan -f docker/openjdk-11/Dockerfile docker.io/hyperledger/besu:21.7.0-RC1-SNAPSHOT-openjdk-11 --severity high

Testing docker.io/hyperledger/besu:21.7.0-RC1-SNAPSHOT-openjdk-11...

Organization:      juan.dominguez
Package manager:   deb
Target file:       docker/openjdk-11/Dockerfile
Project name:      docker-image|docker.io/hyperledger/besu
Docker image:      docker.io/hyperledger/besu:21.7.0-RC1-SNAPSHOT-openjdk-11
Base image:        adoptopenjdk/openjdk11:x86_64-ubuntu-jre-11.0.11_9
Licenses:          enabled

✓ Tested 132 dependencies for known issues, no vulnerable paths found.
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-18 16:29:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2449" class=".btn">#2449</a>
            </td>
            <td>
                <b>
                    Qbft duplicate prepares in roundchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
Fix duplicate prepares being included the roundchange message which is invalid.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-18 06:48:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2448" class=".btn">#2448</a>
            </td>
            <td>
                <b>
                    dialing down logging of invalid HELO to debug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin.florentine@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
[Previous assumption](https://github.com/hyperledger/besu/pull/2406#discussion_r649821858) was a mistake, I didn't realize those canaries I checked were not running at DEBUG. Invalid HELOs happen often enough, without any impact, that the log level should remain at debug.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2004 
## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 14:34:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2447" class=".btn">#2447</a>
            </td>
            <td>
                <b>
                    update changelog
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-16 15:43:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2445" class=".btn">#2445</a>
            </td>
            <td>
                <b>
                    Update eth call post 1559
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

Update eth_call to work correctly after the london fork 

Update integration tests to be able to test JSON RPC methods after the london fork

**Explained behavior :**

- Before EIP1559
     - If gasPrice is not present. 0 is used and balance account is not checked
     - If gasPrice is present. this gasPrice value is used and balance account is checked

- After EIP1559
     - If gasPrice is not present. 0 is used and balance account is not checked (baseFee forced to 0)
     - if gasPrice is present, this value is used for the max and priority fee and the balance is checked (the current baseFee is used)
     - if max and/or priority fee are present, they are interpreted as specified and the balance is checked  (the current baseFee is used)

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-16 14:29:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2444" class=".btn">#2444</a>
            </td>
            <td>
                <b>
                    Fix version for release 21.7.0 branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

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
        Created At 2021-06-16 13:52:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2440" class=".btn">#2440</a>
            </td>
            <td>
                <b>
                    Prepare for version 21.7.0-RC2-SNAPSHOT
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
        Created At 2021-06-15 17:27:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2438" class=".btn">#2438</a>
            </td>
            <td>
                <b>
                    Release 21.7.0-RC1
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
        Created At 2021-06-15 16:50:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2434" class=".btn">#2434</a>
            </td>
            <td>
                <b>
                    ensure test_importRawBlock appends to chain head
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
Ensures `test_importRawBlock` appends the block to the chain even if the block already exists in storage.  This behavior is limited to the test endpoint, rather than pushing it down into the block importer.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#2409 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-15 06:16:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2433" class=".btn">#2433</a>
            </td>
            <td>
                <b>
                    Include custom errorprone checks as external dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Include custom errorprone checks as external dependency. Custom errorprone checks has been refactored to its own repo https://github.com/Consensys/errorprone-checks. 

This change will allow to use custom errorprone checks in other projects as well.

Signed-off-by: Usman Saleem <usman@usmans.info>

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-15 02:01:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2432" class=".btn">#2432</a>
            </td>
            <td>
                <b>
                    eth_feeHistory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The spec for this implementation is listed in the issue below.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2430 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-14 22:37:13 +0000 UTC
    </div>
</div>

