---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1896" class=".btn">#1896</a>
            </td>
            <td>
                <b>
                    [#1895] Stopping the aca-py shell process keeps python process running
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Thomas Diesler <tdiesler@redhat.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-12 09:16:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1894" class=".btn">#1894</a>
            </td>
            <td>
                <b>
                    Fix: SchemasInputDescriptorFilter: broken deserialization renders generated clients unusable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **What’s wrong?**
The OpenAPI spec requires an Input Descriptor’s `schema` property to contain a `SchemasInputDescriptorFilter` object.
However, on deserialization, there is a [preprocessing step](https://github.com/hyperledger/aries-cloudagent-python/blob/d407c48cc9f041c5b27ee8f589fc0e2eaef2220d/aries_cloudagent/protocols/present_proof/dif/pres_exch.py#L235-L254) which ensures that lists of URIs or a dict containing a `oneof_filter` property are accepted as well by transforming them into said object. (These alternative input formats are also [included as examples](https://github.com/hyperledger/aries-cloudagent-python/blob/d407c48cc9f041c5b27ee8f589fc0e2eaef2220d/aries_cloudagent/protocols/present_proof/dif/pres_exch.py#L640-L663) in the `InputDescriptors` model.) Yet, input that already IS a `SchemasInputDescriptorFilter` object is not handled correctly during preprocessing and deserialization fails. This results in any client adhering to the spec being unable to create valid input descriptors and, ultimately, a presentation definition to use in a DIF proof request.

**What has been changed?**
I adjusted the preprocessing step such that input is forwarded as-is if it looks like a `SchemasInputDescriptorFilter`. I also extended the tests to cover deserializing the actual object.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-11 15:58:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1892" class=".btn">#1892</a>
            </td>
            <td>
                <b>
                    Refactor ledger correction code and insert into revocation error handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addresses issue https://github.com/hyperledger/aries-cloudagent-python/issues/1868

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-09 22:04:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1891" class=".btn">#1891</a>
            </td>
            <td>
                <b>
                    did registry cleanup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR removes did registry class and uses a list instead. Simplifying the code.

Signed-off-by: Adam Burdett <burdettadam@gmail.com>
Co-authored-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-09 19:12:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1888" class=".btn">#1888</a>
            </td>
            <td>
                <b>
                    feat: add dockerfiles for building images from repo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Putting this out there to hopefully spark some discussion.

This PR adds Dockerfiles for publishing images for ACA-Py directly from this repo (i.e. no dependencies on bcgovimages). I made some opinionated decisions that I hope will catch some people's attention (so you can tell me why I'm wrong :slightly_smiling_face:):
- Rather than building aries-askar, indy-shared-rs, and indy-vdr directly in the image, I opted to instead let it use the binaries bundled in the python packages. Good chance I'm wrong, but I'm about 70% sure these libraries might have been taking precedence over those included in von-image anyways.
- I am thinking of "indy-less" ACA-Py as the default. `ghcr.io/hyperledger/aries-cloudagent-python:py3.6-0.7.4` image would not have any Indy libraries installed. To get an image with Indy included, I'm thinking the image name+tag might look like: `ghcr.io/hyperledger/aries-cloudagent-python:py3.6-indy-1.16.0-0.7.4`.
- The ACA-Py+Indy image does NOT include Indy CLI (von-image did).
- The default ACA-Py image's user is now `aries` instead of `indy`. The ACA-Py+Indy image's user will still be `indy` (this inconsistency may be undesirable...).
- I introduced an `indy-python` image that can be reused as a base for things needing an image with just python3-indy and built Indy libraries. This is the base image used by the ACA-Py+Indy image. I would like to see this published as `ghcr.io/hyperledger/indy-python`.
- Rather than using pyenv to get a specific python version, I opted to just use the relevant python docker image for the requested version, i.e. `python:3.6.13-slim-buster`. Python packages are installed into the system site packages (rather than the user site packages or a virtual environment).
- For now, I've followed the example of the aries-cloudagent-container repo and am installing ACA-Py through the published PyPI package. It might make more sense to be able to publish directly from the repo contents?

I get the feeling that we can further prune a lot of the installed packages but (for now) I've left in most of those originally installed in von-image.

I've included a simple Makefile purely to demonstrate building the image and I do not anticipate that we'd leave this Makefile around. I'll plan on removing it before this PR moves on to potentially getting merged.

This is relevant to #1854, #1856, and #1871.

cc @WadeBarnes @andrewwhitehead @swcurran @burdettadam 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-06 21:58:54 +0000 UTC
    </div>
</div>

