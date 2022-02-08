---
layout: default
title: firefly-cli
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-cli
---

# firefly-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/143" class=".btn">#143</a>
            </td>
            <td>
                <b>
                    Fixes for running on arm64
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR contains a couple of fixes to be able to run FireFly on 64 bit ARM based processors, like M1 Macs.

IPFS has been downgraded to 0.10.0 until https://github.com/ipfs/go-ipfs/issues/8645 is fixed

Go Ethereum has been upgraded to 1.10 as it provides native arm64 builds

Resolves https://github.com/hyperledger/firefly-cli/issues/136
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-07 22:02:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/142" class=".btn">#142</a>
            </td>
            <td>
                <b>
                    Add --platform linux/amd64 to suppress Docker warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                arm64 machines such as Apple's m1 series can run linux/amd64 images via Docker Desktop's emulation, but will produce the following warning that causes some command JSON output parsing to fail:

WARNING: The requested image's platform (linux/amd64) does not match the detected host platform (linux/arm64/v8) and no specific platform was requested
Because Fabric so far only publishes linux/amd64 images, and they seem to work fine running under the emulation on m1 machines, we can simply force the platform to be linux/amd4 during docker run in order to suppress the warning
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-04 18:00:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/140" class=".btn">#140</a>
            </td>
            <td>
                <b>
                    [default-connector] default token provider is erc1155
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The out of the box token connector is only ERC1155
Signed-off-by: David Echelberger <david.echelberger@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-04 16:58:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/138" class=".btn">#138</a>
            </td>
            <td>
                <b>
                    [add-back-prom] adding back prometheus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The `--prometheus-enabled` flag was inadvertently removed from `cmd/init.go` in a previous merge. This is to add it back

Signed-off-by: David Echelberger <david.echelberger@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 20:05:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/137" class=".btn">#137</a>
            </td>
            <td>
                <b>
                    Support multiple token connectors in a stack, with ERC20/ERC721
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Broadhurst <peter.broadhurst@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-01 16:10:13 +0000 UTC
    </div>
</div>

