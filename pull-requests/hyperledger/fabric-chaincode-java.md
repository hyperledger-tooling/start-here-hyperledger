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
                PR <a href="https://github.com/hyperledger/fabric-chaincode-java/pull/255" class=".btn">#255</a>
            </td>
            <td>
                <b>
                    Patched 🐛 Deserialization of Untrusted Data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **CVE-2017-5929**
`9.8/ 10`
CVSS:3.0/AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:H/A:H

## Sumarry of issue vulnerabilities:
QOS.ch Logback before 1.2.0 has a serialization vulnerability affecting the SocketServer and ServerSocketReceiver components. The RemoteStreamAppenderClient class in logback-classic and the SocketNode classes in logback-classic and logback-access allow data to be deserialized over a Java Socket, via an ObjectInputStream, without validating the data beforehand. When data is received from the Socket, to be logged, it is deserialized into Java objects.An attacker can exploit this vulnerability by sending malicious, serialized Java objects over the connection to the Socket, which may result in execution of arbitrary code when those objects are deserialized. Note that although logback-core is implicated by the Logback project here, the Sonatype Security Research team discovered that the vulnerability is actually present in the logback-classic and logback-access components. Versions prior to 1.2.0 are vulnerable, as stated in the advisory.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 03:56:13 +0000 UTC
    </div>
</div>

