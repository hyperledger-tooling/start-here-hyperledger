---
layout: default
title: fabric-chaincode-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-java
---

# fabric-chaincode-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-chaincode-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/244" class=".btn">#244</a>
            </td>
            <td>
                <b>
                    Add test for Logger.debug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hey 😊
I want to contribute the following test:

Test that calling `Logger.getLogger(LoggerTest.class).debug("debug message")` does not throw an exception.
This tests the method [`Logger.debug`](https://github.com/hyperledger/fabric-chaincode-java/blob/d1d093b42324230f55410fda3c9efb1663859380/fabric-chaincode-shim/src/main/java/org/hyperledger/fabric/Logger.java#L45).
This test is based on the test [`logger`](https://github.com/hyperledger/fabric-chaincode-java/blob/d1d093b42324230f55410fda3c9efb1663859380/fabric-chaincode-shim/src/test/java/org/hyperledger/fabric/LoggerTest.java#L19).

Curious to hear what you think!

(I wrote this test as part of a research study at TU Delft. [Find out more](https://github.com/lacinoire/lacinoire/blob/main/README.md))
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-09 08:47:32 +0000 UTC
    </div>
</div>

