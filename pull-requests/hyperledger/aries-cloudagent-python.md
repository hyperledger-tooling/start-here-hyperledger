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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2758" class=".btn">#2758</a>
            </td>
            <td>
                <b>
                    Update anoncreds to 0.2.0-dev10
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
        Created At 2024-02-03 01:02:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2756" class=".btn">#2756</a>
            </td>
            <td>
                <b>
                    Fix deprecation warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Such as:
- `DeprecationWarning: pkg_resources is deprecated as an API` 
  - ♻️  Refactored to use `importlib`
- `RemovedInMarshmallow4Warning: Passing field metadata as keyword arguments is deprecated. Use the explicit `metadata=...` argument instead.` 
  - 🎨 description and example fields must be wrapped as metadata
- various `DeprecationWarning`s
  - fixed by :arrow_up: Upgrading `jsonpath-ng`, `Markdown`, and `rlp`

The bulk of the warnings seem to stem from a mixing of pytest-asyncio alongside unittest.IsolatedAsyncioTestCase:
```sh
pytest_asyncio/plugin.py:451: DeprecationWarning: pytest-asyncio detected an unclosed event loop when tearing down the event_loop
  fixture: <_UnixSelectorEventLoop running=False closed=False debug=False>
  pytest-asyncio will close the event loop for you, but future versions of the
  library will no longer do so. In order to ensure compatibility with future
  versions, please make sure that:
      1. Any custom "event_loop" fixture properly closes the loop after yielding it
      2. The scopes of your custom "event_loop" fixtures do not overlap
      3. Your code does not modify the event loop in async fixtures or tests
```
This is because IsolatedAsyncioTestCase manages its own event loop. Not clear to me yet what the fix or config should be to solve this.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-02 10:21:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2755" class=".btn">#2755</a>
            </td>
            <td>
                <b>
                    Remove asynctest dependency and fix "coroutine not awaited" warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As initially done by @dbluhm in #2566, this drops the asynctest dependency, as it's massively out of date and generates hundreds of warnings in the tests - making it harder to improve on other warning logs.

It seems the dependency was subtly reintroduced in #2596. This PR attempts to refactor tests to only use unittest, as they fully support async tests since python 3.8 and external deps for async tests shouldn't be needed.

Edit: Summary of changes:

:heavy_minus_sign: Drops dependencies: `asynctest` (deprecated), and `async-case` (unused)

:recycle: Refactors tests to use unittest mocking

:white_check_mark:  Includes fixes for 3 tests that were silently not implemented properly (`coroutine not awaited`)

:construction_worker: Added a condition to tests workflow that it will fail if "coroutine not awaited" appears in the warning logs. (Here's a [sample result](https://github.com/hyperledger/aries-cloudagent-python/actions/runs/7756059087/job/21152653635?pr=2755) of a workflow failing, where all tests passed, but the warning appears in logs)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-02 09:40:51 +0000 UTC
    </div>
</div>

