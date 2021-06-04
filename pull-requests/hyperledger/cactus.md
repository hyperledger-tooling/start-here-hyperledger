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
                PR <a href="https://github.com/hyperledger/cactus/pull/1008" class=".btn">#1008</a>
            </td>
            <td>
                <b>
                    Fixed cleanup.sh script according to the requirements, squashed to a single commit.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Konstantin Rybalko <konstantin.rybalko@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-03 12:25:37 +0000 UTC
    </div>
</div>

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

