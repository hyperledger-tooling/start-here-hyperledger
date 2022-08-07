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
- For now, I've followed the example of the aries-cloudagent-container repo and am installing ACA-Py through the published PyPI package. It might make more sense to be able to published directly from the repo contents?

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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1886" class=".btn">#1886</a>
            </td>
            <td>
                <b>
                    Use did:key for recipient keys
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As part of #1859, I have made it so the coordinate-mediation protocol uses did:key representation. Apologies that this took as long as it did. Implementing this impacted more of ACA-Py than I realized it would while keeping it compatible with existing agents.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-04 18:58:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1885" class=".btn">#1885</a>
            </td>
            <td>
                <b>
                    fix: schema class can set Meta.unknown
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR enables the Schema class of a model to determine the default `unknown` behavior. Without this, if you have a schema where you expect extra values to be present, every time `deserialize` or `serialize` is called, you must set `unknown=INCLUDE`. Now, in the `Meta` class of the Schema, `unknown` can be set to some value that will be respected as the default if not overrided by method parameter.

While I was at it, I also touched up some of the typing. I'm not fond of using `@overload` but I think it's the best way to address typing a method where a bool flag impacts the return type.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-04 16:54:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1881" class=".btn">#1881</a>
            </td>
            <td>
                <b>
                    fix: didx request cannot be accepted
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hi everyone,

this PR fixes a few problems which were apparently introduced by #1710:

- A didx request which is received in response to an explicit oob invitation cannot be accepted because the state of the corresponding connection record is not updated to `'request-received'`

- The admin api incorrectly indicates that the `/out-of-band/receive-invitation` endpoint returns a `ConnRecord` instead of the new `OobRecord` (which is also why the `OobRecord` is not included in the `swagger.json`)

@TimoGlastra: maybe you want to take a look to make sure I didn't break the connectionless exchange feature by saving the updated connection record?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-01 16:44:08 +0000 UTC
    </div>
</div>

