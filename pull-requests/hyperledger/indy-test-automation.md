---
layout: default
title: indy-test-automation
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-test-automation
---

# indy-test-automation <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-test-automation){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-test-automation/pull/119" class=".btn">#119</a>
            </td>
            <td>
                <b>
                    CVE-2007-4559 Patch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Patching CVE-2007-4559

Hi, we are security researchers from the Advanced Research Center at [Trellix](https://www.trellix.com). We have began a campaign to patch a widespread bug named CVE-2007-4559. CVE-2007-4559 is a 15 year old bug in the Python tarfile package. By using extract() or extractall() on a tarfile object without sanitizing input, a maliciously crafted .tar file could perform a directory path traversal attack. We found at least one unsantized extractall() in your codebase and are providing a patch for you via pull request. The patch essentially checks to see if all tarfile members will be extracted safely and throws an exception otherwise. We encourage you to use this patch or your own solution to secure against CVE-2007-4559. Further technical information about the vulnerability can be found in this [blog](https://www.trellix.com/en-us/about/newsroom/stories/research/tarfile-exploiting-the-world.html).

If you have further questions you may contact us through this projects lead researcher [Kasimir Schulz](mailto:kasimir.schulz@trellix.com).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-08 19:56:16 +0000 UTC
    </div>
</div>

