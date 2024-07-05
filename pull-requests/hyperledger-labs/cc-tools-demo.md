---
layout: default
title: cc-tools-demo
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/cc-tools-demo
---

# cc-tools-demo <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/cc-tools-demo){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/cc-tools-demo/pull/67" class=".btn">#67</a>
            </td>
            <td>
                <b>
                    Correction of the getBlockByHash function - QueryQSCC Handler: hashBytes, err := hex.DecodeString(hash), passed as a parameter to the chaincode.QueryGateway function, assigned to result.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Matheus Lázaro <matheus.lazaro@discente.ufg.br>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-04 23:25:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/cc-tools-demo/pull/66" class=".btn">#66</a>
            </td>
            <td>
                <b>
                    CC-Tools 1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Changes
- Bump CC-Tools version to 1.0
- Bump Go version from both chaincode and API to 1.21
- Update project dependencies
- Refactor godog tests to use the library instead of the binaries
- Generate collection files on startDev
- Use new callers format on transactions
- Automatic fabric binaries download if non-existent on the system
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-02 12:51:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/cc-tools-demo/pull/65" class=".btn">#65</a>
            </td>
            <td>
                <b>
                    Bump to CC-Tools 1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Bump CC-Tools version to 1.0
- Bump CCAPI Go version to 1.21
- Update dependencies
- Remove `ioutil` references, following its deprecation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-01 17:36:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/cc-tools-demo/pull/64" class=".btn">#64</a>
            </td>
            <td>
                <b>
                    Resolved Deprecated Function and Updated .gitignore File
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this update,I have addressed some deprecated function from ioutil that may cause issues in our project. I have replaced the deprecated function with a more up-to-date alternative, which has resolved the problem and improved the overall stability of the project.

Reference:
https://github.com/go-critic/go-critic/issues/1019
https://github.com/golang/go/issues/42026
https://github.com/golang/go/issues/40025
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-28 12:44:48 +0000 UTC
    </div>
</div>

