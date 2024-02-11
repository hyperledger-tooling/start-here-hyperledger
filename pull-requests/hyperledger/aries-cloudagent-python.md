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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2770" class=".btn">#2770</a>
            </td>
            <td>
                <b>
                    update admin route to include vcdi filter format
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
        Created At 2024-02-10 18:32:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2765" class=".btn">#2765</a>
            </td>
            <td>
                <b>
                    Reorganize the ACA-Py Documentation Files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR does a radical reorganization of the documents in the ACA-Py repository. The following is a summary of the changes:

- Most Markdown files in the root have been moved to the docs folder, and organized into folders that match those used on the [https://aca-py.org](https://aca-py.org) -- demo, gettingStarted, testing, deploying, etc.
- Expected files -- LICENSE, MAINTAINERS.md, README.md and the like were left in the root folder.
- The MD files in the `demo` folder were moved to `docs/demo' and a new README.md file added pointing to those.
- The previous Getting Started files were moved to the `docs/gettingStarted` folders.
- A pass was done to change all the links found (in a manual pass...) to be relative links and to the new location of the files.
- A pass was done to remove all of the MD lint warnings (other than spelling of ACA-Py/Aries/SSI terms).
- Some cleanup was done to external references -- changing references from greenlight ledger to BCovrin test, eliminating some references to old demos, adding references to the Traction Tutorial.
- New README.md files were needed -- such as in the root of the `docs` folder with pointers to guidance for maintaining both the ReadTheDocs documentation and the [https://aca-py.org](https://aca-py.org) documentation.
- I've not done anything with the ELK Stack MD documents -- will think about what to do with those later (if anything).

Not perfect, but I think it is close.

It is a lot of change. Would appreciate people browsing [my branch](https://github.com/swcurran/aries-cloudagent-python/tree/organize-docs) in the GitHub UI to scan for issues, and report them.  Important things to note are changes that need to be made before we merge this and more general updates that are overdue and needed.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-07 22:38:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2764" class=".btn">#2764</a>
            </td>
            <td>
                <b>
                    ⬆️ Update pytest-asyncio to 0.23.4 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Summary: 
⬆️ Upgrades pytest-asyncio to latest
✅ fix some test's event loop scopes (also mark some tests requiring askar or bbs)
🎉  resolves 2154 deprecation warnings
___
Original:
Reviewing test logs show that there are 2154 deprecation warnings coming from across 202 test files, each reporting:
```sh
  /home/runner/.cache/pypoetry/virtualenvs/aries-cloudagent-LQSjsNdA-py3.9/lib/python3.9/site-packages/pytest_asyncio/plugin.py:451: DeprecationWarning: pytest-asyncio detected an unclosed event loop when tearing down the event_loop
  fixture: <_UnixSelectorEventLoop running=False closed=False debug=False>
  pytest-asyncio will close the event loop for you, but future versions of the
  library will no longer do so. In order to ensure compatibility with future
  versions, please make sure that:
      1. Any custom "event_loop" fixture properly closes the loop after yielding it
      2. The scopes of your custom "event_loop" fixtures do not overlap
      3. Your code does not modify the event loop in async fixtures or tests
```

This indicates that the pytests are not configured correctly, or at least not in an up-to-date way.

These are the current test results after upgrading to the latest pytest-asyncio version
```sh
FAILED aries_cloudagent/revocation/models/tests/test_issuer_rev_reg_record.py::TestIssuerRevRegRecord::test_fix_ledger_entry - TypeError: the JSON object must be str, bytes or bytearray, not MagicMock
FAILED aries_cloudagent/vc/vc_ld/tests/test_manager.py::test_issue - pyld.jsonld.JsonLdError: ('Could not expand input before compaction.',)
FAILED aries_cloudagent/vc/vc_ld/tests/test_manager.py::test_issue_ed25519_2020 - pyld.jsonld.JsonLdError: ('Could not expand input before compaction.',)
FAILED aries_cloudagent/vc/vc_ld/tests/test_manager.py::test_issue_bbs - TypeError: sequence item 1: expected a bytes-like object, MagicMock found
FAILED aries_cloudagent/vc/vc_ld/tests/test_manager.py::test_store - pyld.jsonld.JsonLdError: ('Could not expand input before compaction.',)
ERROR aries_cloudagent/storage/vc_holder/tests/test_askar_vc_holder.py::TestAskarVCHolder::test_repr - TypeError: catching classes that do not inherit from BaseException is not allowed
ERROR aries_cloudagent/storage/vc_holder/tests/test_askar_vc_holder.py::TestAskarVCHolder::test_handle_parser_error - TypeError: catching classes that do not inherit from BaseException is not allowed
ERROR aries_cloudagent/storage/vc_holder/tests/test_askar_vc_holder.py::TestAskarVCHolder::test_sorting_vcrecord - TypeError: catching classes that do not inherit from BaseException is not allowed
ERROR aries_cloudagent/storage/vc_holder/tests/test_askar_vc_holder.py::TestAskarVCHolder::test_tag_query_valid_and_operator - TypeError: catching classes that do not inherit from BaseException is not allowed
ERROR aries_cloudagent/storage/vc_holder/tests/test_askar_vc_holder.py::TestAskarVCHolder::test_store_retrieve - TypeError: catching classes that do not inherit from BaseException is not allowed
ERROR aries_cloudagent/storage/vc_holder/tests/test_askar_vc_holder.py::TestAskarVCHolder::test_delete - TypeError: catching classes that do not inherit from BaseException is not allowed
ERROR aries_cloudagent/storage/vc_holder/tests/test_askar_vc_holder.py::TestAskarVCHolder::test_search - TypeError: catching classes that do not inherit from BaseException is not allowed
ERROR aries_cloudagent/storage/vc_holder/tests/test_askar_vc_holder.py::TestAskarVCHolder::test_tag_query - TypeError: catching classes that do not inherit from BaseException is not allowed
5 failed, 4490 passed, 598 skipped, 6 xfailed, 238 warnings, 8 errors in 128.86s (0:02:08)
```

Edit: these new test failures/errors all come down to either pytest scope needing to be a higher level, or tests that should be marked "to skip" (askar or bbs)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-07 13:11:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2763" class=".btn">#2763</a>
            </td>
            <td>
                <b>
                    Upgrade anoncreds to version 0.2.0-dev11
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
        Created At 2024-02-06 18:10:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2760" class=".btn">#2760</a>
            </td>
            <td>
                <b>
                    Move emit events to profile and delay sending until after commit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See issue #2000 

This update doesn't break anything ...  I haven't been able to duplicate the issue (by strategically inserting `sleep()` statements) so I can't 100% confirm that this fixes the issue, but I think it "should" ...

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-05 23:47:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2759" class=".btn">#2759</a>
            </td>
            <td>
                <b>
                    feat: add new format and implement VCDICredFormatHandler (Draft)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - add `VC_DI` in `CredFormat.Format`
- lay out `VCDICredFormatHandler`
- add new schema classes for cred offer and request
- implement CredExRecordVCDI

next step
- Create additional functions `create_credential_offer_vc_di` and `create_credential` in `AnoncredsIssuer`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-05 17:33:44 +0000 UTC
    </div>
</div>

