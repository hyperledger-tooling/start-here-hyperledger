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
                PR <a href="https://github.com/hyperledger/besu/pull/2783" class=".btn">#2783</a>
            </td>
            <td>
                <b>
                    Snapsync get list  of accounts in range
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
        Created At 2021-09-20 08:14:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2782" class=".btn">#2782</a>
            </td>
            <td>
                <b>
                    Feature/merge execute payload
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
* implements engine_executePayload
* rename and repurpose rayonism options & flag
* treat the merge as another consensus mechanism:
  * add a `merge` consensus gradle subproject 
  * create MergeBesuController
  * create MergeProtocolSchedule 
  * create MergeContext for merge-specific consensus context
  * create MergeHeaderValidationRuleFactory for merge specific header validation rules
  * create MergeUnfinalizedValidationRule, attempt to enforce finalized block rules for import


## Fixed Issue(s)
protocol-misc 476 
protocol-misc 485

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-20 06:00:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2779" class=".btn">#2779</a>
            </td>
            <td>
                <b>
                    Create new datatypes module for Address, Hash, and Wei
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Create a new `datatypes` module to hold datatypes that are broadly used.
This will aid modularization by making sure the base types in the module
minimize the amount of unrelated support classes needed.

Move the Address, Hash, and Wei to datatypes in as they are needed for
EVM modularization.

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-17 14:34:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2774" class=".btn">#2774</a>
            </td>
            <td>
                <b>
                    fix RC1-SNAPSHOT release version 🤦‍♂️
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
add missing -SNAPSHOT to gradle.properties build version

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 19:12:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2773" class=".btn">#2773</a>
            </td>
            <td>
                <b>
                    prepare for 21.10.0-RC1
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

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
bump build version and changelog to reflect next quarterly release candidate 

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 17:35:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2772" class=".btn">#2772</a>
            </td>
            <td>
                <b>
                    Release 21.7.4
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
        Created At 2021-09-16 16:07:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2771" class=".btn">#2771</a>
            </td>
            <td>
                <b>
                    CHANGELOG: moved experimental features
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Moved QBFT experimental features to the "Early access features" section

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 23:58:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2770" class=".btn">#2770</a>
            </td>
            <td>
                <b>
                    Changelog for 21.7.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move entires that were mistakenly added to 21.7.3 lists to 21.7.4.
Add entry for ETC gas calculator bug.

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 21:30:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2769" class=".btn">#2769</a>
            </td>
            <td>
                <b>
                    Add additional minimum merge spec stubs  #474
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
* Stub out additional [minimum merge spec](https://gist.github.com/mkalinin/e26f1fe70df83a25834cc6a62b6afdac)  endpoints 



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 19:51:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2768" class=".btn">#2768</a>
            </td>
            <td>
                <b>
                    Proposal for breaking change to the way plugins load cli options
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Description 

https://wiki.hyperledger.org/display/BESU/DRAFT+-+Pico+CLI+Plugin+Integration

The main change is to move preparePlugins into the begging of the run method. This means that all the cli parsing will happen before any plugins are called. The only way to register cli options will be to have them on the `BesuPlugin` e.g

https://github.com/hyperledger/besu/pull/2768/files#diff-2080ac0bf38c1e492921f4191b738b729195e0b1ad82657abc9103f19ac87cd8L1195

```
@AutoService(BesuPlugin.class)
public class MyPlugin implements BesuPlugin {

  @Option(
    names = {"--Xplugin-my-option"},
    defaultValue = "foo")
  String myOption;

  @Override
  public Optional<String> getName() {
    return Optional.of("my");
  }
}
```

The other breaking change is that you should override getName and provide a meaningful plugin name. This is used for the namespace when registering the cli arguments.

https://github.com/hyperledger/besu/pull/2768/files#diff-2080ac0bf38c1e492921f4191b738b729195e0b1ad82657abc9103f19ac87cd8R1204



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 14:39:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2763" class=".btn">#2763</a>
            </td>
            <td>
                <b>
                    Stub out new execution endpoint api, #474
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update json-rpc consensus API (474)
* change rpc endpoint to engine_* rather than consensus_*
* split consensus_assembleBlock into engine_preparePayload and engine_getPayload
* engine_preparePayload should be stubbed to return a success response
* engine_getPayload should repurpose consensus_assembleBlock

stub out:
* engine_executePayload
* engine_consensusValidated
* engine_forkChoiceUpdated

remove/repurpose:
* consensus_finalizeBlock
* consensus_newBlock
* consensus_setHead
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 00:01:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2761" class=".btn">#2761</a>
            </td>
            <td>
                <b>
                    Gradle 7.2 upgrade / Java 17 Build Support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Upgrade to Gradle 7.2, which supports Java 17
* Regenerate gradlew script and wrapper (as recommended)
* Suppress the removal warning for `AccessController` for now
* Update the JMH version to get rid of Gradle deprecation warning
* Add spotless `targetExcludes` so it won't re-format submodules

Signed-off-by: Danno Ferrin <danno.ferrin@gmail.com>

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 17:54:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2758" class=".btn">#2758</a>
            </td>
            <td>
                <b>
                    [MINOR] typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

Fixed a typo

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 04:04:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2754" class=".btn">#2754</a>
            </td>
            <td>
                <b>
                    Allow Besu to host RPC endpoints via a plugin.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                ## PR description
re-implementation of https://github.com/PegaSysEng/pantheon/pull/1909/


Implements https://github.com/hyperledger/besu/issues/1317

You can now register endpoints using

```
context
  .getService(RpcEndpointService.class)
  .get()
  .registerRPCEndpoint("namespace", "method", request -> {
    return "any serializable response";
  });
```
To enable the endpoint you must utilise `--rpc-http-api` and specify the namespace e.g `--rpc-http-api namespace`.


## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 14:56:33 +0000 UTC
    </div>
</div>

