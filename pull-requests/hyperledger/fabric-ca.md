---
layout: default
title: fabric-ca
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-ca
---

# fabric-ca <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-ca){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/396" class=".btn">#396</a>
            </td>
            <td>
                <b>
                    Upgrade to Jinja2 v3.1.3 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The version of Sphinx we were using is simply not compatible with Jinja2 > v3.0.3, so given that we had to upset the delicate balance of requirements anyway, the goal of this PR is now to bring all docs infrastructure for CI/CD as well as dependencies and indeed the docs themselves to the latest version.

#### Type of change

- Documentation update

#### Description

Motivation is https://nvd.nist.gov/vuln/detail/CVE-2024-22195, quite simply. But the version of Sphinx that we were using was many years old and does not support a version of Jinja higher than v3.0.3.  So we need to update the entire set of dependencies for the documentation.

#### Additional details

I will make whatever changes are needed to the docs and/or to the CI/CD pipeline to make this compatible with Sphinx v7.2.6, which is the latest.  Please let me know if something isn't right or needs fixing, because this is the time to do it.

#### Related issues

* https://github.com/hyperledger/fabric-ca/issues/395

#### Release Note

This change does **NOT** impact users of Fabric CA, nor shall it impact the functionality of **any** CA release, past, future, present.   We are also unlikely to merge it until the docs look correct on RTD.  But be advised that they may indeed change.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-16 21:29:11 +0000 UTC
    </div>
</div>

