---
layout: default
title: private-data-objects
parent: Hyperledger Labs
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger-labs/private-data-objects
---

# private-data-objects <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/private-data-objects){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger-labs/private-data-objects/issues/330" class=".btn">330</a>
            </td>
            <td>
                <b>
                    enclave quote status error: CONFIGURATION_NEEDED
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">help wanted</span><span class="chip">good first issue</span>
            </td>
            <td>
                Hi，I am an undergraduate student who just started to study blockchain privacy. I learned about your project from my friend some time ago.  I'm so grateful for this open source project, a fantastic project.
I reinstalled a ubuntu18.04, a clean environment. I builded PDO followed by host_install.md. Everything is ok! 
And  I `make` it after changed the value of SGX_MODE from SIM to HW. It break down at register-with-ledger.sh, its output as follow:

> registering enclave and IAS public key on the ledger
. /root/private-data-objects/bin/activate && /root/private-data-objects/eservice/bin/register-with-ledger.sh
 register-with-ledger.sh: Download IAS certificates and Compute the enclave information
 register-with-ledger.sh: operation failed: eservice-enclave-info --spid ABAC66755CB4E6424B04F96CC07C21C7 --save /tmp/pdo-test.sPkasxVmc --loglevel warn --identity eservice1 --config eservice1.toml enclave.toml --config-dir /root/private-data-objects/opt/pdo/etc/
 register-with-ledger.sh: Clean up temporary files
Makefile:227: recipe for target 'register' failed
make: *** [register] Error 111

`
` 
I tried the following:
When I execute this command alone `eservice-enclave-info --spid ABAC66755CB4E6424B04F96CC07C21C7 ...,` there are no errors.
But I execute this shell file alone `register-with-ledger.sh`, it fail as above.How can I solve it?
I have done as follows：
It can be successfully built and tested in Docker. But I need non-docker build. So I followed by host_install.md now. And I have deployed the sawtooth ledger service on a new ubuntu16.04. The variables are configured correctly，such as PDO_LEDGER_URL.
My plan is as follows：
If PDO in HW mode can be builded successfully, I'll replace Gipsy with Wawaka.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-30 17:13:00 +0000 UTC
    </div>
</div>

