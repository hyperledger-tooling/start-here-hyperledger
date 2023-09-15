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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1575" class=".btn">#1575</a>
            </td>
            <td>
                <b>
                    fix: service validation in OOB invitation objects
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I'm not an expert (neither a fan 😝) of `class-validator` but I recently found an issue when creating an `OutOfBandInvitation` instance whose `service` field contains a plain string. It works and allows to do a `toUrl()` and so on, but when it passes through the MessageValidator it threw an error saying:

```
OutOfBandInvitation: Failed to validate class.
    An instance of OutOfBandInvitation has failed the validation:
     - property services[0] has failed the following constraints: each value in nested property services must be either object or array·
```

I found that services field has both `@IsStringOrInstance` and `@ValidateNested` decorators. The first one seems to be doing the correct check on every element of the array, while the latter (which is the one  throwing the error) seems to me redundant in this case. If I remove it, class validation passes (as expected). 

So here I'm removing `@ValidateNested` decorator. Not sure if it's the best approach, but of course happy to change it if there is a more appropriate way.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-15 14:48:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1574" class=".btn">#1574</a>
            </td>
            <td>
                <b>
                    fix(cheqd): Changed the name formatting to a encoded hex value
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For more information about these changes, see: https://cheqd-community.slack.com/archives/C02AQ9UK4HY/p1693916571308369
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-15 10:30:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1573" class=".btn">#1573</a>
            </td>
            <td>
                <b>
                    fix: improve logging
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
        Created At 2023-09-13 10:12:51 +0000 UTC
    </div>
</div>

