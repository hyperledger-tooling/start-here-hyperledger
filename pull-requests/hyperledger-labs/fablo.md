---
layout: default
title: fablo
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fablo
---

# fablo <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fablo){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fablo/pull/448" class=".btn">#448</a>
            </td>
            <td>
                <b>
                    depricate test-03-private-data test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #396 
I have removed the test-03-private-data from the CI and have also renamed couple of files in CI as well as in script.
- [x] Remove test-03-private-data check - both from CI and the whole test script
- [x] Move private data checks to test-02-private-data
- [x] Rename remaining checks, to keep naming consistent (i.e. either rename 04 to 03, or remove numbers entirely from names)
- [ ] Update TEST_CASES.md to reflect the updated test cases

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 15:53:27 +0000 UTC
    </div>
</div>

