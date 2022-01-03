---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/590" class=".btn">#590</a>
            </td>
            <td>
                <b>
                    docs(apple-silicon): update OpenSSL instructions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When following the instructions for installing indy for an Apple Silicon (M1 Pro) system, I found that the `brew install` command didn't work. After looking into how to install OpenSSL for M1, I found that the OpenSSL v1.1 on Homebrew also works for Apple Silicon chips (see: https://formulae.brew.sh/formula/openssl@1.1).

After following the rest of the instructions I ran the `is-indy-installed` test script, which resulted in `Libindy was installed correctly`. As a double check I have also installed `@aries-framework/node`, again with success.

> NOTE: When I ran `brew install openssl@1.1` it told me v1.1 was already on my system. I am unsure if this is because stuff I have installed prior to this attempt, or if this is because it's natively shipped with macOs. Therefore I have included the install command in the instructions, just to be sure. 


﻿Signed-off-by: Karim Stekelenburg <karim@animo.id>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 17:46:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/589" class=".btn">#589</a>
            </td>
            <td>
                <b>
                    feat(core): allow to set auto accept connetion exchange when accepting invitation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Related to #583 

I'm already using these changes in OOB implementation #531 but I wanted to create separate PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 16:04:31 +0000 UTC
    </div>
</div>

