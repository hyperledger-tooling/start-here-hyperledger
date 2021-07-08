---
layout: default
title: indy-plenum
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-plenum
---

# indy-plenum <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-plenum){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1545" class=".btn">#1545</a>
            </td>
            <td>
                <b>
                    Publishing artifacts ubuntu 20.04
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR contains the CD part of the GHA pipeline for the Ubuntu 20.04 upgrade (Issue #1537).

- Copied the CD part (Merge #1541) from the master branch and adjusted it to run in the 20.04 workflow
- rearranged dependencies in alphabetical order
- extended the `Dockerfile.ubuntu-2004` with `fpm` and `zstd`
- created build-scripts for ubuntu 20.04 based on the build-scripts for Ubuntu 16.04
- Creates artifacts of all 3rd-party dependencies from `install_requires` with pinned versions according to the versions used in `Dockerfile.ubuntu-2004` that are necessary to pass the tests
- removed `build_rocksdb_deb` because rocksdb v.5.17.2 package is available as [ubuntu package](https://packages.ubuntu.com/source/focal/rocksdb)

All tests pass but Sliced Module Tests (plenum, 3). [GHA of the PR ](https://github.com/udosson/indy-plenum/runs/3018170304?check_suite_focus=true). 
A lean-up of the commit history will be done once we're ready to merge.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-08 13:13:28 +0000 UTC
    </div>
</div>

