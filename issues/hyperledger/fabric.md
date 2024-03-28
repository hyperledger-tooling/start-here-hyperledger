---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/fabric/issues/4617" class=".btn">4617</a>
            </td>
            <td>
                <b>
                    Fix documentation errors and warnings from Sphinx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">workitem</span>
            </td>
            <td>
                ### Current Status

```
# python -m sphinx -T -E -b html -d _build/doctrees -D language=en . ~/html
Running Sphinx v7.2.6
myst v2.0.0: MdParserConfig(commonmark_only=False, gfm_only=False, enable_extensions=set(), disable_syntax=[], all_links_external=False, url_schemes=('http', 'https', 'mailto', 'ftp'), ref_domains=None, fence_as_directive=set(), number_code_blocks=[], title_to_header=False, heading_anchors=0, heading_slug_func=None, html_meta={}, footnote_transition=True, words_per_minute=200, substitutions={}, linkify_fuzzy_links=True, dmath_allow_labels=True, dmath_allow_space=True, dmath_allow_digits=True, dmath_double_inline=False, update_mathjax=True, mathjax_classes='tex2jax_process|mathjax_process|math|output_area', enable_checkboxes=False, suppress_warnings=[], highlight_code_blocks=True)
building [mo]: targets for 0 po files that are out of date
writing output... 
building [html]: targets for 130 source files that are out of date
updating environment: [new config] 130 added, 0 changed, 0 removed
reading sources... [100%] write_first_app
/root/docs/source/channel_update_tutorial.rst:196: ERROR: Error in "code" directive:
maximum 1 argument(s) allowed, 3 supplied.

.. code:: bash
  cd ..
/root/docs/source/channel_update_tutorial.rst:253: ERROR: Error in "code" directive:
maximum 1 argument(s) allowed, 3 supplied.

.. code:: bash
   cd channel-artifacts
/root/docs/source/channel_update_tutorial.rst:356: ERROR: Error in "code" directive:
maximum 1 argument(s) allowed, 3 supplied.

.. code:: bash
   cd ..
/root/docs/source/channel_update_tutorial.rst:687: ERROR: Error in "code" directive:
maximum 1 argument(s) allowed, 3 supplied.

.. code:: bash
   cd channel-artifacts
/root/docs/source/channel_update_tutorial.rst:760: ERROR: Error in "code" directive:
maximum 1 argument(s) allowed, 3 supplied.

.. code:: bash
   cd ..
/root/docs/source/deployment_guide_overview.rst:2: WARNING: Duplicate explicit target name: "in the sampleconfig directory of hyperledger fabric".
/root/docs/source/peers/peers.md:30: WARNING: Non-consecutive header level increase; H1 to H3 [myst.header]
/root/docs/source/updating_capabilities.md:52: WARNING: Non-consecutive header level increase; H2 to H4 [myst.header]
looking for now-outdated files... none found
pickling environment... done
checking consistency... /root/docs/source/build_network.rst: WARNING: document isn't included in any toctree
/root/docs/source/developapps/apis.md: WARNING: document isn't included in any toctree
/root/docs/source/github/github.rst: WARNING: document isn't included in any toctree
/root/docs/source/ledger.rst: WARNING: document isn't included in any toctree
/root/docs/source/msp-identity-validity-rules.rst: WARNING: document isn't included in any toctree
/root/docs/source/policies.rst: WARNING: document isn't included in any toctree
/root/docs/source/tutorial/installxcode.md: WARNING: document isn't included in any toctree
```

### Goal

Fix the Sphinx warnings in the Fabric docs.

### Solution

Fix the Sphinx warnings in the Fabric docs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 20:46:39 +0000 UTC
    </div>
</div>

