---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/881" class=".btn">#881</a>
            </td>
            <td>
                <b>
                    Move SubmitNetworkAction and RootOrg config to Multiparty Manager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also added new transaction and operation types for network action.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-24 20:17:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/880" class=".btn">#880</a>
            </td>
            <td>
                <b>
                    Collapse batchpin.Submitter into multiparty.Manager
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
        Created At 2022-06-24 15:42:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/879" class=".btn">#879</a>
            </td>
            <td>
                <b>
                    surface URI as parameter for token mint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-candidate</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-24 15:03:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/878" class=".btn">#878</a>
            </td>
            <td>
                <b>
                    Enable "gateway-mode" namespaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Needs cleanup, but should be (mostly) fully functional.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-23 18:34:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/877" class=".btn">#877</a>
            </td>
            <td>
                <b>
                    Remove "namespace" as a query param from all routes
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
        Created At 2022-06-22 21:42:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/876" class=".btn">#876</a>
            </td>
            <td>
                <b>
                    Handle namespace validation at the route level rather than at data manager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Data manager is already part of a namespace, so determination of whether the namespace is valid needs to happen earlier in the router, when we're attempting to lookup the proper orchestrator to handle the request.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 21:14:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/875" class=".btn">#875</a>
            </td>
            <td>
                <b>
                    Remove namespace param from remaining manager calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of [FIR-12](https://github.com/hyperledger/firefly-fir/pull/12)
Follow-on to #864

This removes "namespace" as a param to remaining manager methods (since each manager is already assigned to a single namespace) and adds "namespace" as a param to most database queries (since all queries should be scoped to a single namespace).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 20:09:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/874" class=".btn">#874</a>
            </td>
            <td>
                <b>
                    Convert more callback handlers to be namespace-specific
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part of [FIR-12](https://github.com/hyperledger/firefly-fir/pull/12).
Follow-up to #863.

Only the blockchain plugin remains, and will need to be addressed after #865.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 14:40:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/873" class=".btn">#873</a>
            </td>
            <td>
                <b>
                    Use docker buildx for multiarch builds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR switches to the `docker buildx` command for building images for multiple CPU architectures. Currently, the build jobs are set up to build `linux/amd64` and `linux/arm64`. This is set in the `Makefile`. Because building a Docker image for a non-native CPU architecture is very slow (because it's emulated), mutiarch builds are not the default when running `make docker`. Instead a new command, `make docker-multiarch` has been added, which is used by our GitHub Actions.

> **NOTE:** From my testing `docker buildx` seems to return status 0, despite the fact that it may have failed to push to a repository. This can result in false positives for our GitHub Actions. I looked into this and it seems to be an open issue with `buildx` https://github.com/docker/buildx/issues/732
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 14:12:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/872" class=".btn">#872</a>
            </td>
            <td>
                <b>
                    Resolve DX operations via requestID (not event ID)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #871 

Also enhance all E2E test suites to check for stuck operations, as this seems to be a recurring theme that slips through the cracks.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-21 14:33:22 +0000 UTC
    </div>
</div>

