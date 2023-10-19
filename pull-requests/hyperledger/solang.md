---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1570" class=".btn">#1570</a>
            </td>
            <td>
                <b>
                    Bump anchor and other dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update all the crates which can be updated easily.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-18 10:56:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1569" class=".btn">#1569</a>
            </td>
            <td>
                <b>
                    Bugfix: The type of a resolved assignments needs a storage deref
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When resolving an assignment, the resolved variable is always in memory and can't be of `Type::StorageRef`. Not dereferencing the type causes various issues in later compilation stages.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 18:44:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1568" class=".btn">#1568</a>
            </td>
            <td>
                <b>
                    Refactor library_using_for.sol for clarity and naming conventions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit refactors the library_using_for.sol code for better readability and adherence to naming conventions.

This pull request focuses on enhancing the [library_using_for.sol](https://github.com/hyperledger/solang/blob/main/docs/examples/library_using_for.sol). The changes improve the contract's readability and adherence to naming conventions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-16 16:23:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1567" class=".btn">#1567</a>
            </td>
            <td>
                <b>
                    Refactor library.sol for clarity and naming conventions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull request aims to improve the readability and documentation of the [library.sol ](https://github.com/hyperledger/solang/blob/main/docs/examples/library.sol)in the codebase. It includes changes such as renaming the contract and library to adhere to Solidity naming conventions, adding informative comments for function, and ensuring the library function has the correct visibility specifier. These modifications enhance the codebase's clarity.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-16 16:11:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1566" class=".btn">#1566</a>
            </td>
            <td>
                <b>
                    Update library documentation for clarity and correctness
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This Pull Request enhances the clarity and correctness of the documentation regarding [libraries ](https://solang.readthedocs.io/en/latest/language/interface_libraries.html#libraries)in Solidity. It addresses the restrictions applied to libraries, emphasizing their inability to modify the state and the necessity of using "view" or "pure" functions. These changes aim to provide more accurate guidance to users of the documentation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-16 15:43:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1565" class=".btn">#1565</a>
            </td>
            <td>
                <b>
                    Refactor interface.sol for better readability and adherence to best practices
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This Pull Request refactors the [Solidity code ](https://github.com/hyperledger/solang/blob/main/docs/examples/polkadot/interface.sol)in the repository to enhance readability and align with best practices. The changes include renaming contracts and functions for improved clarity, adding comments for documentation, and following the SPDX license identifier convention.

Key Changes:

- Renamed contracts and functions to follow naming conventions.
- Added comments for documentation.
- Added pragma version
- Followed the SPDX license identifier convention.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-16 15:19:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1564" class=".btn">#1564</a>
            </td>
            <td>
                <b>
                    Default flipper example should not include @program_id
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Users are getting the error "incorrect program id for instruction", which is confusing.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-16 13:09:04 +0000 UTC
    </div>
</div>

