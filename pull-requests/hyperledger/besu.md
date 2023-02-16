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
                PR <a href="https://github.com/hyperledger/besu/pull/5096" class=".btn">#5096</a>
            </td>
            <td>
                <b>
                    updates to latest version of kzg wrapper
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Sadly this does not get us any finer grained error reasons, and that seems intentional.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-15 21:58:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5095" class=".btn">#5095</a>
            </td>
            <td>
                <b>
                    Only use MAINNET version of KZG
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

Since we are only going to use the MAINNET preset of the KZG native lib, simplify the code to remove the logic to select the preset.
All unit tests have been ported to the MAINNET setup.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [x] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-15 15:24:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5093" class=".btn">#5093</a>
            </td>
            <td>
                <b>
                    Burn in build of 23.1.0
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
burn-in release of 23.1.0 onto  [RC2](https://github.com/hyperledger/besu/tree/23.1.0-RC2) tag
* cherry pick of #5076
* consolidated changelog

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-14 20:08:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5092" class=".btn">#5092</a>
            </td>
            <td>
                <b>
                    Allow other users to read the /opt/besu dir when using docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

Same issue existed on Teku: https://github.com/ConsenSys/teku/pull/6740 

## PR description

Can't use the docker image when running it with another user than root or `1000`.

```sh
$ docker pull consensys/besu 

# Running as root
$ docker run --rm -it --entrypoint ls  consensys/besu 
LICENSE  besu.autocomplete.sh  bin  lib  license-dependency.html 

# Running as user 1000 
$ docker run --rm -it --entrypoint ls --user=1000  consensys/besu 
LICENSE  besu.autocomplete.sh  bin  lib  license-dependency.html

# Running as user 1003
$ docker run --rm -it --entrypoint ls --user=1003  consensys/besu 
ls: cannot open directory '.': Permission denied
```

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-14 18:44:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5091" class=".btn">#5091</a>
            </td>
            <td>
                <b>
                    Temporary embed devnet 4 trusted setup until a configuration option is available
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

Temporary embed devnet 4 trusted setup until a configuration option is available. Proper solution being worked on PR https://github.com/hyperledger/besu/pull/5084

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-14 13:19:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5090" class=".btn">#5090</a>
            </td>
            <td>
                <b>
                    [MINOR] Allow dashes in ethstats password
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
        Created At 2023-02-14 08:12:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5088" class=".btn">#5088</a>
            </td>
            <td>
                <b>
                    Add shanghaiTime to sepolia
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span><span class="chip">EIP</span>
            </td>
            <td>
                Announced here: https://github.com/ethereum/execution-specs/pull/716

Move timestamp forks from getForkBlockNumbers to getForkBlockTimestamps in JsonGenesisConfigOptions - this ultimately gets used to popoulate the ForkIdManager which handles lists of blocks and timestamps the same way so this hasn't changed any actual behaviour, but rather supports the test fixes.

Implement TransitionProtocolSchedule.streamMilestoneBlocks as a concatenation of blockNumbers++blockTimestamps. This may have been a latent bug since it's used to update the node record when a fork transition occurs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-10 22:53:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5084" class=".btn">#5084</a>
            </td>
            <td>
                <b>
                    Initialize KZG native lib at startup if Cancun is enabled
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Move c-kzg native lib initialization at startup, when all the other native lib are configured, and also because it is not only used by the precompile, but also for transaction validation.
Added the option `--kzg-trusted-setup` to pass a custom setup file for custom networks or to override the default one for named networks


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [x] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-10 14:07:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5083" class=".btn">#5083</a>
            </td>
            <td>
                <b>
                    reintroduce checking of block height for certain tasks when we are not PoS (Revert PR#3911)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span><span class="chip">peering</span>
            </td>
            <td>
                fixes issue #5061

Signed-off-by: Stefan <stefan.pingel@consensys.net>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-10 07:01:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5082" class=".btn">#5082</a>
            </td>
            <td>
                <b>
                    Differentiate proposed bad blocks from imported bad block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Gabriel Fukushima <gabrielfukushima@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
This PR uses a new parameter to distinguish between bad imported blocks vs bad proposed blocks. 
Main objective is stop adding proposed bad blocks to the badBlockManager.

Tested on local devnet beku + txfuzzer

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #5058 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [x] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-10 06:21:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5081" class=".btn">#5081</a>
            </td>
            <td>
                <b>
                    Fix PoS checkpoint validation
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
Fixes the experimental PoS checkpoint edge case where PoS blocks have same TD than TTD 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [x] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-10 05:51:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5077" class=".btn">#5077</a>
            </td>
            <td>
                <b>
                    moves check for init code length before balance check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Justin Florentine <justin+github@florentine.us>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [X] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-09 21:46:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5076" class=".btn">#5076</a>
            </td>
            <td>
                <b>
                    Fix Layered World State issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>
Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

We found the problem :

During a remember block we added a copy of the worldstate during the saveTrieLog in order to fix the get balance == 0. By making a copy we have a BonsaiInMemoryWorldstate which does not persist the trielog in rocksdb. We saw the log that tells us that we can’t commit. 
The problem is that during a FCU when we persist a block if we have a reorg we finally save the trielog after the different Rollback / Forward. Because of that we do not save a valid log. Instead of saving a Trielog for 1 to 2 bis we have a Trielog which is a mix of 2-1 + 1-2bis . This happens because it is not normal  to not already have the trielog in base during a reorg.

Because of that we can't rollback/rollfoward anymore with this invalid trielog so we have the layered copy worldstate error

The worldstate copy is not really needed and we decided to not create a copy and to subscribe to the worldstateStorage directly in the BonsaiLayeredWorldstate.

This fixed was not fixing yet the problem because we had another problem. During a getAccount we are getting the BonsaiLayeredWorldstate and we are closing this one after the getAccount. Because of that we are unsubscribing the worldstateStorage and losing the instance. to fix that we decided to use the same code we re using for the validate/transaction pool etc and to create a copy of the layeredWorldstate instead 

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-09 21:45:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5075" class=".btn">#5075</a>
            </td>
            <td>
                <b>
                    [4844] Fix GetBlobBundleV1 response
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

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Acceptance Tests (Non Mainnet)

- [ ] I have considered running `./gradlew acceptanceTestNonMainnet` locally if my PR affects non-mainnet modules.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-09 11:59:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5073" class=".btn">#5073</a>
            </td>
            <td>
                <b>
                    Revert "Keep Worldstate Storage open for Bonsai archive latest layer (#5039)"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit e7150102ea208165ac29bd10986fe26bc9e176d0.

This is causing "Unable to copy Layered Worldstate" errors affecting canary nodes, devnets and the 23.1.0 burn-in
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-09 03:15:39 +0000 UTC
    </div>
</div>

