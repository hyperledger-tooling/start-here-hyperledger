---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/895" class=".btn">#895</a>
            </td>
            <td>
                <b>
                    build: remove npm dep. commitizen to avoid git-cz conflict
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allegedly fixes the strange git-cz error encountered
while running "npm run commit"

(node:11594) UnhandledPromiseRejectionWarning: TypeError: Cannot convert undefined or null to object
    at Function.keys (<anonymous>)
    at runInteractiveQuestions (//node_modules/git-cz/dist/cz.js:576:10)
    at run (//node_modules/git-cz/dist/cz.js:157:11)
    at exports.prompter (//node_modules/git-cz/dist/cz.js:164:3)
    at //node_modules/commitizen/dist/commitizen/commit.js:598:9
    at //node_modules/fs-extra/lib/mkdirs/mkdirs.js:56:16
    at callback (//node_modules/graceful-fs/polyfills.js:295:20)
    at FSReqCallback.oncomplete (fs.js:184:5)

Hit the same issue, multiple times with it disappearing and then resurfacing with different versions as well, made no sense.

So, I started checking other things and found out that I also had commitizen installed which for some reason declares it's own, conflicting binary also called git-cz that (I'm guessing) may end up being hooked up to ./node_modules/.bin/git-cz randomly depending on the cookie crumbles when you run npm install (which I assume does as much as possible parallelized)

Uninstalled commitizen and right now it's working. Just a theory, but maybe it's right.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>


cc: @travis-payne @TonyRowntree 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-02 00:08:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/894" class=".btn">#894</a>
            </td>
            <td>
                <b>
                    chore(linter): fix warning in isIPluginWebService
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 21:24:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/892" class=".btn">#892</a>
            </td>
            <td>
                <b>
                    fix(github/workflows): dependent issues job name typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">dependencies</span>
            </td>
            <td>
                There was a typo in the first fix I attempted so now fixing the fix here
(hopefully)

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 21:13:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/884" class=".btn">#884</a>
            </td>
            <td>
                <b>
                    refactor(consortium-manual): move logic from endpoint to plugin class
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolve #429 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 15:39:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/883" class=".btn">#883</a>
            </td>
            <td>
                <b>
                    refactor(core-api): discontinue web service plugin aspect #350
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: TonyRowntree <33454202+TonyRowntree@users.noreply.github.com>

**Removed**
- WEB_SERVICE PluginAspect


**Added**
- BUSINESS_LOGIC PluginAspect

Resolve #350 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 15:37:20 +0000 UTC
    </div>
</div>

