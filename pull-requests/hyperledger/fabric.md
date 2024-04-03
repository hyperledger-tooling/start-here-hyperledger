---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4793" class=".btn">#4793</a>
            </td>
            <td>
                <b>
                    Remove global level endpoints from the channel config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 16:46:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4792" class=".btn">#4792</a>
            </td>
            <td>
                <b>
                    Update profile data in create a channel doc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #4779

Finish the changes that were started in #4781 and #4788.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 13:55:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4791" class=".btn">#4791</a>
            </td>
            <td>
                <b>
                    fix warning during doc build (backport #4786)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix #4617 

- Bug fix
- New feature
- Improvement (improvement to code, performance, etc)
- Test update
- Documentation update

#### Description

```
$ python -m sphinx -T -E -b html -d _build/doctrees -D language=en . ~/html
Running Sphinx v7.2.6
myst v2.0.0: MdParserConfig(commonmark_only=False, gfm_only=False, enable_extensions=set(), disable_syntax=[], all_links_external=True, url_schemes=('http', 'https', 'mailto', 'ftp'), ref_domains=None, fence_as_directive=set(), number_code_blocks=[], title_to_header=False, heading_anchors=0, heading_slug_func=None, html_meta={}, footnote_transition=True, words_per_minute=200, substitutions={}, linkify_fuzzy_links=True, dmath_allow_labels=True, dmath_allow_space=True, dmath_allow_digits=True, dmath_double_inline=False, update_mathjax=True, mathjax_classes='tex2jax_process|mathjax_process|math|output_area', enable_checkboxes=False, suppress_warnings=[], highlight_code_blocks=True)
building [mo]: targets for 0 po files that are out of date
writing output...
building [html]: targets for 124 source files that are out of date
updating environment: [new config] 124 added, 0 changed, 0 removed
reading sources... [100%] write_first_app
looking for now-outdated files... none found
pickling environment... done
checking consistency... /Users/theholygrail/hyperledger/fabric/docs/source/build_network.rst: WARNING: document isn't included in any toctree
/Users/theholygrail/hyperledger/fabric/docs/source/github/github.rst: WARNING: document isn't included in any toctree
/Users/theholygrail/hyperledger/fabric/docs/source/msp-identity-validity-rules.rst: WARNING: document isn't included in any toctree
/Users/theholygrail/hyperledger/fabric/docs/source/policies.rst: WARNING: document isn't included in any toctree
/Users/theholygrail/hyperledger/fabric/docs/source/raft_bft_migration.md: WARNING: document isn't included in any toctree
/Users/theholygrail/hyperledger/fabric/docs/source/tutorial/installxcode.md: WARNING: document isn't included in any toctree
done
preparing documents... done
copying assets... copying static files... done
copying extra files... done
done
writing output... [100%] write_first_app
generating indices... genindex done
highlighting module code...
writing additional pages... search done
copying images... [100%] images/AppConceptsOverview.png
dumping search index in English (code: en)... done
dumping object inventory... done
build succeeded, 6 warnings.

The HTML pages are in ../../../../html.
```

Only warnings related to inclusion of document in toctree left
<hr>This is an automatic backport of pull request #4786 done by [Mergify](https://mergify.com).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 12:47:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4790" class=".btn">#4790</a>
            </td>
            <td>
                <b>
                    fix: close file in the PackageMetadata func (backport #4789)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                



#### Type of change



- Bug fix
- New feature
- Improvement (improvement to code, performance, etc)
- Test update
- Documentation update

#### Description
close file in the PackageMetadata func


#### Additional details




#### Related issues






<hr>This is an automatic backport of pull request #4789 done by [Mergify](https://mergify.com).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 12:35:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4789" class=".btn">#4789</a>
            </td>
            <td>
                <b>
                    fix: close file in the PackageMetadata func
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix
- New feature
- Improvement (improvement to code, performance, etc)
- Test update
- Documentation update

#### Description
close file in the PackageMetadata func
<!--- Describe your changes in detail, including motivation. -->

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Github issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

<!--
Checklist (DELETE AFTER READING):

- `Signed-off-by` added to commits (required for DCO check to pass)
- Tests have been added/updated (required for bug fixes and features)
- Unit and/or integration tests pass locally
- Run linters and checks locally using 'make checks'
- If change requires documentation updates, make updates in pull request,
  or open a separate issue and provide link
- Squash commits into a single commit, unless a stack of commits is
  intentional to assist reviewers or to preserve review comments.
- For additional contribution guidelines see the project's CONTRIBUTING.md file
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 06:43:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4788" class=".btn">#4788</a>
            </td>
            <td>
                <b>
                    Update profile data in create a channel doc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix #4779 

- Documentation update



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 04:03:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4786" class=".btn">#4786</a>
            </td>
            <td>
                <b>
                    fix warning during doc build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix #4617 

- Bug fix
- New feature
- Improvement (improvement to code, performance, etc)
- Test update
- Documentation update

#### Description

```
$ python -m sphinx -T -E -b html -d _build/doctrees -D language=en . ~/html
Running Sphinx v7.2.6
myst v2.0.0: MdParserConfig(commonmark_only=False, gfm_only=False, enable_extensions=set(), disable_syntax=[], all_links_external=True, url_schemes=('http', 'https', 'mailto', 'ftp'), ref_domains=None, fence_as_directive=set(), number_code_blocks=[], title_to_header=False, heading_anchors=0, heading_slug_func=None, html_meta={}, footnote_transition=True, words_per_minute=200, substitutions={}, linkify_fuzzy_links=True, dmath_allow_labels=True, dmath_allow_space=True, dmath_allow_digits=True, dmath_double_inline=False, update_mathjax=True, mathjax_classes='tex2jax_process|mathjax_process|math|output_area', enable_checkboxes=False, suppress_warnings=[], highlight_code_blocks=True)
building [mo]: targets for 0 po files that are out of date
writing output...
building [html]: targets for 124 source files that are out of date
updating environment: [new config] 124 added, 0 changed, 0 removed
reading sources... [100%] write_first_app
looking for now-outdated files... none found
pickling environment... done
checking consistency... /Users/theholygrail/hyperledger/fabric/docs/source/build_network.rst: WARNING: document isn't included in any toctree
/Users/theholygrail/hyperledger/fabric/docs/source/github/github.rst: WARNING: document isn't included in any toctree
/Users/theholygrail/hyperledger/fabric/docs/source/msp-identity-validity-rules.rst: WARNING: document isn't included in any toctree
/Users/theholygrail/hyperledger/fabric/docs/source/policies.rst: WARNING: document isn't included in any toctree
/Users/theholygrail/hyperledger/fabric/docs/source/raft_bft_migration.md: WARNING: document isn't included in any toctree
/Users/theholygrail/hyperledger/fabric/docs/source/tutorial/installxcode.md: WARNING: document isn't included in any toctree
done
preparing documents... done
copying assets... copying static files... done
copying extra files... done
done
writing output... [100%] write_first_app
generating indices... genindex done
highlighting module code...
writing additional pages... search done
copying images... [100%] images/AppConceptsOverview.png
dumping search index in English (code: en)... done
dumping object inventory... done
build succeeded, 6 warnings.

The HTML pages are in ../../../../html.
```

Only warnings related to inclusion of document in toctree left

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 18:47:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4785" class=".btn">#4785</a>
            </td>
            <td>
                <b>
                    Remove references to Jira in docs (backport #4783)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Jira system has been retired.
Remove the remaining doc reference to Jira.
<hr>This is an automatic backport of pull request #4783 done by [Mergify](https://mergify.com).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 16:37:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4784" class=".btn">#4784</a>
            </td>
            <td>
                <b>
                    add defer GinkgoRecover
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 16:20:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4783" class=".btn">#4783</a>
            </td>
            <td>
                <b>
                    Remove references to Jira in docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Jira system has been retired.
Remove the remaining doc reference to Jira.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 16:14:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4782" class=".btn">#4782</a>
            </td>
            <td>
                <b>
                    I change the RequestMaxBytes setting with the value from the config block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If the RequestMaxBytes parameter is set not equal to 0 when generating a genesis block (passed to the function in the options parameter), it will be ignored. This change corrects the situation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 15:46:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4781" class=".btn">#4781</a>
            </td>
            <td>
                <b>
                    update variable name in create a channel doc. 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs
fix #4779 
- Bug fix
- New feature
- Improvement (improvement to code, performance, etc)
- Test update
- Documentation update

#### Description

<!--- Describe your changes in detail, including motivation. -->

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Github issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

<!--
Checklist (DELETE AFTER READING):

- `Signed-off-by` added to commits (required for DCO check to pass)
- Tests have been added/updated (required for bug fixes and features)
- Unit and/or integration tests pass locally
- Run linters and checks locally using 'make checks'
- If change requires documentation updates, make updates in pull request,
  or open a separate issue and provide link
- Squash commits into a single commit, unless a stack of commits is
  intentional to assist reviewers or to preserve review comments.
- For additional contribution guidelines see the project's CONTRIBUTING.md file
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 14:41:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4778" class=".btn">#4778</a>
            </td>
            <td>
                <b>
                    Remove global-level endpoints from channel config - WIP
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- config update

#### Description

This PR aims to block the option to specify global-level endpoints and enforce that endpoints per org are defined. 

#### Related issues

 issue #4763 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 13:45:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4775" class=".btn">#4775</a>
            </td>
            <td>
                <b>
                    Deprecated fabric tools image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

Deprecated fabric tools image

#### Description

<!--- Describe your changes in detail, including motivation. -->

Deprecated fabric tools image

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->
Remove tools image related code for github action, make file, docker file, test data, test case.

#### Related issues

<!--- Include a link to any associated issues, e.g. Github issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

https://github.com/hyperledger/fabric-samples/pull/1186

<!--
Checklist (DELETE AFTER READING):

- `Signed-off-by` added to commits (required for DCO check to pass)
- Tests have been added/updated (required for bug fixes and features)
- Unit and/or integration tests pass locally
- Run linters and checks locally using 'make checks'
- If change requires documentation updates, make updates in pull request,
  or open a separate issue and provide link
- Squash commits into a single commit, unless a stack of commits is
  intentional to assist reviewers or to preserve review comments.
- For additional contribution guidelines see the project's CONTRIBUTING.md file
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-30 12:08:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4774" class=".btn">#4774</a>
            </td>
            <td>
                <b>
                    common: fix function name in comment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix
- New feature
- Improvement (improvement to code, performance, etc)
- Test update
- Documentation update

#### Description

<!--- Describe your changes in detail, including motivation. -->

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Github issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

<!--
Checklist (DELETE AFTER READING):

- `Signed-off-by` added to commits (required for DCO check to pass)
- Tests have been added/updated (required for bug fixes and features)
- Unit and/or integration tests pass locally
- Run linters and checks locally using 'make checks'
- If change requires documentation updates, make updates in pull request,
  or open a separate issue and provide link
- Squash commits into a single commit, unless a stack of commits is
  intentional to assist reviewers or to preserve review comments.
- For additional contribution guidelines see the project's CONTRIBUTING.md file
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-29 08:44:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4771" class=".btn">#4771</a>
            </td>
            <td>
                <b>
                    BFT synchronizer: integration test against an orderer that does block censorship
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                TEST update

* Run a 4 orderer smart bft cluster.
* Do 10 TXs.
* Shut down o4.
* Do 10 more TXs.
* Shutdown o1,o2,o3
* Prepares 3 orderer mocks with 20 TXs, with the addresses of o1,o2,o3
* Emulates block censorship
* Start o4
* O4 should detects the block censorship attempt and get all 20 blocks to its ledger

#### Related issues
BFT synchronizer: integration test against an orderer that does block censorship #4731
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-28 10:13:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4770" class=".btn">#4770</a>
            </td>
            <td>
                <b>
                    Update channel_update_tutorial.rst to follow the latest fabric-samples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix
- Documentation update

#### Description

Minor updates on  channel_update_tutorial.rst to follow the latest fabric-samples.

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Github issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

<!--
Checklist (DELETE AFTER READING):

- `Signed-off-by` added to commits (required for DCO check to pass)
- Tests have been added/updated (required for bug fixes and features)
- Unit and/or integration tests pass locally
- Run linters and checks locally using 'make checks'
- If change requires documentation updates, make updates in pull request,
  or open a separate issue and provide link
- Squash commits into a single commit, unless a stack of commits is
  intentional to assist reviewers or to preserve review comments.
- For additional contribution guidelines see the project's CONTRIBUTING.md file
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-28 03:01:24 +0000 UTC
    </div>
</div>

