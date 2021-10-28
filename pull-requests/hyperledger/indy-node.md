---
layout: default
title: indy-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-node
---

# indy-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node/pull/1705" class=".btn">#1705</a>
            </td>
            <td>
                <b>
                    Baseimage 0.0.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Baseimage changes as discussed in #1684 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-28 08:41:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node/pull/1704" class=".btn">#1704</a>
            </td>
            <td>
                <b>
                    LF Endings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As discussed in #1684
Signed-off-by: pSchlarb <p.schlarb@esatus.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-28 08:31:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node/pull/1703" class=".btn">#1703</a>
            </td>
            <td>
                <b>
                    changed pypi package of plenum to the newest one published by GHA 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the version of the PyPI package of `indy-plenum`  from `1.13.0.dev1034` (build and published by Jenkins instance of Sovrin) to version `1.13.0.dev143`. This version was published in the latest successful GHA run from the `master` branch. The GHA run is at: https://github.com/hyperledger/indy-plenum/runs/3579890752?check_suite_focus=true

This change is the precondition to start migrating from https://repo.sovrin.org/deb/pool/xenial/ to https://hyperledger.jfrog.io/ui/native/indy/pool/xenial.
Also, this update is required to run the node system tests from https://github.com/hyperledger/indy-test-automation/ with the Debian files built and published in the new CI/CD pipeline.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 15:35:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node/pull/1702" class=".btn">#1702</a>
            </td>
            <td>
                <b>
                    Ubuntu16:04: Indy-Test-Automation workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR provides a GHA workflow to run the node system tests from https://github.com/hyperledger/indy-test-automation
The workflow covers all tests from the following pipelines
- The CD Pipeline runs these set of tests; https://github.com/hyperledger/indy-node/blob/master/Jenkinsfile.cd#L87-L100
- The nightly build runs these set of tests; https://github.com/hyperledger/indy-node/blob/master/Jenkinsfile.nightly#L41-L72

- [ ] Test with Debian packages from Artifactory 
- [ ] Decide about the trigger of the pipeline
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 14:11:11 +0000 UTC
    </div>
</div>

