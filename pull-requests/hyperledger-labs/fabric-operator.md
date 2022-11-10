---
layout: default
title: fabric-operator
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operator
---

# fabric-operator <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operator){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/80" class=".btn">#80</a>
            </td>
            <td>
                <b>
                    chore: remove todo in unit-tests workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                uncomment push and gosec
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-10 06:32:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/79" class=".btn">#79</a>
            </td>
            <td>
                <b>
                    chore: remove same code in orderer integration test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                the line87-89 and line 91-93 is same, but twice:

https://github.com/hyperledger-labs/fabric-operator/blob/db38e856fda7798650de925addadbc75305adc39/integration/orderer/orderer_suite_test.go#L85-L97

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-10 06:09:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/78" class=".btn">#78</a>
            </td>
            <td>
                <b>
                    chore: push image workflow should limit repository
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The idea of automatically building the image and pushing it to the `ghcr.io` repository after the pull request merge is great. 

Just one small restriction: only run the push job on the main repository: `hyperledger-labs/fabric-operator`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-10 03:02:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/76" class=".btn">#76</a>
            </td>
            <td>
                <b>
                    chore: typo ngress -> ingress
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Abirdcfly <fp544037857@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-09 07:40:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/74" class=".btn">#74</a>
            </td>
            <td>
                <b>
                    feat: add golangci-lint check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pr introduces [golangci-lint](https://github.com/golangci/golangci-lint) to detect problems with go source code. 

And turns on 4 linters: gofmt goimports govet gosimple 
(The first 3 linters are maintained by golang.org, gosimple is a linter enabled by golangci-lint default)


|linters|describe|link|
|---|---|---|
|gofmt|Gofmt checks whether code was gofmt-ed. By default this tool runs with -s option to check for code simplification|https://golang.org/cmd/gofmt/|
|goimports|In addition to fixing imports, goimports also formats your code in the same style as gofmt.|https://godoc.org/golang.org/x/tools/cmd/goimports|
|govet|Vet examines Go source code and reports suspicious constructs, such as Printf calls whose arguments do not align with the format string|https://golang.org/cmd/vet/|
|gosimple|Linter for Go source code that specializes in simplifying code|https://github.com/dominikh/go-tools/tree/master/simple|

See a list of supported linters and which linters are enabled/disabled in https://golangci-lint.run/usage/linters/.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-08 09:27:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/72" class=".btn">#72</a>
            </td>
            <td>
                <b>
                    Add an OPERATOR_LOCAL_MODE environment variable to launch locally.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR allows the operator to be launched locally without running within a Docker container / kubernetes cluster.

Fixes Issue #67

Note that this changes the default path at which the operator config files are read, from `../../` to `./`.   This was actually a bug / error in the original logic, as the working directory for `ibp-operator` in the container is actually `/`.  (When running from the root folder, the `../../` path prefix resolves to `/` on the file system.)

Thank you @bjwswang for the great recommendations on pushing this forward.

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-05 02:43:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/70" class=".btn">#70</a>
            </td>
            <td>
                <b>
                    Fix the build: Run integration tests with golang 1.18, ginkgo v2.1.4, and gomega v1.19 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The recent ginkgo update requires golang 1.18.  This PR fixes the build pipeline, which was pinning the test version to 1.17. 

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-04 13:05:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/69" class=".btn">#69</a>
            </td>
            <td>
                <b>
                    Launch the sample network on Apple Silicon;  Pin k8s to 1.24
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR allows the sample network to run correctly (albeit, slowly) on the new Mac Silicon / arm64 chipset.

The docker images run as `linux/amd64` under QEMU, so performance is very slow.  We should improve the build pipeline to support the `buildx` builder and generate multi-arch containers. 

This PR addresses Issue #63 by pinning the KIND target revision to 1.24.4 (`KIND_CLUSTER_IMAGE`). 

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-04 11:31:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operator/pull/68" class=".btn">#68</a>
            </td>
            <td>
                <b>
                    cleanup: remove BoolTrue and BoolFalse variable
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
        Created At 2022-11-04 08:04:00 +0000 UTC
    </div>
</div>

