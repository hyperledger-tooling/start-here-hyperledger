---
layout: default
title: aries-framework-swift
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-swift
---

# aries-framework-swift <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-swift){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-swift/pull/16" class=".btn">#16</a>
            </td>
            <td>
                <b>
                    feature: Support invitation short url
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Checklist

- [x] I have run swiftlint
- [x] I have run AriesFrameworkTests
- [x] I have run AllTests

## Description

Close https://github.com/naver/aries-framework-swift/issues/19

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-23 02:27:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-swift/pull/15" class=".btn">#15</a>
            </td>
            <td>
                <b>
                    doc: Update install guide
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Checklist

- [ ] I have run swiftlint
- [ ] I have run AriesFrameworkTests
- [ ] I have run AllTests

## Description

Fix #14 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-22 02:02:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-swift/pull/13" class=".btn">#13</a>
            </td>
            <td>
                <b>
                    sample: Change QRCode scanner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Checklist

- [ ] I have run swiftlint
- [ ] I have run AriesFrameworkTests
- [ ] I have run AllTests

## Description

The previous scanner did not work on iOS 16.
Changed to https://github.com/twostraws/CodeScanner which supports SwiftUI.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-21 05:50:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-swift/pull/11" class=".btn">#11</a>
            </td>
            <td>
                <b>
                    fix: Fix decoding error when oob attachments contain json data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Checklist

- [x] I have run swiftlint
- [x] I have run AriesFrameworkTests
- [ ] I have run AllTests

## Description

Fix #9
Swift `Decodable` cannot decode untyped json. Requests of oob invitation will be `AgentMessage` types, but we don't know the exact type in advance.
This fix works as follows to handle this:
- Change the json data of attachments  to a `String` by serializing it
- The string data will be treated the same as the decoded base64-encoded string
- Use `JSONSerialization` to change the message instead of `Codable` protocol
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-19 09:02:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-swift/pull/10" class=".btn">#10</a>
            </td>
            <td>
                <b>
                    fix: Allow legacy did:sov prefix in the oob invitation message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Checklist

- [x] I have run swiftlint
- [x] I have run AriesFrameworkTests
- [ ] I have run AllTests

## Description

Fix #6 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-19 03:15:17 +0000 UTC
    </div>
</div>

