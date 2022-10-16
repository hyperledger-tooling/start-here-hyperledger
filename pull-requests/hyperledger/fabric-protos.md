---
layout: default
title: fabric-protos
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-protos
---

# fabric-protos <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-protos){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/141" class=".btn">#141</a>
            </td>
            <td>
                <b>
                    Fixed @ CVE-2022-31163
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: mik-patient <112659896+mik-patient@users.noreply.github.com>

## Vulnerability Description
With the Ruby data source (the tzinfo-data gem for tzinfo version 1.0.0 and later and built-in to earlier versions), time zones are defined in Ruby files. There is one file per time zone. Time zone files are loaded with require on demand. In the affected versions, `TZInfo::Timezone.get` fails to validate time zone identifiers correctly, allowing a new line character within the identifier. With Ruby version 1.9.3 and later, `TZInfo::Timezone.get` can be made to load unintended files with require, executing them within the Ruby process.
```rb
TZInfo::Timezone.get("foo\n/../../../../../../../../../../../../../../../../tmp/payload")
```
**CVE-2022-31163**
`CVSS:3.1/AV:N/AC:H/PR:N/UI:R/S:U/C:H/I:H/A:H`
GHSA-5cm2-9h8c-rvfx


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-16 04:16:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/140" class=".btn">#140</a>
            </td>
            <td>
                <b>
                    Fixed CWE-400 Uncontrolled Resource Consumption
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: mik-patient <112659896+mik-patient@users.noreply.github.com>
## Vulnerability Description
CommonMarker uses cmark-gfm for rendering [Github Flavored Markdown](https://github.github.com/gfm/). A polynomial time complexity issue in cmark-gfm's autolink extension may lead to unbounded resource exhaustion and subsequent denial of service.

https://github.com/gjtorikian/commonmarker/pull/190
[GHSA-cgh3-p57x-9q7q](https://github.com/github/cmark-gfm/security/advisories/GHSA-cgh3-p57x-9q7q)
https://en.wikipedia.org/wiki/Time_complexity
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-16 04:13:11 +0000 UTC
    </div>
</div>

