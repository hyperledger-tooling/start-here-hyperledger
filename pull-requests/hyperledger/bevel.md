---
layout: default
title: bevel
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/bevel
---

# bevel <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/bevel){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1987" class=".btn">#1987</a>
            </td>
            <td>
                <b>
                    [indy]: update platform indy helm value templates for flux v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: manikanta-darsi <manikanta.darsi@accenture.com>

**Changelog**
- Update platform indy helm value templates for flux v2

 

**Reviewed by**
@sownak @suvajit-sarkar @jagpreetsinghsasan 

 

**Linked issue**
#1984 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-21 11:16:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1986" class=".btn">#1986</a>
            </td>
            <td>
                <b>
                    Bump kotlin-stdlib from 1.1.60 to 1.6.0 in /platforms/r3-corda/images/doorman
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps [kotlin-stdlib](https://github.com/JetBrains/kotlin) from 1.1.60 to 1.6.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/JetBrains/kotlin/releases">kotlin-stdlib's releases</a>.</em></p>
<blockquote>
<h2>Kotlin 1.6.0</h2>
<h2>Changelog</h2>
<h3>Android</h3>
<ul>
<li><a href="https://youtrack.jetbrains.com/issue/KT-48019"><code>KT-48019</code></a> Bundle Kotlin Tooling Metadata into apk artifacts</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-47733"><code>KT-47733</code></a> JVM / IR: Android Synthetic don't generate _findCachedViewById function</li>
</ul>
<h3>Compiler</h3>
<h4>New Features</h4>
<ul>
<li><a href="https://youtrack.jetbrains.com/issue/KT-47984"><code>KT-47984</code></a> In-place arguments inlining for <a href="https://github.com/InlineOnly"><code>@​InlineOnly</code></a> functions</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-12794"><code>KT-12794</code></a> Allow runtime retention repeatable annotations when compiling under Java 8</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-43714"><code>KT-43714</code></a> Support annotations on class type parameters (AnnotationTarget.TYPE_PARAMETER)</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-45949"><code>KT-45949</code></a> Kotlin/Native: Improve bound check elimination</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-43919"><code>KT-43919</code></a> Support loading Java annotations on base classes and implementing interfaces'  type arguments</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-48194"><code>KT-48194</code></a> Try to resolve calls where we don't have enough type information, using the builder inference despite the presence of the annotation</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-47736"><code>KT-47736</code></a> Support conversion from regular functional types to suspending ones in JVM IR</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-39055"><code>KT-39055</code></a> Support property delegate created via synthetic method instead of field</li>
</ul>
<h4>Performance Improvements</h4>
<ul>
<li><a href="https://youtrack.jetbrains.com/issue/KT-45185"><code>KT-45185</code></a> FIR2IR: get rid of IrBuiltIns usages</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-47918"><code>KT-47918</code></a> JVM / IR: Performance degradation with const-bound for-cycles</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-33835"><code>KT-33835</code></a> Bytecode including unnecessary null checks for safe calls where left-hand side is non-nullable</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-41510"><code>KT-41510</code></a> Compilation of kotlin html DSL is still too slow</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-48211"><code>KT-48211</code></a> We spend a lot of time in ExpectActual declaration checker when there is very small amount of actual/expect declaration</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-39054"><code>KT-39054</code></a> Optimize delegated properties which call get/set on the given KProperty instance on JVM</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-46615"><code>KT-46615</code></a> Don't generate nullability assertions in methods for directly invoked lambdas</li>
</ul>
<h4>Fixes</h4>
<ul>
<li><a href="https://youtrack.jetbrains.com/issue/KT-49613"><code>KT-49613</code></a> JVM / IR: &quot;Exception during IR lowering&quot; with java fun interface and it's non-trivial usage</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-49548"><code>KT-49548</code></a> &quot;ClassCastException: java.util.ArrayList$Itr cannot be cast to kotlin.collections.IntIterator&quot; with Iterable inside <code>let</code></li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-22562"><code>KT-22562</code></a> Deprecate calls to &quot;suspend&quot; named functions with single dangling lambda argument</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-47120"><code>KT-47120</code></a> JVM IR: NoClassDefFoundError when there are an extension and a regular function with the same name</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-49477"><code>KT-49477</code></a> Has ran into recursion problem with two interdependant delegates</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-49442"><code>KT-49442</code></a> ClassCastException on reporting [EXPOSED_FROM_PRIVATE_IN_FILE] Deprecation: private-in-file class should not expose 'private-in-class'</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-49371"><code>KT-49371</code></a> JVM / IR: &quot;NoSuchMethodError&quot; with multiple inheritance</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-44843"><code>KT-44843</code></a> PSI2IR: &quot;org.jetbrains.kotlin.psi2ir.generators.ErrorExpressionException: null: KtCallExpression&quot; with delegate who has name or parameter with the same name as a property</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-49294"><code>KT-49294</code></a> Turning FlowCollector into 'fun interface' leads to AbstractMethodError</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-18282"><code>KT-18282</code></a> Companion object referencing it's own method during construction compiles successfully but fails at runtime with VerifyError</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-25289"><code>KT-25289</code></a> Prohibit access to class members in the super constructor call of its companion and nested object</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-32753"><code>KT-32753</code></a> Prohibit <a href="https://github.com/JvmField"><code>@​JvmField</code></a> on property in primary constructor that overrides interface property</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-43433"><code>KT-43433</code></a> <code>Suspend conversion is disabled</code> message in cases where it is not supported and quickfix to update language version is suggested</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-49399"><code>KT-49399</code></a> Building repeatable annotation with Container nested class fails with ISE: &quot;Repeatable annotation class should have a container generated&quot;</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-49209"><code>KT-49209</code></a> Default upper bound for type variables should be non-null</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-49335"><code>KT-49335</code></a> NPE in <code>RepeatedAnnotationLowering.wrapAnnotationEntriesInContainer</code> when using <code>@Repeatable</code> annotation from different file</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-48876"><code>KT-48876</code></a> java.lang.UnsupportedOperationException: org.jetbrains.kotlin.ir.expressions.impl.IrReturnableBlockImpl@4a729df2</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/JetBrains/kotlin/blob/v1.6.0/ChangeLog.md">kotlin-stdlib's changelog</a>.</em></p>
<blockquote>
<h2>1.6.0</h2>
<h3>Android</h3>
<ul>
<li><a href="https://youtrack.jetbrains.com/issue/KT-48019"><code>KT-48019</code></a> Bundle Kotlin Tooling Metadata into apk artifacts</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-47733"><code>KT-47733</code></a> JVM / IR: Android Synthetic don't generate _findCachedViewById function</li>
</ul>
<h3>Compiler</h3>
<h4>New Features</h4>
<ul>
<li><a href="https://youtrack.jetbrains.com/issue/KT-47984"><code>KT-47984</code></a> In-place arguments inlining for <a href="https://github.com/InlineOnly"><code>@​InlineOnly</code></a> functions</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-12794"><code>KT-12794</code></a> Allow runtime retention repeatable annotations when compiling under Java 8</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-43714"><code>KT-43714</code></a> Support annotations on class type parameters (AnnotationTarget.TYPE_PARAMETER)</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-45949"><code>KT-45949</code></a> Kotlin/Native: Improve bound check elimination</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-43919"><code>KT-43919</code></a> Support loading Java annotations on base classes and implementing interfaces'  type arguments</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-48194"><code>KT-48194</code></a> Try to resolve calls where we don't have enough type information, using the builder inference despite the presence of the annotation</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-47736"><code>KT-47736</code></a> Support conversion from regular functional types to suspending ones in JVM IR</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-39055"><code>KT-39055</code></a> Support property delegate created via synthetic method instead of field</li>
</ul>
<h4>Performance Improvements</h4>
<ul>
<li><a href="https://youtrack.jetbrains.com/issue/KT-45185"><code>KT-45185</code></a> FIR2IR: get rid of IrBuiltIns usages</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-47918"><code>KT-47918</code></a> JVM / IR: Performance degradation with const-bound for-cycles</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-33835"><code>KT-33835</code></a> Bytecode including unnecessary null checks for safe calls where left-hand side is non-nullable</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-41510"><code>KT-41510</code></a> Compilation of kotlin html DSL is still too slow</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-48211"><code>KT-48211</code></a> We spend a lot of time in ExpectActual declaration checker when there is very small amount of actual/expect declaration</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-39054"><code>KT-39054</code></a> Optimize delegated properties which call get/set on the given KProperty instance on JVM</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-46615"><code>KT-46615</code></a> Don't generate nullability assertions in methods for directly invoked lambdas</li>
</ul>
<h4>Fixes</h4>
<ul>
<li><a href="https://youtrack.jetbrains.com/issue/KT-49613"><code>KT-49613</code></a> JVM / IR: &quot;Exception during IR lowering&quot; with java fun interface and it's non-trivial usage</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-49548"><code>KT-49548</code></a> &quot;ClassCastException: java.util.ArrayList$Itr cannot be cast to kotlin.collections.IntIterator&quot; with Iterable inside <code>let</code></li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-22562"><code>KT-22562</code></a> Deprecate calls to &quot;suspend&quot; named functions with single dangling lambda argument</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-47120"><code>KT-47120</code></a> JVM IR: NoClassDefFoundError when there are an extension and a regular function with the same name</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-49477"><code>KT-49477</code></a> Has ran into recursion problem with two interdependant delegates</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-49442"><code>KT-49442</code></a> ClassCastException on reporting [EXPOSED_FROM_PRIVATE_IN_FILE] Deprecation: private-in-file class should not expose 'private-in-class'</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-49371"><code>KT-49371</code></a> JVM / IR: &quot;NoSuchMethodError&quot; with multiple inheritance</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-44843"><code>KT-44843</code></a> PSI2IR: &quot;org.jetbrains.kotlin.psi2ir.generators.ErrorExpressionException: null: KtCallExpression&quot; with delegate who has name or parameter with the same name as a property</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-49294"><code>KT-49294</code></a> Turning FlowCollector into 'fun interface' leads to AbstractMethodError</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-18282"><code>KT-18282</code></a> Companion object referencing it's own method during construction compiles successfully but fails at runtime with VerifyError</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-25289"><code>KT-25289</code></a> Prohibit access to class members in the super constructor call of its companion and nested object</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-32753"><code>KT-32753</code></a> Prohibit <a href="https://github.com/JvmField"><code>@​JvmField</code></a> on property in primary constructor that overrides interface property</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-43433"><code>KT-43433</code></a> <code>Suspend conversion is disabled</code> message in cases where it is not supported and quickfix to update language version is suggested</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-49399"><code>KT-49399</code></a> Building repeatable annotation with Container nested class fails with ISE: &quot;Repeatable annotation class should have a container generated&quot;</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-49209"><code>KT-49209</code></a> Default upper bound for type variables should be non-null</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-49335"><code>KT-49335</code></a> NPE in <code>RepeatedAnnotationLowering.wrapAnnotationEntriesInContainer</code> when using <code>@Repeatable</code> annotation from different file</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-48876"><code>KT-48876</code></a> java.lang.UnsupportedOperationException: org.jetbrains.kotlin.ir.expressions.impl.IrReturnableBlockImpl@4a729df2</li>
<li><a href="https://youtrack.jetbrains.com/issue/KT-48131"><code>KT-48131</code></a> IAE &quot;Repeatable annotation container value must be a class reference&quot; on using Kotlin-repeatable annotation from dependency</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/JetBrains/kotlin/commit/829d1d887636689955b56beebdbb8725e908ef0f"><code>829d1d8</code></a> Add changelog for 1.6.0</li>
<li><a href="https://github.com/JetBrains/kotlin/commit/99b69aeebec79615608bf242be3f12fdb15062be"><code>99b69ae</code></a> Merge KT-MR-4942: Mark packages for relocation to fix classpath interferring ...</li>
<li><a href="https://github.com/JetBrains/kotlin/commit/583488e3cecfc3890ba845d86ef5cc16e340ff7f"><code>583488e</code></a> [scripting] Fix NPE in aether.kt</li>
<li><a href="https://github.com/JetBrains/kotlin/commit/0d1f3623b265fa311b25f01558c76c03eece3258"><code>0d1f362</code></a> Fix PureAndroidAndJavaConsumeMppLibIT working with test project</li>
<li><a href="https://github.com/JetBrains/kotlin/commit/46af453c2687981c866ec3d4ac097db7df0531de"><code>46af453</code></a> JVM KT-49613 don't generate indy reference to protected constructor</li>
<li><a href="https://github.com/JetBrains/kotlin/commit/d5275aaf07a3149a4d263ee4b768c7adcac25400"><code>d5275aa</code></a> Mark packages for relocation to fix classpath interferring in main-kts</li>
<li><a href="https://github.com/JetBrains/kotlin/commit/a3820d409d9f2c98d9619cef870bbfa211838a56"><code>a3820d4</code></a> JVM KT-49548 progression iterators can be tainted</li>
<li><a href="https://github.com/JetBrains/kotlin/commit/63044b115b9675e32f8f0a66bffd33cee44fc088"><code>63044b1</code></a> Update <code>-Xjvm-default</code> description</li>
<li><a href="https://github.com/JetBrains/kotlin/commit/e8e3c72649b688907aa574f667d73c9acd3fadaa"><code>e8e3c72</code></a> Update INTERFACE_CANT_CALL_DEFAULT_METHOD_VIA_SUPER message</li>
<li><a href="https://github.com/JetBrains/kotlin/commit/ddd02fecbe423dd1f95a8d7952aabc3149b76656"><code>ddd02fe</code></a> JvmDefault. Allow non default inheritance with special flag</li>
<li>Additional commits viewable in <a href="https://github.com/JetBrains/kotlin/compare/1.1.60...v1.6.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=org.jetbrains.kotlin:kotlin-stdlib&package-manager=maven&previous-version=1.1.60&new-version=1.6.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
[//]: # (dependabot-automerge-end)

---

<details>
<summary>Dependabot commands and options</summary>
<br />

You can trigger Dependabot actions by commenting on this PR:
- `@dependabot rebase` will rebase this PR
- `@dependabot recreate` will recreate this PR, overwriting any edits that have been made to it
- `@dependabot merge` will merge this PR after your CI passes on it
- `@dependabot squash and merge` will squash and merge this PR after your CI passes on it
- `@dependabot cancel merge` will cancel a previously requested merge and block automerging
- `@dependabot reopen` will reopen this PR if it is closed
- `@dependabot close` will close this PR and stop Dependabot recreating it. You can achieve the same result by closing it manually
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/bevel/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 22:43:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1983" class=".btn">#1983</a>
            </td>
            <td>
                <b>
                    [docs] update roadmap, and verify guide links
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Update roadmap, compatibility metrics
- Added troubleshooting links 



**Linked issue**
#1927 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 09:47:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/1982" class=".btn">#1982</a>
            </td>
            <td>
                <b>
                    [corda]: update platform r3 corda-ent helm value templates for fluxv2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

Signed-off-by: manikanta-darsi <manikanta.darsi@accenture.com>

**Changelog**
- Update platform r3 corda-ent helm value templates for fluxv2

 

**Reviewed by**
@sownak @suvajit-sarkar @jagpreetsinghsasan 

 

**Linked issue**
#1972 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-17 15:14:08 +0000 UTC
    </div>
</div>

