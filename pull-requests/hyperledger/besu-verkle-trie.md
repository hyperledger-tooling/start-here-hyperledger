---
layout: default
title: besu-verkle-trie
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu-verkle-trie
---

# besu-verkle-trie <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-verkle-trie){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-verkle-trie/pull/21" class=".btn">#21</a>
            </td>
            <td>
                <b>
                    Implement `toDot` Method and File Storing Mechanism for `VerkleTrie`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes https://github.com/neotheprogramist/besu-verkle-trie/issues/3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-23 07:56:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-verkle-trie/pull/20" class=".btn">#20</a>
            </td>
            <td>
                <b>
                    Ensure Clean State of Nodes After Commit in Besu-Verkle-Trie
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes https://github.com/neotheprogramist/besu-verkle-trie/issues/1
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-22 14:45:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-verkle-trie/pull/19" class=".btn">#19</a>
            </td>
            <td>
                <b>
                    improve pedersen vector commitment docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Small change, this is a bit confusing - IPA is used in proofs, for the trie we only need Pedersen commitment (MSM)

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-22 11:51:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-verkle-trie/pull/18" class=".btn">#18</a>
            </td>
            <td>
                <b>
                    Fix `classifier` Property Issue in Gradle Build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes https://github.com/visoftsolutions/besu-verkle-trie/issues/2

> ## Description
> 
> This PR addresses a build failure in the `besu-verkle-trie` project while executing the `gradle` command. The error was caused by the use of the deprecated `classifier` property in the `build.gradle` file.
> ### Error Details
> 
> Running the `gradle` command resulted in the following error:
> 
> ```
> $ gradle
> 
> FAILURE: Build failed with an exception.
> 
> * Where:
> Build file './besu-verkle-trie/build.gradle' line: 111
> 
> * What went wrong:
> A problem occurred evaluating root project 'besu-verkle-trie'.
> > Could not set unknown property 'classifier' for task ':sourcesJar' of type org.gradle.api.tasks.bundling.Jar.
> ...
> ```
> 
> ### Cause
> 
> The issue was due to the use of the `classifier` key, which has been deprecated. The problematic code snippet was:
> 
> ```groovy
>   task sourcesJar(type: Jar, dependsOn: classes) {
>     archiveBaseName = 'besu-verkle.trie'
>     classifier = 'sources'
>     from sourceSets.main.allSource
>   }
> 
>   task javadocJar(type: Jar, dependsOn: javadoc) {
>     archiveBaseName = 'besu-verkle.trie'
>     classifier = 'javadoc'
>     from javadoc.destinationDir
>   }
> ```
> 
> ### Resolution
> 
> The `classifier` property has been replaced with `archiveClassifier` to maintain compatibility with the latest version of Gradle. The updated code is as follows:
> 
> ```groovy
>   task sourcesJar(type: Jar, dependsOn: classes) {
>     archiveBaseName = 'besu-verkle.trie'
>     archiveClassifier = 'sources'
>     from sourceSets.main.allSource
>   }
> 
>   task javadocJar(type: Jar, dependsOn: javadoc) {
>     archiveBaseName = 'besu-verkle.trie'
>     archiveClassifier = 'javadoc'
>     from javadoc.destinationDir
>   }
> ```
> 
> ## Impact
> 
> This change ensures compatibility with Gradle 9.0 and resolves the build failure issue.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-21 17:30:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-verkle-trie/pull/17" class=".btn">#17</a>
            </td>
            <td>
                <b>
                    Implement `toDot` Method and File Storing Mechanism for `VerkleTrie`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes https://github.com/visoftsolutions/besu-verkle-trie/issues/1

> #### Description
> 
> This issue aims to enhance the functionality of `VerkleTrie` in two significant ways:
> 
>     1. **Implementing `toDot` Method for String Representation:**
>        
>        * Develop a method `toDot` for `VerkleTrie` to create a human-readable string representation in [Dot format](https://en.wikipedia.org/wiki/DOT_%28graph_description_language%29). This feature will aid in debugging and visualizing the `VerkleTrie` structure.
>        * The `toDot` method should include:
>          
>          * `BranchNodes` with `commitment` attribute.
>          * `StemNodes` with `stem`, `leftCommitment`, and `rightCommitment` attributes.
>          * `LeafNodes` with `suffix` and `value` attributes.
>          * A `location` attribute for each node to uniquely name them.
> 
>     2. **Implementing File Storing Mechanism for `toDot` Output:**
>        
>        * Extend the `toDot` functionality to include the capability of saving its output into a file. This addition will facilitate users in saving the `VerkleTrie` graphical representation for further analysis or sharing.
>        * The file storing feature should:
>          
>          * Allow efficient and user-friendly saving of the Dot format output.
>          * Handle errors related to write permissions or file system issues.
>          * Optionally let users specify the file path and name for storing the output.
> 
> 
> #### Expected Behavior
> 
>     * `toDot` returns the tree representation in Dot format with specified attributes for different node types.
> 
>     * Users can save the Dot format output of `VerkleTrie` into a file, enhancing the method's usability for debugging and analysis.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-21 17:21:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-verkle-trie/pull/13" class=".btn">#13</a>
            </td>
            <td>
                <b>
                    FIX: bug in TrieKeyAdaptor swapLastByte
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
There was a bug in TrieKeyAdaptor.swapLastByte : it did not take properly into account the last byte of a UInt256.
Some minor improvements where also made:

  1. UInt256 are reversed to littleEndian as it should be.
  2. All indexes are passed as UInt256.
  3. More tests have been included for contract code chunking.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-17 12:05:02 +0000 UTC
    </div>
</div>

