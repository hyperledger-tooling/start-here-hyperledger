---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1007" class=".btn">#1007</a>
            </td>
            <td>
                <b>
                    Feat object store plugin ipfs
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
        Created At 2021-06-03 05:48:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1005" class=".btn">#1005</a>
            </td>
            <td>
                <b>
                    test(connector-fabric): upgrade Fabric AIO image tag used for test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Fabric</span>
            </td>
            <td>
                Upgraded from the image build in March 2021 to the one in April which
is believed to be more stable making this change potentially viable as
a soltuion to the flakes that we've been observing during test execution
when the AIO image fails to boot.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-01 17:21:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1004" class=".btn">#1004</a>
            </td>
            <td>
                <b>
                    fix(readthedocs): updated readthedocs file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolve #981 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-01 08:41:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1001" class=".btn">#1001</a>
            </td>
            <td>
                <b>
                    fix(validator,verifier): delete some minor duplicated documents
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolve #1002 

Signed-off-by: Takuma TAKEUCHI <takeuchi.takuma@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-31 10:50:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/999" class=".btn">#999</a>
            </td>
            <td>
                <b>
                    fix(tools): fix a typo of README on iroha-testnet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolve #1000 
cc: @tkyonezu 

Signed-off-by: Takuma TAKEUCHI <takeuchi.takuma@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-31 10:08:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/998" class=".btn">#998</a>
            </td>
            <td>
                <b>
                    refactor(examples): refactor electricity-trade in order to allow BLP connects ledgers only via Verifier and Validator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                resolve #970 

contents:
 - modify electricity-trade in order to allow BLP not to direcly call getNonceHex but to call getNonceHex via Verifier and Validator

Signed-off-by: Takuma TAKEUCHI <takeuchi.takuma@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-31 09:50:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/996" class=".btn">#996</a>
            </td>
            <td>
                <b>
                    build: migrate dev container to Ubuntu 20; add nvm to image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">dependencies</span>
            </td>
            <td>
                Primary change:
--------------

The Debian 10 to Ubuntu 20.04 LTS move

This came up when I tried to install the DFINITY SDK which failed due to
some GLIB C version mismatch which was not possible to get resolved
on Debian Buster (v10) without upgrading to the not-yet-stable version
11 (Bullseye).

While going through the above, I also realized that our CI uses
Ubuntu 20.04 so it would be great to have consistency across the board
when it comes OS versions. This will become even more important when
we start adding microk8s in the mix as well (hopefully soon).

Secondary change:
-----------------

build: include node version manager (nvm) to .devcontainer

The need for this dawned on me when I pulled up a fresh dev
container, tried to run the configure script that failed because
the current latest NodeJS (v16) was installed by apk and the
build could not handle that
We have a pending PR for this separately at the time of this
writing, but to make it easier to work around issues like this
in the future, nvm should be in the image should that people
can just do nvm use 14 for example. (which is what the fix
was in my case).

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-28 21:27:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/994" class=".btn">#994</a>
            </td>
            <td>
                <b>
                    test: container shutdown hook prior to starting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span>
            </td>
            <td>
                ## Dependencies

Depends on #993 

## Commit to review

Author: Peter Somogyvari <peter.somogyvari@accenture.com>
Committer: Peter Somogyvari <peter.somogyvari@accenture.com>
Date: Fri May 28 2021 00:04:09 GMT-0700 (Pacific Daylight Time) 

test: container shutdown hook prior to starting

Figured out from the additional logs we recently added that
the reason why the Fabric 1.4.x AIO image fails to start for
the 1.4.x tests is because a previously ran test (2.x)
crashes and never stops it's container which then ends up
hogging the ports which cannot be randomized for the
Fabric AIO images yet.

So, adding more logging here and also ensuring that the
test finish hooks that are responsible for shutting down
the containers are registered prior to calling
the start method on the test container classes so that
if the start method hangs the container will still go
away as it should.

This is what gave me the clue from the CI logs:

    # BEFORE runs tx on a Fabric v2.2.0 ledger
    Detected current process to be running inside a Github Action. Pruning all docker resources...
    [2021-05-28T01:23:31.310Z] DEBUG (Containers#pruneDockerResources()): Finished pruning all docker resources. Outcome: {
      containers: { ContainersDeleted: null, SpaceReclaimed: 0 },
      images: { ImagesDeleted: null, SpaceReclaimed: 0 },
      networks: { NetworksDeleted: null },
      volumes: {
        VolumesDeleted: [
          '10afa6c6071a4e362324ec7eaabedbbee088dedc0b0e182880ca4ccc6430b998',
          [length]: 1
        ],
        SpaceReclaimed: 1915254089
      }
    }
    ok 1 Pruning didn't throw OK
    # runs tx on a Fabric v2.2.0 ledger
    # test count(1) != plan(null)
    # failed 1 test
not ok 62 - packages/cactus-plugin-ledger-connector-fabric/src/test/typescript/integration/fabric-v2-2-x/run-transaction-endpoint-v1.test.ts # time=3600276.779ms

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-28 07:13:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/993" class=".btn">#993</a>
            </td>
            <td>
                <b>
                    ci: delete Android SDK, .NET in GitHub Action runners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">dependencies</span>
            </td>
            <td>
                This is a workaround for the warnings that we've been getting
about the disk of the GHA runners being full. 

The trick is to delete the Android SDK and .NET from the runner
because we don't need any of those and it gives us a cozy 30 GB
extra space to play with which should be more than enough for
the foreseeable future.

The idea comes from:
https://github.com/actions/virtual-environments/issues/2606#issuecomment-772683150

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 21:06:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/991" class=".btn">#991</a>
            </td>
            <td>
                <b>
                    feat(azure-kv): added keychain plugin for azure keyvault
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Commit to be reviewed
------------------------------
feat(azure-kv): added keychain plugin for azure keyvault

        Primary Change
        ---
        1. Added new package cactus-plugin-keychain-azure-kv under packages/
        2. Added PluginKeychainAzureKvMock class to mock the functions of SecretClient under packages/cactus-plugin-keychain-azure-kv/src/test/typescript/mock/plugin-keychain-azure-kv-mock.ts

Resolves #971

Signed-off-by: Jagpreet Singh Sasan <jagpreet.singh.sasan@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 09:49:44 +0000 UTC
    </div>
</div>

