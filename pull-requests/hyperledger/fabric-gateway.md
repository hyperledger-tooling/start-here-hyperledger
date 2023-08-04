---
layout: default
title: fabric-gateway
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-gateway
---

# fabric-gateway <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-gateway){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/617" class=".btn">#617</a>
            </td>
            <td>
                <b>
                    Use Java 17 for publishing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Java 8 was used for safety, since the intention is to maintain compatibility with Java 8 by compiling compatible bytecode and only using Java 8 standard libraries. This caused a Javadoc failure when linking to Javadoc built with later versions of Java, since they produce a different format of package-list / element-list file. This problem surfaced when gRPC-Java started to publish builds using Java 11 instead of Java 8, and caused Javadoc warnings linking to their published Javadoc.

Use Java 17 for publishing, relying on the maven.compiler.release (javac --release) option to ensure that compiled output links to the Java 8 standard libraries. To allow this, no longer enforce exactly Java 8 in the Maven release profile.

Fix some broken links in Javadoc.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-04 11:28:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/616" class=".btn">#616</a>
            </td>
            <td>
                <b>
                    Update versions following v1.3.1 release
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
        Created At 2023-08-02 18:07:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-gateway/pull/611" class=".btn">#611</a>
            </td>
            <td>
                <b>
                    Update Java dependencies to address CVE-2023-2976
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 Also update dependencies for Go and Node implementation to stay current.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-30 16:23:49 +0000 UTC
    </div>
</div>

