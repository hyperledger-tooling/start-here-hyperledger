---
layout: default
title: sawtooth-core
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-core
---

# sawtooth-core <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-core){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-core/pull/2431" class=".btn">#2431</a>
            </td>
            <td>
                <b>
                    Fix dependencies to build on ARM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates many dependencies to enable sawtooth validator to build and
run on ARM. Fixes a memory leak that occurs when using the currently
published image on ARM.

Some packages that were pulled in via apt install (ex.
python3-pyformance, python3-grpcio, etc.) aren't published for ARM, so
we need to install them via pip. To install them via pip, we need to
lock versions for some of the packages to continue to use python3.6 and
be compatible with Grid. Some packages need to be up-to-date and not
version-locked. Installing packages via pip is done in steps, as some
packages need to be finished installing before calling `pip install ...`
for others.

This also removes the dependency declarations in `setup.py` and
`stdeb.cfg` files, as these mostly refer to packages without
compatible ARM versions published. They are also silent failures in the
build process.

I suspect that using an updated version of lmdb resolved the memory
leak.

Signed-off-by: Chris Eckhardt <eckhardt@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 21:52:46 +0000 UTC
    </div>
</div>

