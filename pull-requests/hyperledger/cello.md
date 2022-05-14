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
                PR <a href="https://github.com/hyperledger/cello/pull/443" class=".btn">#443</a>
            </td>
            <td>
                <b>
                    Fix (security) : Path Traversal Bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Unsanitized input from ```r.headers``` and ```content_type = r.headers["content-type"]
    extension = mimetypes.guess_extension(content_type)
    file_name = "%s%s" % (uuid4().hex, extension)
    target_file = os.path.join(target_dir, secure(file_name))``` resource  flows into ```open(target_file, "wb").write(r.content)```, where it is used as a path. This may result in a Path Traversal vulnerability and allow an attacker to write arbitrary files.
Signed-off-by: Bhaskar <dev@bhaskar.email>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-14 14:46:35 +0000 UTC
    </div>
</div>

