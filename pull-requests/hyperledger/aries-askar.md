---
layout: default
title: aries-askar
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-askar
---

# aries-askar <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-askar){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/143" class=".btn">#143</a>
            </td>
            <td>
                <b>
                    chore: update version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Discussed with @andrewwhitehead and we will do a quick 0.2.9-dev.1 release to make sure all the iOS fixes are correct and release 2.9.0 when everything is working.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-22 10:13:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/142" class=".btn">#142</a>
            </td>
            <td>
                <b>
                    feat: react native > 0.71.x support and Expo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                small edit: there might be some cleanup to do as we do not use JSC or Hermes directly so we can likely omit some checks there in the `CMakelist.txt`.

tested with:
  - expo 48 + RN 71
  - RN 71
  - RN 69
  - RN 68
  - RN 66 (needs a minor change in the android/app/build.gradle, this is relevant for bifold). 


# for RN 66 support:

in android/app/build.gradle

```diff
-    implementation "com.facebook.react:react-native:+"  // From node_modules
+    implementation "com.facebook.react:react-native:0.66.2"
```

or 

```diff
+ def REACT_NATIVE_VERSION = new File(['node', '--print',"JSON.parse(require('fs').readFileSync(require.resolve('react-native/package.json'), 'utf-8')).version"].execute(null, rootDir).text.trim())

-    implementation "com.facebook.react:react-native:+"  // From node_modules
+    implementation "com.facebook.react:react-native:" + REACT_NATIVE_VERSION
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-19 13:22:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/141" class=".btn">#141</a>
            </td>
            <td>
                <b>
                    chore(js): update version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: blu3beri <blu3beri@proton.me>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-17 13:30:50 +0000 UTC
    </div>
</div>

