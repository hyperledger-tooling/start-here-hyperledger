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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/140" class=".btn">#140</a>
            </td>
            <td>
                <b>
                    feat(js): allow custom native bindings for RN
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allows the user the supply custom native bindings to the reactnativeariesaskar class. This is done to make it easier to add support for Expo in the future.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-17 11:51:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/139" class=".btn">#139</a>
            </td>
            <td>
                <b>
                    chore: lower iOS compatibility
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Use static libraries for iOS for lower version compatibility
- Use rust 1.61.0 in CI as hashbrown needs 1.61.0 minimum.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-17 09:17:45 +0000 UTC
    </div>
</div>

