---
layout: default
title: cello
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cello
---

# cello <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cello){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/627" class=".btn">#627</a>
            </td>
            <td>
                <b>
                    update glob(npm) for dashboard
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Problem:
When I run the project, the following errors occur.

31.71 warning netlify-lambda > globby > glob@7.2.3: Glob versions prior to v9 are no longer supported
40.63 warning netlify-lambda > webpack > terser-webpack-plugin > cacache > glob@7.2.3: Glob versions prior to v9 are no longer supported
......
204.5 error glob@11.0.0: The engine "node" is incompatible with this module. Expected version "20 || >=22". Got "14.18.3"
204.5 info Visit https://yarnpkg.com/en/docs/cli/install for documentation about this ⌘.
204.5 error Found incompatible module

## Reason:
The original version of glob@7.2.3 is no longer supported. Manual update to version 9.0.0 required.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-13 00:48:53 +0000 UTC
    </div>
</div>

