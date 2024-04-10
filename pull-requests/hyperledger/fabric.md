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
                PR <a href="https://github.com/hyperledger/fabric/pull/4810" class=".btn">#4810</a>
            </td>
            <td>
                <b>
                    fix function name
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

- Documentation update

#### Description

<!--- Describe your changes in detail, including motivation. -->

fix function name 


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
        Created At 2024-04-10 11:49:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4809" class=".btn">#4809</a>
            </td>
            <td>
                <b>
                    Remove the outputAnchorPeersUpdate flag of configtxgen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR removes the configtxgen flag --outputAnchorPeersUpdate from the code.

#### Type of change

- New feature
- Documentation update

#### Description

In v3.0, we should use channel configuration updates and avoid using the "outputAnchorPeersUpdate" flag of configtxgen.
So, this PR removes the configtxgen flag --outputAnchorPeersUpdate from the code.

#### Related issues

Resolves #4765
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-10 08:41:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4808" class=".btn">#4808</a>
            </td>
            <td>
                <b>
                    chore: fix some typos in comments
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

fix some typos in comments

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
        Created At 2024-04-10 07:01:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4807" class=".btn">#4807</a>
            </td>
            <td>
                <b>
                    Remove elided badge from README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update

#### Description

removed Azure badge, which is 404


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-09 17:08:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4806" class=".btn">#4806</a>
            </td>
            <td>
                <b>
                    Move main to Golang v1.21.9.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Build Fabric using Go v1.21.9.

#### Additional details

n/a

#### Related issues

As per https://github.com/hyperledger/fabric/issues/4804

#### Release Note
None known.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-09 16:02:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4805" class=".btn">#4805</a>
            </td>
            <td>
                <b>
                    Move release 2.5.x to Golang v1.21.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Moves Fabric to being built using v1.21.9

#### Additional details

n/a

#### Related issues

https://github.com/hyperledger/fabric/issues/4804

#### Release Note

No known release impacts.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-09 15:58:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4803" class=".btn">#4803</a>
            </td>
            <td>
                <b>
                    Update gRPC dependency to address GO-2024-2687
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Use grpc.NewClient() instead of (soon to be) deprecated grpc.Dial().
- Update staticcheck version to avoid panic when running `make basic-checks` -- at least with Go 1.22.
- Regenerate documentation and remove trailing space that caused check failure.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-09 15:31:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4801" class=".btn">#4801</a>
            </td>
            <td>
                <b>
                    BFT chain unit tests: configure - remove node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Test update

#### Description

This PR aims to test a removal of a node as part of the BFT chain unit tests.

#### Related issues

#4008 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-07 12:48:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4800" class=".btn">#4800</a>
            </td>
            <td>
                <b>
                    Remove global-level endpoints from channel config - mid version - w.i.p.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

config update

#### Description

This PR aims to block the option to specify global-level endpoints and enforce that endpoints per org are defined.
Integration tests + unit tests were updated. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-07 08:52:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4799" class=".btn">#4799</a>
            </td>
            <td>
                <b>
                    core: fix some typos
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
        Created At 2024-04-07 06:33:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4798" class=".btn">#4798</a>
            </td>
            <td>
                <b>
                    add unit test for common/deliverclient/blocksprovider/delivery_requester
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
- Test update

#### Description
fix #4567 
Added unit test for deliveryRequester.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-07 00:11:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4797" class=".btn">#4797</a>
            </td>
            <td>
                <b>
                    Fix prerequisites doc page for content is partly occluded by navigator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Bug fix

#### Description
The change is intended to fix #4745 that the prerequisites page's content is partly occluded by navigator. As analyzed in the discussion of the issue, embedded div elements cause the issue. Therefore the change is going to remove all `<div>` elements 

(Due to accidentally closing the PR for Mergeify's backport(#4796), I am resolving the conflict and submitting it as a new PR.)

#### Additional details

#### Related issues
#4745 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-06 12:27:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4795" class=".btn">#4795</a>
            </td>
            <td>
                <b>
                    Fix prerequisites doc page for content is partly occluded by navigator
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

#### Description

<!--- Describe your changes in detail, including motivation. -->
The change is intended to fix #4745 that the prerequisites page's content is partly occluded by navigator. As analyzed in the discussion of the issue, embedded div elements cause the issue. Therefore the change is going to remove all `<div>` elements 

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues
#4745 

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
        Created At 2024-04-05 05:07:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4794" class=".btn">#4794</a>
            </td>
            <td>
                <b>
                    CouchDB index support for implicit collections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allow CouchDB index creation on implicit collection of organisations.

Indexes can be created for specific organisation's implicit collections at:
`META-INF/statedb/couchdb/collections/_implicit_org_<MSP_ID>` directory of the chaincode package.

Common indexes for all the organisations' implicit collection can be created at:
`META-INF/statedb/couchdb/collections/_implicit_org_*` directory of the chaincode package.
( `*` acts as wildcard for all organisation MSP ids. )

#### Type of change

- New feature

#### Description
Updated chaincode deployment handler to check if the indexes are for implicit collection if given collection directory name not explicitly defined in collection config. If the implicit collection indexes belong this handling peer's organisation or passed as global implicit collection indexes (using `*` notation), then indexes are created on corresponding implicit collection.

#### Additional details
- Please review the way of fetching `localMspId` directly using `viper` at `NewDB` constructor function.
- Added few more tar file entries to represent implicit collection indexes in unit tests. (However UT `TestHandleChainCodeDeployOnCouchDB` was already failing due to some other error)

#### Related issues
- #4780 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-04 08:10:24 +0000 UTC
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

