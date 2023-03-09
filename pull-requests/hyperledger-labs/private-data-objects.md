---
layout: default
title: private-data-objects
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/private-data-objects
---

# private-data-objects <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/private-data-objects){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/413" class=".btn">#413</a>
            </td>
            <td>
                <b>
                    Make CCF HW mode work even with a proxy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The title is self-explanatory and the PR depends on #406.

Explanation.
(short)
CCF can be configured with a domain name, and the PDO legacy proxy handling works.

(long)
CCF is currently configured to use IPs. The main implication is that CCF generates certificates where x509 Subject Alternative Name is an IP address.
```
X509v3 Subject Alternative Name:
                IP Address:192.168.192.2
```
Because of that, CCF clients have to use the IP address to contact it, otherwise the connection fails with an SSL error.

The PDO legacy proxy handling does not work in this case. The `no_proxy` variables are set up only with the `pdo-tp-ccf` domain name -- since clients are supposed to use the `pdo-tp-ccf:6600` ledger url. However, using the URL as-is would not work, as explained above, because the hostname does not match the certificate subject. For this reason, clients first resolve the hostname into the IP address, and then contact CCF.

Fortunately, CCF can be configured with a domain name, as indicated in the [documentation](https://github.com/microsoft/CCF/blob/ccf-1.0.19/doc/operations/start_network.rst).
This just involves adding an argument (the domain name) in the execution of the `cchost` script.
As a result, the domain name is added to the Subject Alternative Name of the node certificate.
```
X509v3 Subject Alternative Name:
                DNS:pdo-tp-ccf, IP Address:192.168.192.2
```
Due this change, clients do not need to resolve the domain name in an IP address and the PDO legacy proxy handling is already configured to make the connections work as intended.

(a separate timing issue)
A final note regarding a timing issue in the registration step, which is solved by waiting a few seconds.
The PDO docker build (the makefile), at some point starts CCF and immediately triggers the registration.
This has two problems -- which surprisingly were not triggered during the HW mode test without a proxy:
1) if CCF is not up, the registration fails because CCF is unreachable.
2) if CCF is up but not configured, the registration fails because the client is not a known member.
Adding a long-enough sleep before the registration seems to provide a satisfactory mitigation to the issue.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 08:02:34 +0000 UTC
    </div>
</div>

