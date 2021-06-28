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
                PR <a href="https://github.com/hyperledger/cactus/pull/1099" class=".btn">#1099</a>
            </td>
            <td>
                <b>
                    feat(validator): Indy validator and indy-testnet files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added new code that talks to indy pool. It submits request to indy it received and sends response back.
The python code will be updated in the future so that users can simply pip install them and run (although it is incomplete at the moment). The directory structure reflects this intention.

Also included are updated version of indy-testnet files. The code described above needs this environment to properly run.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-28 11:35:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1095" class=".btn">#1095</a>
            </td>
            <td>
                <b>
                    test(test-tooling): containers#pruneDockerResources prints disk usage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span>
            </td>
            <td>
                Also adds a timeout and a log level parameter to the containers#exec
utility function to improve the developer experience while
troubleshooting test failures related to containers.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 21:48:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1094" class=".btn">#1094</a>
            </td>
            <td>
                <b>
                    test: call pruneDockerAllIfGithubAction in test.onFinish handler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span>
            </td>
            <td>
                This may or may not make a difference with the flaky tests (the theory
is that it does).

Why? I noticed that one of the random test failures we have happens
when the test container's stop+destroy calls in the finish handler are
not being awaited for by the test runner internally before starting a
new test case in the same test file.
This lead to situations where a race appeared to cause crashes because
the pruning began before the container could gracefully shut itself
down.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 21:32:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1093" class=".btn">#1093</a>
            </td>
            <td>
                <b>
                    test: migrate AIO images to the GitHub Container Registry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span>
            </td>
            <td>
                This will help solve the rate limiting problems we've been having
with DockerHub lately.

Still have to figure out automatic builds as part of the CI, but for
now at least we have the most heavily used images (manually)
uploaded to GHCR so that the tests can use it.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 21:24:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1092" class=".btn">#1092</a>
            </td>
            <td>
                <b>
                    ci(tools): ci.sh prints disk usage between test runs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span>
            </td>
            <td>
                This will be useful to detect cases of tests failing only because the
disk was full and not because the tests themselves had a bug in them.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-25 21:07:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1091" class=".btn">#1091</a>
            </td>
            <td>
                <b>
                    style(linter): multiple linter fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span>
            </td>
            <td>
                Signed-off-by: Youngone Lee <youngone.lee@accenture.com>

@petermetz ping for review, this is a large group of linter warning fixes. If it was better to break them apart for next time please let me know! ⭐ 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 16:48:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1090" class=".btn">#1090</a>
            </td>
            <td>
                <b>
                    feat(connector-besu): add getBlock web service #1065
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Besu</span><span class="chip">enhancement</span>
            </td>
            <td>
                fixes #1065
Signed-off-by: Tommesha Wiggins <tommesha.wiggins@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-24 15:34:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1089" class=".btn">#1089</a>
            </td>
            <td>
                <b>
                    style(supply-chain-frontend): multiple linter fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span>
            </td>
            <td>
                Signed-off-by: Youngone Lee <youngone.lee@accenture.com>

@petermetz ping for review
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 20:08:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1088" class=".btn">#1088</a>
            </td>
            <td>
                <b>
                    style(i-eth-contract-deployment): linter fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Youngone Lee <youngone.lee@accenture.com>

@petermetz ping for review! 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 19:46:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1087" class=".btn">#1087</a>
            </td>
            <td>
                <b>
                    feat(connector-besu): add getTransaction web service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jeffrey Ushry <jeffrey.ushry@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 18:09:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1086" class=".btn">#1086</a>
            </td>
            <td>
                <b>
                    style(data-fetcher): multiple linter fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Youngone Lee <youngone.lee@accenture.com>

@petermetz ping for review, all the warnings looked the same so they are in the same PR! 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 16:59:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1085" class=".btn">#1085</a>
            </td>
            <td>
                <b>
                    feat(connector-besu): add getBalance web service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Besu</span><span class="chip">enhancement</span>
            </td>
            <td>
                Fixes #1066

@petermetz Mr.Tyler helped me with the test cases! 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 15:36:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1084" class=".btn">#1084</a>
            </td>
            <td>
                <b>
                    feat(test-tooling): faio features and improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds several improvements:
1) destroys faio volume when tests end
2) allows to recover a test ledger (setContainer)
3) allows to add organizations

Replaces PR #949 cc @petermetz 

Signed-off-by: Rafael Belchior <rafael.belchior@tecnico.ulisboa.pt>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-23 14:29:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1081" class=".btn">#1081</a>
            </td>
            <td>
                <b>
                    feat(connector-xdai): add interval to pollForTxReceipt
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Xdai</span><span class="chip">bug</span><span class="chip">enhancement</span>
            </td>
            <td>
                #1078 
Signed-off-by: Pritam Singh <pkspritam16@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-22 18:39:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1080" class=".btn">#1080</a>
            </td>
            <td>
                <b>
                    docs(examples): fix supply chain image build errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span>
            </td>
            <td>
                Fixes #1063

cc: @sichen1234 @Zzocker 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-22 06:15:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1079" class=".btn">#1079</a>
            </td>
            <td>
                <b>
                    feat(connector-besu): add getPastLogs web service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                Fixes #1067 
Depends on #1042


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 20:42:23 +0000 UTC
    </div>
</div>

