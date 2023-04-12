---
layout: default
title: karma-charity-platform
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/karma-charity-platform
---

# karma-charity-platform <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/karma-charity-platform){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/93" class=".btn">#93</a>
            </td>
            <td>
                <b>
                    Bump xml2js and typeorm in /chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Removes [xml2js](https://github.com/Leonidas-from-XIV/node-xml2js). It's no longer used after updating ancestor dependency [typeorm](https://github.com/typeorm/typeorm). These dependencies need to be updated together.

Removes `xml2js`

Updates `typeorm` from 0.3.8 to 0.3.14
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/typeorm/typeorm/releases">typeorm's releases</a>.</em></p>
<blockquote>
<h2>0.3.14</h2>
<h3>Bug Fixes</h3>
<ul>
<li>drop xml &amp; yml connection option support. Addresses security issues in underlying dependency (<a href="https://redirect.github.com/typeorm/typeorm/issues/9930">#9930</a>) (<a href="https://github.com/typeorm/typeorm/commit/7dac12c2b18be34fb63ebfde988eb0825ec21384">7dac12c</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>QueryBuilder performance optimizations (<a href="https://redirect.github.com/typeorm/typeorm/issues/9914">#9914</a>) (<a href="https://github.com/typeorm/typeorm/commit/12e9db07b6b9676e63fff5f55a45b1d269716ed9">12e9db0</a>)</li>
</ul>
<h2>0.3.13</h2>
<h3>Bug Fixes</h3>
<ul>
<li>firstCapital=true not working in camelCase() function (<a href="https://github.com/typeorm/typeorm/commit/f1330ad6e23bea65a16b4f1c4199f10f3fa7282b">f1330ad</a>)</li>
<li>handles &quot;query&quot; relation loading strategy for TreeRepositories (<a href="https://redirect.github.com/typeorm/typeorm/issues/9680">#9680</a>) (<a href="https://github.com/typeorm/typeorm/commit/a11809e1b20cc77fd2767b8bab2500a0c7e20d23">a11809e</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9673">#9673</a></li>
<li>improve EntityNotFound error message in QueryBuilder.findOneOrFail (<a href="https://redirect.github.com/typeorm/typeorm/issues/9872">#9872</a>) (<a href="https://github.com/typeorm/typeorm/commit/f7f68178640120d8c1e92b8c9be0eeaa8262b4f3">f7f6817</a>)</li>
<li>loading tables with fk in sqlite query runner (<a href="https://redirect.github.com/typeorm/typeorm/issues/9875">#9875</a>) (<a href="https://github.com/typeorm/typeorm/commit/4997da054b5cfafdbdf374b3e554e5c4e0590da7">4997da0</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9266">#9266</a></li>
<li>prevent foreign key support during migration batch under sqlite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9775">#9775</a>) (<a href="https://github.com/typeorm/typeorm/commit/197cc05e90c0182357d85aa1ce7ae45de99d9d98">197cc05</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9770">#9770</a></li>
<li>proper default value on generating migration when default value is a function calling [Postgres] (<a href="https://redirect.github.com/typeorm/typeorm/issues/9830">#9830</a>) (<a href="https://github.com/typeorm/typeorm/commit/bebba05388a40a9f278a450d4a988865c158abb7">bebba05</a>)</li>
<li>react-native doesn't properly work in ESM projects because of circular dependency (<a href="https://redirect.github.com/typeorm/typeorm/issues/9765">#9765</a>) (<a href="https://github.com/typeorm/typeorm/commit/099fcd9b104bc930faea08f97ee3d5610118e0c4">099fcd9</a>)</li>
<li>resolve issues for mssql migration when simple-enum was changed (<a href="https://github.com/typeorm/typeorm/commit/cb154d4ca36cda251fcb9eb05a29b7758ae813cf">cb154d4</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/7785">#7785</a> <a href="https://redirect.github.com/typeorm/typeorm/issues/9457">#9457</a> <a href="https://redirect.github.com/typeorm/typeorm/issues/7785">#7785</a> <a href="https://redirect.github.com/typeorm/typeorm/issues/9457">#9457</a></li>
<li>resolves issue with mssql column recreation (<a href="https://redirect.github.com/typeorm/typeorm/issues/9773">#9773</a>) (<a href="https://github.com/typeorm/typeorm/commit/07221a364682b567533c93130efb4f5189e009a9">07221a3</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9399">#9399</a></li>
<li>transform values for FindOperators <a href="https://redirect.github.com/typeorm/typeorm/issues/9381">#9381</a> (<a href="https://redirect.github.com/typeorm/typeorm/issues/9777">#9777</a>) (<a href="https://github.com/typeorm/typeorm/commit/de1228deace974eca3e9dd3956208ebe4cd9347f">de1228d</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9816">#9816</a></li>
<li>use forward slashes when normalizing path (<a href="https://redirect.github.com/typeorm/typeorm/issues/9768">#9768</a>) (<a href="https://github.com/typeorm/typeorm/commit/58fc08840a4a64ca1935391f4709a784c3f0b373">58fc088</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9766">#9766</a></li>
<li>use object create if entity skip constructor is set (<a href="https://redirect.github.com/typeorm/typeorm/issues/9831">#9831</a>) (<a href="https://github.com/typeorm/typeorm/commit/a8689795dad796338e2a291a6a2fda89b00ef243">a868979</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>add support for json datatype for sqlite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9744">#9744</a>) (<a href="https://github.com/typeorm/typeorm/commit/4ac8c00117417ae622368aabe36d0fd5c676bd00">4ac8c00</a>)</li>
<li>add support for STI on EntitySchema (<a href="https://redirect.github.com/typeorm/typeorm/issues/9834">#9834</a>) (<a href="https://github.com/typeorm/typeorm/commit/bc306fb5a2c4dc02d04632af2b2f6c697a684356">bc306fb</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9833">#9833</a></li>
<li>allow type FindOptionsOrderValue for order by object property (<a href="https://redirect.github.com/typeorm/typeorm/issues/9895">#9895</a>) (<a href="https://redirect.github.com/typeorm/typeorm/issues/9896">#9896</a>) (<a href="https://github.com/typeorm/typeorm/commit/0814970a9cc2c958199c9d74d1ef313de43dab50">0814970</a>)</li>
<li>Broadcast identifier for removed related entities  (<a href="https://redirect.github.com/typeorm/typeorm/issues/9913">#9913</a>) (<a href="https://github.com/typeorm/typeorm/commit/f530811b0da2863711db3467e55bf815c66b4b4b">f530811</a>)</li>
<li>leftJoinAndMapOne and innerJoinAndMapOne map result to entity (<a href="https://redirect.github.com/typeorm/typeorm/issues/9354">#9354</a>) (<a href="https://github.com/typeorm/typeorm/commit/947ffc34324c1d692496804e43dafa6302efc1db">947ffc3</a>)</li>
</ul>
<h2>0.3.12</h2>
<h3>Bug Fixes</h3>
<ul>
<li>allow to pass ObjectLiteral in mongo find where condition (<a href="https://redirect.github.com/typeorm/typeorm/issues/9632">#9632</a>) (<a href="https://github.com/typeorm/typeorm/commit/4eda5df8693d1a659ff5c3461124cf05619fdd72">4eda5df</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9518">#9518</a></li>
<li>DataSource.setOptions doesn't properly update the database in the drivers (<a href="https://redirect.github.com/typeorm/typeorm/issues/9635">#9635</a>) (<a href="https://github.com/typeorm/typeorm/commit/a95bed7c05d10eb4b508e225faa4cb3c7ea7944f">a95bed7</a>)</li>
<li>Fix grammar error in no migrations found log (<a href="https://redirect.github.com/typeorm/typeorm/issues/9754">#9754</a>) (<a href="https://github.com/typeorm/typeorm/commit/6fb212187fdf97c07c41aad20d4f5503dfd44215">6fb2121</a>)</li>
<li>improved <code>FindOptionsWhere</code> behavior with union types (<a href="https://redirect.github.com/typeorm/typeorm/issues/9607">#9607</a>) (<a href="https://github.com/typeorm/typeorm/commit/7726f5ad1ec0c826510202a0f2cbeea705547eee">7726f5a</a>)</li>
<li>Incorrect enum default value when table name contains dash character (<a href="https://redirect.github.com/typeorm/typeorm/issues/9685">#9685</a>) (<a href="https://github.com/typeorm/typeorm/commit/b3b0c118a40441b31ac18ee7ce0cea0696b701ab">b3b0c11</a>)</li>
<li>incorrect sorting of entities with multi-inheritances (<a href="https://redirect.github.com/typeorm/typeorm/issues/9406">#9406</a>) (<a href="https://github.com/typeorm/typeorm/commit/54ca9dd801a77e011c2faf056b9e12845ccde82b">54ca9dd</a>)</li>
<li>make sure &quot;require&quot; is defined in the environment (<a href="https://github.com/typeorm/typeorm/commit/1a9b9fbcd683b2a28acbd26e39ac98dc6b60f001">1a9b9fb</a>)</li>
<li>materialized hints support for cte (<a href="https://redirect.github.com/typeorm/typeorm/issues/9605">#9605</a>) (<a href="https://github.com/typeorm/typeorm/commit/67973b4726500fc835639ffc302e0b6b20093df4">67973b4</a>)</li>
<li>multiple select queries during db sync in sqlite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9639">#9639</a>) (<a href="https://github.com/typeorm/typeorm/commit/6c928a4aa002cf5db0733055c0a754e97e4b43b3">6c928a4</a>)</li>
<li>overriding caching settings when alwaysEnabled is true (<a href="https://redirect.github.com/typeorm/typeorm/issues/9731">#9731</a>) (<a href="https://github.com/typeorm/typeorm/commit/4df969ea6254f9f69c371a72d80e857ab7c1f62d">4df969e</a>)</li>
<li>redundant Unique constraint on primary join column in Postgres (<a href="https://redirect.github.com/typeorm/typeorm/issues/9677">#9677</a>) (<a href="https://github.com/typeorm/typeorm/commit/b8704f87d2e06c048dea3f0b408ab18738acf7d7">b8704f8</a>)</li>
<li>remove unnecessary .js extension in imports (<a href="https://redirect.github.com/typeorm/typeorm/issues/9713">#9713</a>) (<a href="https://github.com/typeorm/typeorm/commit/6b37e3818bd74541cadbd44e55c84df510e41e3a">6b37e38</a>)</li>
<li>resolve issue with &quot;simple-enum&quot; synchronization in SQLite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9716">#9716</a>) (<a href="https://github.com/typeorm/typeorm/commit/c77c43e2423201bdc2ede85ae921447570685585">c77c43e</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9715">#9715</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/typeorm/typeorm/blob/master/CHANGELOG.md">typeorm's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/typeorm/typeorm/compare/0.3.12...0.3.14">0.3.14</a> (2023-04-09)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>drop xml &amp; yml connection option support. Addresses security issues in underlying dependency (<a href="https://redirect.github.com/typeorm/typeorm/issues/9930">#9930</a>) (<a href="https://github.com/typeorm/typeorm/commit/7dac12c2b18be34fb63ebfde988eb0825ec21384">7dac12c</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>QueryBuilder performance optimizations (<a href="https://redirect.github.com/typeorm/typeorm/issues/9914">#9914</a>) (<a href="https://github.com/typeorm/typeorm/commit/12e9db07b6b9676e63fff5f55a45b1d269716ed9">12e9db0</a>)</li>
</ul>
<h2><a href="https://github.com/typeorm/typeorm/compare/0.3.12...0.3.13">0.3.13</a> (2023-04-06)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>firstCapital=true not working in camelCase() function (<a href="https://github.com/typeorm/typeorm/commit/f1330ad6e23bea65a16b4f1c4199f10f3fa7282b">f1330ad</a>)</li>
<li>handles &quot;query&quot; relation loading strategy for TreeRepositories (<a href="https://redirect.github.com/typeorm/typeorm/issues/9680">#9680</a>) (<a href="https://github.com/typeorm/typeorm/commit/a11809e1b20cc77fd2767b8bab2500a0c7e20d23">a11809e</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9673">#9673</a></li>
<li>improve EntityNotFound error message in QueryBuilder.findOneOrFail (<a href="https://redirect.github.com/typeorm/typeorm/issues/9872">#9872</a>) (<a href="https://github.com/typeorm/typeorm/commit/f7f68178640120d8c1e92b8c9be0eeaa8262b4f3">f7f6817</a>)</li>
<li>loading tables with fk in sqlite query runner (<a href="https://redirect.github.com/typeorm/typeorm/issues/9875">#9875</a>) (<a href="https://github.com/typeorm/typeorm/commit/4997da054b5cfafdbdf374b3e554e5c4e0590da7">4997da0</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9266">#9266</a></li>
<li>prevent foreign key support during migration batch under sqlite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9775">#9775</a>) (<a href="https://github.com/typeorm/typeorm/commit/197cc05e90c0182357d85aa1ce7ae45de99d9d98">197cc05</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9770">#9770</a></li>
<li>proper default value on generating migration when default value is a function calling [Postgres] (<a href="https://redirect.github.com/typeorm/typeorm/issues/9830">#9830</a>) (<a href="https://github.com/typeorm/typeorm/commit/bebba05388a40a9f278a450d4a988865c158abb7">bebba05</a>)</li>
<li>react-native doesn't properly work in ESM projects because of circular dependency (<a href="https://redirect.github.com/typeorm/typeorm/issues/9765">#9765</a>) (<a href="https://github.com/typeorm/typeorm/commit/099fcd9b104bc930faea08f97ee3d5610118e0c4">099fcd9</a>)</li>
<li>resolve issues for mssql migration when simple-enum was changed (<a href="https://github.com/typeorm/typeorm/commit/cb154d4ca36cda251fcb9eb05a29b7758ae813cf">cb154d4</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/7785">#7785</a> <a href="https://redirect.github.com/typeorm/typeorm/issues/9457">#9457</a> <a href="https://redirect.github.com/typeorm/typeorm/issues/7785">#7785</a> <a href="https://redirect.github.com/typeorm/typeorm/issues/9457">#9457</a></li>
<li>resolves issue with mssql column recreation (<a href="https://redirect.github.com/typeorm/typeorm/issues/9773">#9773</a>) (<a href="https://github.com/typeorm/typeorm/commit/07221a364682b567533c93130efb4f5189e009a9">07221a3</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9399">#9399</a></li>
<li>transform values for FindOperators <a href="https://redirect.github.com/typeorm/typeorm/issues/9381">#9381</a> (<a href="https://redirect.github.com/typeorm/typeorm/issues/9777">#9777</a>) (<a href="https://github.com/typeorm/typeorm/commit/de1228deace974eca3e9dd3956208ebe4cd9347f">de1228d</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9816">#9816</a></li>
<li>use forward slashes when normalizing path (<a href="https://redirect.github.com/typeorm/typeorm/issues/9768">#9768</a>) (<a href="https://github.com/typeorm/typeorm/commit/58fc08840a4a64ca1935391f4709a784c3f0b373">58fc088</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9766">#9766</a></li>
<li>use object create if entity skip constructor is set (<a href="https://redirect.github.com/typeorm/typeorm/issues/9831">#9831</a>) (<a href="https://github.com/typeorm/typeorm/commit/a8689795dad796338e2a291a6a2fda89b00ef243">a868979</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>add support for json datatype for sqlite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9744">#9744</a>) (<a href="https://github.com/typeorm/typeorm/commit/4ac8c00117417ae622368aabe36d0fd5c676bd00">4ac8c00</a>)</li>
<li>add support for STI on EntitySchema (<a href="https://redirect.github.com/typeorm/typeorm/issues/9834">#9834</a>) (<a href="https://github.com/typeorm/typeorm/commit/bc306fb5a2c4dc02d04632af2b2f6c697a684356">bc306fb</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9833">#9833</a></li>
<li>allow type FindOptionsOrderValue for order by object property (<a href="https://redirect.github.com/typeorm/typeorm/issues/9895">#9895</a>) (<a href="https://redirect.github.com/typeorm/typeorm/issues/9896">#9896</a>) (<a href="https://github.com/typeorm/typeorm/commit/0814970a9cc2c958199c9d74d1ef313de43dab50">0814970</a>)</li>
<li>Broadcast identifier for removed related entities  (<a href="https://redirect.github.com/typeorm/typeorm/issues/9913">#9913</a>) (<a href="https://github.com/typeorm/typeorm/commit/f530811b0da2863711db3467e55bf815c66b4b4b">f530811</a>)</li>
<li>leftJoinAndMapOne and innerJoinAndMapOne map result to entity (<a href="https://redirect.github.com/typeorm/typeorm/issues/9354">#9354</a>) (<a href="https://github.com/typeorm/typeorm/commit/947ffc34324c1d692496804e43dafa6302efc1db">947ffc3</a>)</li>
</ul>
<h2><a href="https://github.com/typeorm/typeorm/compare/0.3.11...0.3.12">0.3.12</a> (2023-02-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>allow to pass ObjectLiteral in mongo find where condition (<a href="https://redirect.github.com/typeorm/typeorm/issues/9632">#9632</a>) (<a href="https://github.com/typeorm/typeorm/commit/4eda5df8693d1a659ff5c3461124cf05619fdd72">4eda5df</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9518">#9518</a></li>
<li>DataSource.setOptions doesn't properly update the database in the drivers (<a href="https://redirect.github.com/typeorm/typeorm/issues/9635">#9635</a>) (<a href="https://github.com/typeorm/typeorm/commit/a95bed7c05d10eb4b508e225faa4cb3c7ea7944f">a95bed7</a>)</li>
<li>Fix grammar error in no migrations found log (<a href="https://redirect.github.com/typeorm/typeorm/issues/9754">#9754</a>) (<a href="https://github.com/typeorm/typeorm/commit/6fb212187fdf97c07c41aad20d4f5503dfd44215">6fb2121</a>)</li>
<li>improved <code>FindOptionsWhere</code> behavior with union types (<a href="https://redirect.github.com/typeorm/typeorm/issues/9607">#9607</a>) (<a href="https://github.com/typeorm/typeorm/commit/7726f5ad1ec0c826510202a0f2cbeea705547eee">7726f5a</a>)</li>
<li>Incorrect enum default value when table name contains dash character (<a href="https://redirect.github.com/typeorm/typeorm/issues/9685">#9685</a>) (<a href="https://github.com/typeorm/typeorm/commit/b3b0c118a40441b31ac18ee7ce0cea0696b701ab">b3b0c11</a>)</li>
<li>incorrect sorting of entities with multi-inheritances (<a href="https://redirect.github.com/typeorm/typeorm/issues/9406">#9406</a>) (<a href="https://github.com/typeorm/typeorm/commit/54ca9dd801a77e011c2faf056b9e12845ccde82b">54ca9dd</a>)</li>
<li>make sure &quot;require&quot; is defined in the environment (<a href="https://github.com/typeorm/typeorm/commit/1a9b9fbcd683b2a28acbd26e39ac98dc6b60f001">1a9b9fb</a>)</li>
<li>materialized hints support for cte (<a href="https://redirect.github.com/typeorm/typeorm/issues/9605">#9605</a>) (<a href="https://github.com/typeorm/typeorm/commit/67973b4726500fc835639ffc302e0b6b20093df4">67973b4</a>)</li>
<li>multiple select queries during db sync in sqlite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9639">#9639</a>) (<a href="https://github.com/typeorm/typeorm/commit/6c928a4aa002cf5db0733055c0a754e97e4b43b3">6c928a4</a>)</li>
<li>overriding caching settings when alwaysEnabled is true (<a href="https://redirect.github.com/typeorm/typeorm/issues/9731">#9731</a>) (<a href="https://github.com/typeorm/typeorm/commit/4df969ea6254f9f69c371a72d80e857ab7c1f62d">4df969e</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/typeorm/typeorm/commit/5e3c565dce843b2deeefa3327340a79e0fc54e66"><code>5e3c565</code></a> version bump</li>
<li><a href="https://github.com/typeorm/typeorm/commit/7dac12c2b18be34fb63ebfde988eb0825ec21384"><code>7dac12c</code></a> fix: drop xml &amp; yml connection option support (<a href="https://redirect.github.com/typeorm/typeorm/issues/9930">#9930</a>)</li>
<li><a href="https://github.com/typeorm/typeorm/commit/daf1b47a609cb5090b71e537668ee115a98b1dc9"><code>daf1b47</code></a> fix: wrong dependency version in init command</li>
<li><a href="https://github.com/typeorm/typeorm/commit/0194f179fee8f346bbf82325716df6935aebda5e"><code>0194f17</code></a> version bump</li>
<li><a href="https://github.com/typeorm/typeorm/commit/12e9db07b6b9676e63fff5f55a45b1d269716ed9"><code>12e9db0</code></a> feat: QueryBuilder performance optimizations (<a href="https://redirect.github.com/typeorm/typeorm/issues/9914">#9914</a>)</li>
<li><a href="https://github.com/typeorm/typeorm/commit/f1330ad6e23bea65a16b4f1c4199f10f3fa7282b"><code>f1330ad</code></a> fix: firstCapital=true not working in camelCase() function</li>
<li><a href="https://github.com/typeorm/typeorm/commit/a11809e1b20cc77fd2767b8bab2500a0c7e20d23"><code>a11809e</code></a> fix: handles &quot;query&quot; relation loading strategy for TreeRepositories (<a href="https://redirect.github.com/typeorm/typeorm/issues/9680">#9680</a>)</li>
<li><a href="https://github.com/typeorm/typeorm/commit/947ffc34324c1d692496804e43dafa6302efc1db"><code>947ffc3</code></a> feat: leftJoinAndMapOne and innerJoinAndMapOne map result to entity (<a href="https://redirect.github.com/typeorm/typeorm/issues/9354">#9354</a>)</li>
<li><a href="https://github.com/typeorm/typeorm/commit/de1228deace974eca3e9dd3956208ebe4cd9347f"><code>de1228d</code></a> fix: transform values for FindOperators <a href="https://redirect.github.com/typeorm/typeorm/issues/9381">#9381</a> (<a href="https://redirect.github.com/typeorm/typeorm/issues/9777">#9777</a>)</li>
<li><a href="https://github.com/typeorm/typeorm/commit/197cc05e90c0182357d85aa1ce7ae45de99d9d98"><code>197cc05</code></a> fix: prevent foreign key support during migration batch under sqlite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9775">#9775</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/typeorm/typeorm/compare/0.3.8...0.3.14">compare view</a></li>
</ul>
</details>
<br />


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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-11 22:18:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/92" class=".btn">#92</a>
            </td>
            <td>
                <b>
                    Bump xml2js and typeorm in /explorer/backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Removes [xml2js](https://github.com/Leonidas-from-XIV/node-xml2js). It's no longer used after updating ancestor dependency [typeorm](https://github.com/typeorm/typeorm). These dependencies need to be updated together.

Removes `xml2js`

Updates `typeorm` from 0.3.9 to 0.3.14
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/typeorm/typeorm/releases">typeorm's releases</a>.</em></p>
<blockquote>
<h2>0.3.14</h2>
<h3>Bug Fixes</h3>
<ul>
<li>drop xml &amp; yml connection option support. Addresses security issues in underlying dependency (<a href="https://redirect.github.com/typeorm/typeorm/issues/9930">#9930</a>) (<a href="https://github.com/typeorm/typeorm/commit/7dac12c2b18be34fb63ebfde988eb0825ec21384">7dac12c</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>QueryBuilder performance optimizations (<a href="https://redirect.github.com/typeorm/typeorm/issues/9914">#9914</a>) (<a href="https://github.com/typeorm/typeorm/commit/12e9db07b6b9676e63fff5f55a45b1d269716ed9">12e9db0</a>)</li>
</ul>
<h2>0.3.13</h2>
<h3>Bug Fixes</h3>
<ul>
<li>firstCapital=true not working in camelCase() function (<a href="https://github.com/typeorm/typeorm/commit/f1330ad6e23bea65a16b4f1c4199f10f3fa7282b">f1330ad</a>)</li>
<li>handles &quot;query&quot; relation loading strategy for TreeRepositories (<a href="https://redirect.github.com/typeorm/typeorm/issues/9680">#9680</a>) (<a href="https://github.com/typeorm/typeorm/commit/a11809e1b20cc77fd2767b8bab2500a0c7e20d23">a11809e</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9673">#9673</a></li>
<li>improve EntityNotFound error message in QueryBuilder.findOneOrFail (<a href="https://redirect.github.com/typeorm/typeorm/issues/9872">#9872</a>) (<a href="https://github.com/typeorm/typeorm/commit/f7f68178640120d8c1e92b8c9be0eeaa8262b4f3">f7f6817</a>)</li>
<li>loading tables with fk in sqlite query runner (<a href="https://redirect.github.com/typeorm/typeorm/issues/9875">#9875</a>) (<a href="https://github.com/typeorm/typeorm/commit/4997da054b5cfafdbdf374b3e554e5c4e0590da7">4997da0</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9266">#9266</a></li>
<li>prevent foreign key support during migration batch under sqlite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9775">#9775</a>) (<a href="https://github.com/typeorm/typeorm/commit/197cc05e90c0182357d85aa1ce7ae45de99d9d98">197cc05</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9770">#9770</a></li>
<li>proper default value on generating migration when default value is a function calling [Postgres] (<a href="https://redirect.github.com/typeorm/typeorm/issues/9830">#9830</a>) (<a href="https://github.com/typeorm/typeorm/commit/bebba05388a40a9f278a450d4a988865c158abb7">bebba05</a>)</li>
<li>react-native doesn't properly work in ESM projects because of circular dependency (<a href="https://redirect.github.com/typeorm/typeorm/issues/9765">#9765</a>) (<a href="https://github.com/typeorm/typeorm/commit/099fcd9b104bc930faea08f97ee3d5610118e0c4">099fcd9</a>)</li>
<li>resolve issues for mssql migration when simple-enum was changed (<a href="https://github.com/typeorm/typeorm/commit/cb154d4ca36cda251fcb9eb05a29b7758ae813cf">cb154d4</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/7785">#7785</a> <a href="https://redirect.github.com/typeorm/typeorm/issues/9457">#9457</a> <a href="https://redirect.github.com/typeorm/typeorm/issues/7785">#7785</a> <a href="https://redirect.github.com/typeorm/typeorm/issues/9457">#9457</a></li>
<li>resolves issue with mssql column recreation (<a href="https://redirect.github.com/typeorm/typeorm/issues/9773">#9773</a>) (<a href="https://github.com/typeorm/typeorm/commit/07221a364682b567533c93130efb4f5189e009a9">07221a3</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9399">#9399</a></li>
<li>transform values for FindOperators <a href="https://redirect.github.com/typeorm/typeorm/issues/9381">#9381</a> (<a href="https://redirect.github.com/typeorm/typeorm/issues/9777">#9777</a>) (<a href="https://github.com/typeorm/typeorm/commit/de1228deace974eca3e9dd3956208ebe4cd9347f">de1228d</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9816">#9816</a></li>
<li>use forward slashes when normalizing path (<a href="https://redirect.github.com/typeorm/typeorm/issues/9768">#9768</a>) (<a href="https://github.com/typeorm/typeorm/commit/58fc08840a4a64ca1935391f4709a784c3f0b373">58fc088</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9766">#9766</a></li>
<li>use object create if entity skip constructor is set (<a href="https://redirect.github.com/typeorm/typeorm/issues/9831">#9831</a>) (<a href="https://github.com/typeorm/typeorm/commit/a8689795dad796338e2a291a6a2fda89b00ef243">a868979</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>add support for json datatype for sqlite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9744">#9744</a>) (<a href="https://github.com/typeorm/typeorm/commit/4ac8c00117417ae622368aabe36d0fd5c676bd00">4ac8c00</a>)</li>
<li>add support for STI on EntitySchema (<a href="https://redirect.github.com/typeorm/typeorm/issues/9834">#9834</a>) (<a href="https://github.com/typeorm/typeorm/commit/bc306fb5a2c4dc02d04632af2b2f6c697a684356">bc306fb</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9833">#9833</a></li>
<li>allow type FindOptionsOrderValue for order by object property (<a href="https://redirect.github.com/typeorm/typeorm/issues/9895">#9895</a>) (<a href="https://redirect.github.com/typeorm/typeorm/issues/9896">#9896</a>) (<a href="https://github.com/typeorm/typeorm/commit/0814970a9cc2c958199c9d74d1ef313de43dab50">0814970</a>)</li>
<li>Broadcast identifier for removed related entities  (<a href="https://redirect.github.com/typeorm/typeorm/issues/9913">#9913</a>) (<a href="https://github.com/typeorm/typeorm/commit/f530811b0da2863711db3467e55bf815c66b4b4b">f530811</a>)</li>
<li>leftJoinAndMapOne and innerJoinAndMapOne map result to entity (<a href="https://redirect.github.com/typeorm/typeorm/issues/9354">#9354</a>) (<a href="https://github.com/typeorm/typeorm/commit/947ffc34324c1d692496804e43dafa6302efc1db">947ffc3</a>)</li>
</ul>
<h2>0.3.12</h2>
<h3>Bug Fixes</h3>
<ul>
<li>allow to pass ObjectLiteral in mongo find where condition (<a href="https://redirect.github.com/typeorm/typeorm/issues/9632">#9632</a>) (<a href="https://github.com/typeorm/typeorm/commit/4eda5df8693d1a659ff5c3461124cf05619fdd72">4eda5df</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9518">#9518</a></li>
<li>DataSource.setOptions doesn't properly update the database in the drivers (<a href="https://redirect.github.com/typeorm/typeorm/issues/9635">#9635</a>) (<a href="https://github.com/typeorm/typeorm/commit/a95bed7c05d10eb4b508e225faa4cb3c7ea7944f">a95bed7</a>)</li>
<li>Fix grammar error in no migrations found log (<a href="https://redirect.github.com/typeorm/typeorm/issues/9754">#9754</a>) (<a href="https://github.com/typeorm/typeorm/commit/6fb212187fdf97c07c41aad20d4f5503dfd44215">6fb2121</a>)</li>
<li>improved <code>FindOptionsWhere</code> behavior with union types (<a href="https://redirect.github.com/typeorm/typeorm/issues/9607">#9607</a>) (<a href="https://github.com/typeorm/typeorm/commit/7726f5ad1ec0c826510202a0f2cbeea705547eee">7726f5a</a>)</li>
<li>Incorrect enum default value when table name contains dash character (<a href="https://redirect.github.com/typeorm/typeorm/issues/9685">#9685</a>) (<a href="https://github.com/typeorm/typeorm/commit/b3b0c118a40441b31ac18ee7ce0cea0696b701ab">b3b0c11</a>)</li>
<li>incorrect sorting of entities with multi-inheritances (<a href="https://redirect.github.com/typeorm/typeorm/issues/9406">#9406</a>) (<a href="https://github.com/typeorm/typeorm/commit/54ca9dd801a77e011c2faf056b9e12845ccde82b">54ca9dd</a>)</li>
<li>make sure &quot;require&quot; is defined in the environment (<a href="https://github.com/typeorm/typeorm/commit/1a9b9fbcd683b2a28acbd26e39ac98dc6b60f001">1a9b9fb</a>)</li>
<li>materialized hints support for cte (<a href="https://redirect.github.com/typeorm/typeorm/issues/9605">#9605</a>) (<a href="https://github.com/typeorm/typeorm/commit/67973b4726500fc835639ffc302e0b6b20093df4">67973b4</a>)</li>
<li>multiple select queries during db sync in sqlite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9639">#9639</a>) (<a href="https://github.com/typeorm/typeorm/commit/6c928a4aa002cf5db0733055c0a754e97e4b43b3">6c928a4</a>)</li>
<li>overriding caching settings when alwaysEnabled is true (<a href="https://redirect.github.com/typeorm/typeorm/issues/9731">#9731</a>) (<a href="https://github.com/typeorm/typeorm/commit/4df969ea6254f9f69c371a72d80e857ab7c1f62d">4df969e</a>)</li>
<li>redundant Unique constraint on primary join column in Postgres (<a href="https://redirect.github.com/typeorm/typeorm/issues/9677">#9677</a>) (<a href="https://github.com/typeorm/typeorm/commit/b8704f87d2e06c048dea3f0b408ab18738acf7d7">b8704f8</a>)</li>
<li>remove unnecessary .js extension in imports (<a href="https://redirect.github.com/typeorm/typeorm/issues/9713">#9713</a>) (<a href="https://github.com/typeorm/typeorm/commit/6b37e3818bd74541cadbd44e55c84df510e41e3a">6b37e38</a>)</li>
<li>resolve issue with &quot;simple-enum&quot; synchronization in SQLite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9716">#9716</a>) (<a href="https://github.com/typeorm/typeorm/commit/c77c43e2423201bdc2ede85ae921447570685585">c77c43e</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9715">#9715</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/typeorm/typeorm/blob/master/CHANGELOG.md">typeorm's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/typeorm/typeorm/compare/0.3.12...0.3.14">0.3.14</a> (2023-04-09)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>drop xml &amp; yml connection option support. Addresses security issues in underlying dependency (<a href="https://redirect.github.com/typeorm/typeorm/issues/9930">#9930</a>) (<a href="https://github.com/typeorm/typeorm/commit/7dac12c2b18be34fb63ebfde988eb0825ec21384">7dac12c</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>QueryBuilder performance optimizations (<a href="https://redirect.github.com/typeorm/typeorm/issues/9914">#9914</a>) (<a href="https://github.com/typeorm/typeorm/commit/12e9db07b6b9676e63fff5f55a45b1d269716ed9">12e9db0</a>)</li>
</ul>
<h2><a href="https://github.com/typeorm/typeorm/compare/0.3.12...0.3.13">0.3.13</a> (2023-04-06)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>firstCapital=true not working in camelCase() function (<a href="https://github.com/typeorm/typeorm/commit/f1330ad6e23bea65a16b4f1c4199f10f3fa7282b">f1330ad</a>)</li>
<li>handles &quot;query&quot; relation loading strategy for TreeRepositories (<a href="https://redirect.github.com/typeorm/typeorm/issues/9680">#9680</a>) (<a href="https://github.com/typeorm/typeorm/commit/a11809e1b20cc77fd2767b8bab2500a0c7e20d23">a11809e</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9673">#9673</a></li>
<li>improve EntityNotFound error message in QueryBuilder.findOneOrFail (<a href="https://redirect.github.com/typeorm/typeorm/issues/9872">#9872</a>) (<a href="https://github.com/typeorm/typeorm/commit/f7f68178640120d8c1e92b8c9be0eeaa8262b4f3">f7f6817</a>)</li>
<li>loading tables with fk in sqlite query runner (<a href="https://redirect.github.com/typeorm/typeorm/issues/9875">#9875</a>) (<a href="https://github.com/typeorm/typeorm/commit/4997da054b5cfafdbdf374b3e554e5c4e0590da7">4997da0</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9266">#9266</a></li>
<li>prevent foreign key support during migration batch under sqlite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9775">#9775</a>) (<a href="https://github.com/typeorm/typeorm/commit/197cc05e90c0182357d85aa1ce7ae45de99d9d98">197cc05</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9770">#9770</a></li>
<li>proper default value on generating migration when default value is a function calling [Postgres] (<a href="https://redirect.github.com/typeorm/typeorm/issues/9830">#9830</a>) (<a href="https://github.com/typeorm/typeorm/commit/bebba05388a40a9f278a450d4a988865c158abb7">bebba05</a>)</li>
<li>react-native doesn't properly work in ESM projects because of circular dependency (<a href="https://redirect.github.com/typeorm/typeorm/issues/9765">#9765</a>) (<a href="https://github.com/typeorm/typeorm/commit/099fcd9b104bc930faea08f97ee3d5610118e0c4">099fcd9</a>)</li>
<li>resolve issues for mssql migration when simple-enum was changed (<a href="https://github.com/typeorm/typeorm/commit/cb154d4ca36cda251fcb9eb05a29b7758ae813cf">cb154d4</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/7785">#7785</a> <a href="https://redirect.github.com/typeorm/typeorm/issues/9457">#9457</a> <a href="https://redirect.github.com/typeorm/typeorm/issues/7785">#7785</a> <a href="https://redirect.github.com/typeorm/typeorm/issues/9457">#9457</a></li>
<li>resolves issue with mssql column recreation (<a href="https://redirect.github.com/typeorm/typeorm/issues/9773">#9773</a>) (<a href="https://github.com/typeorm/typeorm/commit/07221a364682b567533c93130efb4f5189e009a9">07221a3</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9399">#9399</a></li>
<li>transform values for FindOperators <a href="https://redirect.github.com/typeorm/typeorm/issues/9381">#9381</a> (<a href="https://redirect.github.com/typeorm/typeorm/issues/9777">#9777</a>) (<a href="https://github.com/typeorm/typeorm/commit/de1228deace974eca3e9dd3956208ebe4cd9347f">de1228d</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9816">#9816</a></li>
<li>use forward slashes when normalizing path (<a href="https://redirect.github.com/typeorm/typeorm/issues/9768">#9768</a>) (<a href="https://github.com/typeorm/typeorm/commit/58fc08840a4a64ca1935391f4709a784c3f0b373">58fc088</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9766">#9766</a></li>
<li>use object create if entity skip constructor is set (<a href="https://redirect.github.com/typeorm/typeorm/issues/9831">#9831</a>) (<a href="https://github.com/typeorm/typeorm/commit/a8689795dad796338e2a291a6a2fda89b00ef243">a868979</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>add support for json datatype for sqlite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9744">#9744</a>) (<a href="https://github.com/typeorm/typeorm/commit/4ac8c00117417ae622368aabe36d0fd5c676bd00">4ac8c00</a>)</li>
<li>add support for STI on EntitySchema (<a href="https://redirect.github.com/typeorm/typeorm/issues/9834">#9834</a>) (<a href="https://github.com/typeorm/typeorm/commit/bc306fb5a2c4dc02d04632af2b2f6c697a684356">bc306fb</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9833">#9833</a></li>
<li>allow type FindOptionsOrderValue for order by object property (<a href="https://redirect.github.com/typeorm/typeorm/issues/9895">#9895</a>) (<a href="https://redirect.github.com/typeorm/typeorm/issues/9896">#9896</a>) (<a href="https://github.com/typeorm/typeorm/commit/0814970a9cc2c958199c9d74d1ef313de43dab50">0814970</a>)</li>
<li>Broadcast identifier for removed related entities  (<a href="https://redirect.github.com/typeorm/typeorm/issues/9913">#9913</a>) (<a href="https://github.com/typeorm/typeorm/commit/f530811b0da2863711db3467e55bf815c66b4b4b">f530811</a>)</li>
<li>leftJoinAndMapOne and innerJoinAndMapOne map result to entity (<a href="https://redirect.github.com/typeorm/typeorm/issues/9354">#9354</a>) (<a href="https://github.com/typeorm/typeorm/commit/947ffc34324c1d692496804e43dafa6302efc1db">947ffc3</a>)</li>
</ul>
<h2><a href="https://github.com/typeorm/typeorm/compare/0.3.11...0.3.12">0.3.12</a> (2023-02-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>allow to pass ObjectLiteral in mongo find where condition (<a href="https://redirect.github.com/typeorm/typeorm/issues/9632">#9632</a>) (<a href="https://github.com/typeorm/typeorm/commit/4eda5df8693d1a659ff5c3461124cf05619fdd72">4eda5df</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9518">#9518</a></li>
<li>DataSource.setOptions doesn't properly update the database in the drivers (<a href="https://redirect.github.com/typeorm/typeorm/issues/9635">#9635</a>) (<a href="https://github.com/typeorm/typeorm/commit/a95bed7c05d10eb4b508e225faa4cb3c7ea7944f">a95bed7</a>)</li>
<li>Fix grammar error in no migrations found log (<a href="https://redirect.github.com/typeorm/typeorm/issues/9754">#9754</a>) (<a href="https://github.com/typeorm/typeorm/commit/6fb212187fdf97c07c41aad20d4f5503dfd44215">6fb2121</a>)</li>
<li>improved <code>FindOptionsWhere</code> behavior with union types (<a href="https://redirect.github.com/typeorm/typeorm/issues/9607">#9607</a>) (<a href="https://github.com/typeorm/typeorm/commit/7726f5ad1ec0c826510202a0f2cbeea705547eee">7726f5a</a>)</li>
<li>Incorrect enum default value when table name contains dash character (<a href="https://redirect.github.com/typeorm/typeorm/issues/9685">#9685</a>) (<a href="https://github.com/typeorm/typeorm/commit/b3b0c118a40441b31ac18ee7ce0cea0696b701ab">b3b0c11</a>)</li>
<li>incorrect sorting of entities with multi-inheritances (<a href="https://redirect.github.com/typeorm/typeorm/issues/9406">#9406</a>) (<a href="https://github.com/typeorm/typeorm/commit/54ca9dd801a77e011c2faf056b9e12845ccde82b">54ca9dd</a>)</li>
<li>make sure &quot;require&quot; is defined in the environment (<a href="https://github.com/typeorm/typeorm/commit/1a9b9fbcd683b2a28acbd26e39ac98dc6b60f001">1a9b9fb</a>)</li>
<li>materialized hints support for cte (<a href="https://redirect.github.com/typeorm/typeorm/issues/9605">#9605</a>) (<a href="https://github.com/typeorm/typeorm/commit/67973b4726500fc835639ffc302e0b6b20093df4">67973b4</a>)</li>
<li>multiple select queries during db sync in sqlite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9639">#9639</a>) (<a href="https://github.com/typeorm/typeorm/commit/6c928a4aa002cf5db0733055c0a754e97e4b43b3">6c928a4</a>)</li>
<li>overriding caching settings when alwaysEnabled is true (<a href="https://redirect.github.com/typeorm/typeorm/issues/9731">#9731</a>) (<a href="https://github.com/typeorm/typeorm/commit/4df969ea6254f9f69c371a72d80e857ab7c1f62d">4df969e</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/typeorm/typeorm/commit/5e3c565dce843b2deeefa3327340a79e0fc54e66"><code>5e3c565</code></a> version bump</li>
<li><a href="https://github.com/typeorm/typeorm/commit/7dac12c2b18be34fb63ebfde988eb0825ec21384"><code>7dac12c</code></a> fix: drop xml &amp; yml connection option support (<a href="https://redirect.github.com/typeorm/typeorm/issues/9930">#9930</a>)</li>
<li><a href="https://github.com/typeorm/typeorm/commit/daf1b47a609cb5090b71e537668ee115a98b1dc9"><code>daf1b47</code></a> fix: wrong dependency version in init command</li>
<li><a href="https://github.com/typeorm/typeorm/commit/0194f179fee8f346bbf82325716df6935aebda5e"><code>0194f17</code></a> version bump</li>
<li><a href="https://github.com/typeorm/typeorm/commit/12e9db07b6b9676e63fff5f55a45b1d269716ed9"><code>12e9db0</code></a> feat: QueryBuilder performance optimizations (<a href="https://redirect.github.com/typeorm/typeorm/issues/9914">#9914</a>)</li>
<li><a href="https://github.com/typeorm/typeorm/commit/f1330ad6e23bea65a16b4f1c4199f10f3fa7282b"><code>f1330ad</code></a> fix: firstCapital=true not working in camelCase() function</li>
<li><a href="https://github.com/typeorm/typeorm/commit/a11809e1b20cc77fd2767b8bab2500a0c7e20d23"><code>a11809e</code></a> fix: handles &quot;query&quot; relation loading strategy for TreeRepositories (<a href="https://redirect.github.com/typeorm/typeorm/issues/9680">#9680</a>)</li>
<li><a href="https://github.com/typeorm/typeorm/commit/947ffc34324c1d692496804e43dafa6302efc1db"><code>947ffc3</code></a> feat: leftJoinAndMapOne and innerJoinAndMapOne map result to entity (<a href="https://redirect.github.com/typeorm/typeorm/issues/9354">#9354</a>)</li>
<li><a href="https://github.com/typeorm/typeorm/commit/de1228deace974eca3e9dd3956208ebe4cd9347f"><code>de1228d</code></a> fix: transform values for FindOperators <a href="https://redirect.github.com/typeorm/typeorm/issues/9381">#9381</a> (<a href="https://redirect.github.com/typeorm/typeorm/issues/9777">#9777</a>)</li>
<li><a href="https://github.com/typeorm/typeorm/commit/197cc05e90c0182357d85aa1ce7ae45de99d9d98"><code>197cc05</code></a> fix: prevent foreign key support during migration batch under sqlite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9775">#9775</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/typeorm/typeorm/compare/0.3.9...0.3.14">compare view</a></li>
</ul>
</details>
<br />


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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-11 22:17:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/karma-charity-platform/pull/91" class=".btn">#91</a>
            </td>
            <td>
                <b>
                    Bump xml2js, typeorm and aws-sdk in /platform/backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [xml2js](https://github.com/Leonidas-from-XIV/node-xml2js), [typeorm](https://github.com/typeorm/typeorm) and [aws-sdk](https://github.com/aws/aws-sdk-js). These dependencies needed to be updated together.
Updates `xml2js` from 0.4.19 to 0.5.0
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/Leonidas-from-XIV/node-xml2js/commit/9f730bb5001331b4398909db98c80220eb9577f7"><code>9f730bb</code></a> Update package.json with latest PR</li>
<li><a href="https://github.com/Leonidas-from-XIV/node-xml2js/commit/50a492aef9729b8b9b291c5cb2746ec7dc1369db"><code>50a492a</code></a> Merge pull request <a href="https://redirect.github.com/Leonidas-from-XIV/node-xml2js/issues/603">#603</a> from autopulated/master</li>
<li><a href="https://github.com/Leonidas-from-XIV/node-xml2js/commit/7bc3c5d74cf66429dfb804626f3099a17dea1691"><code>7bc3c5d</code></a> Merge pull request <a href="https://redirect.github.com/Leonidas-from-XIV/node-xml2js/issues/598">#598</a> from fnimick/master</li>
<li><a href="https://github.com/Leonidas-from-XIV/node-xml2js/commit/f412a128b6d68c93d0cea44289484e5102b557f4"><code>f412a12</code></a> Merge pull request <a href="https://redirect.github.com/Leonidas-from-XIV/node-xml2js/issues/635">#635</a> from wisesimpson/patch-1</li>
<li><a href="https://github.com/Leonidas-from-XIV/node-xml2js/commit/d318ce0ad8e44971d8334c21f91a68ebbdc80466"><code>d318ce0</code></a> Update README.md</li>
<li><a href="https://github.com/Leonidas-from-XIV/node-xml2js/commit/581b19a62d88f8a3c068b5a45f4542c2d6a495a5"><code>581b19a</code></a> use Object.create(null) to create all parsed objects (prevent prototype repla...</li>
<li><a href="https://github.com/Leonidas-from-XIV/node-xml2js/commit/a21295009e4cbc1f9847bdff0f9b933b5005e690"><code>a212950</code></a> Add documentation for <code>explicitCharkey</code> option</li>
<li><a href="https://github.com/Leonidas-from-XIV/node-xml2js/commit/1832e0b6b2de30a5e326d1cf21708cd32305a538"><code>1832e0b</code></a> Merge pull request <a href="https://redirect.github.com/Leonidas-from-XIV/node-xml2js/issues/512">#512</a> from economia/master</li>
<li><a href="https://github.com/Leonidas-from-XIV/node-xml2js/commit/198063c4d5e051e3c58349a05354b255ef8bd63c"><code>198063c</code></a> Merge pull request <a href="https://redirect.github.com/Leonidas-from-XIV/node-xml2js/issues/556">#556</a> from Omega-Ariston/fix-issue544</li>
<li><a href="https://github.com/Leonidas-from-XIV/node-xml2js/commit/0d717852434131746d4efe147eecfcc1ebb7f4a8"><code>0d71785</code></a> Merge pull request <a href="https://redirect.github.com/Leonidas-from-XIV/node-xml2js/issues/562">#562</a> from Omega-Ariston/addDocExample</li>
<li>Additional commits viewable in <a href="https://github.com/Leonidas-from-XIV/node-xml2js/compare/0.4.19...0.5.0">compare view</a></li>
</ul>
</details>
<br />

Updates `typeorm` from 0.3.7 to 0.3.14
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/typeorm/typeorm/releases">typeorm's releases</a>.</em></p>
<blockquote>
<h2>0.3.14</h2>
<h3>Bug Fixes</h3>
<ul>
<li>drop xml &amp; yml connection option support. Addresses security issues in underlying dependency (<a href="https://redirect.github.com/typeorm/typeorm/issues/9930">#9930</a>) (<a href="https://github.com/typeorm/typeorm/commit/7dac12c2b18be34fb63ebfde988eb0825ec21384">7dac12c</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>QueryBuilder performance optimizations (<a href="https://redirect.github.com/typeorm/typeorm/issues/9914">#9914</a>) (<a href="https://github.com/typeorm/typeorm/commit/12e9db07b6b9676e63fff5f55a45b1d269716ed9">12e9db0</a>)</li>
</ul>
<h2>0.3.13</h2>
<h3>Bug Fixes</h3>
<ul>
<li>firstCapital=true not working in camelCase() function (<a href="https://github.com/typeorm/typeorm/commit/f1330ad6e23bea65a16b4f1c4199f10f3fa7282b">f1330ad</a>)</li>
<li>handles &quot;query&quot; relation loading strategy for TreeRepositories (<a href="https://redirect.github.com/typeorm/typeorm/issues/9680">#9680</a>) (<a href="https://github.com/typeorm/typeorm/commit/a11809e1b20cc77fd2767b8bab2500a0c7e20d23">a11809e</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9673">#9673</a></li>
<li>improve EntityNotFound error message in QueryBuilder.findOneOrFail (<a href="https://redirect.github.com/typeorm/typeorm/issues/9872">#9872</a>) (<a href="https://github.com/typeorm/typeorm/commit/f7f68178640120d8c1e92b8c9be0eeaa8262b4f3">f7f6817</a>)</li>
<li>loading tables with fk in sqlite query runner (<a href="https://redirect.github.com/typeorm/typeorm/issues/9875">#9875</a>) (<a href="https://github.com/typeorm/typeorm/commit/4997da054b5cfafdbdf374b3e554e5c4e0590da7">4997da0</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9266">#9266</a></li>
<li>prevent foreign key support during migration batch under sqlite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9775">#9775</a>) (<a href="https://github.com/typeorm/typeorm/commit/197cc05e90c0182357d85aa1ce7ae45de99d9d98">197cc05</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9770">#9770</a></li>
<li>proper default value on generating migration when default value is a function calling [Postgres] (<a href="https://redirect.github.com/typeorm/typeorm/issues/9830">#9830</a>) (<a href="https://github.com/typeorm/typeorm/commit/bebba05388a40a9f278a450d4a988865c158abb7">bebba05</a>)</li>
<li>react-native doesn't properly work in ESM projects because of circular dependency (<a href="https://redirect.github.com/typeorm/typeorm/issues/9765">#9765</a>) (<a href="https://github.com/typeorm/typeorm/commit/099fcd9b104bc930faea08f97ee3d5610118e0c4">099fcd9</a>)</li>
<li>resolve issues for mssql migration when simple-enum was changed (<a href="https://github.com/typeorm/typeorm/commit/cb154d4ca36cda251fcb9eb05a29b7758ae813cf">cb154d4</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/7785">#7785</a> <a href="https://redirect.github.com/typeorm/typeorm/issues/9457">#9457</a> <a href="https://redirect.github.com/typeorm/typeorm/issues/7785">#7785</a> <a href="https://redirect.github.com/typeorm/typeorm/issues/9457">#9457</a></li>
<li>resolves issue with mssql column recreation (<a href="https://redirect.github.com/typeorm/typeorm/issues/9773">#9773</a>) (<a href="https://github.com/typeorm/typeorm/commit/07221a364682b567533c93130efb4f5189e009a9">07221a3</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9399">#9399</a></li>
<li>transform values for FindOperators <a href="https://redirect.github.com/typeorm/typeorm/issues/9381">#9381</a> (<a href="https://redirect.github.com/typeorm/typeorm/issues/9777">#9777</a>) (<a href="https://github.com/typeorm/typeorm/commit/de1228deace974eca3e9dd3956208ebe4cd9347f">de1228d</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9816">#9816</a></li>
<li>use forward slashes when normalizing path (<a href="https://redirect.github.com/typeorm/typeorm/issues/9768">#9768</a>) (<a href="https://github.com/typeorm/typeorm/commit/58fc08840a4a64ca1935391f4709a784c3f0b373">58fc088</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9766">#9766</a></li>
<li>use object create if entity skip constructor is set (<a href="https://redirect.github.com/typeorm/typeorm/issues/9831">#9831</a>) (<a href="https://github.com/typeorm/typeorm/commit/a8689795dad796338e2a291a6a2fda89b00ef243">a868979</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>add support for json datatype for sqlite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9744">#9744</a>) (<a href="https://github.com/typeorm/typeorm/commit/4ac8c00117417ae622368aabe36d0fd5c676bd00">4ac8c00</a>)</li>
<li>add support for STI on EntitySchema (<a href="https://redirect.github.com/typeorm/typeorm/issues/9834">#9834</a>) (<a href="https://github.com/typeorm/typeorm/commit/bc306fb5a2c4dc02d04632af2b2f6c697a684356">bc306fb</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9833">#9833</a></li>
<li>allow type FindOptionsOrderValue for order by object property (<a href="https://redirect.github.com/typeorm/typeorm/issues/9895">#9895</a>) (<a href="https://redirect.github.com/typeorm/typeorm/issues/9896">#9896</a>) (<a href="https://github.com/typeorm/typeorm/commit/0814970a9cc2c958199c9d74d1ef313de43dab50">0814970</a>)</li>
<li>Broadcast identifier for removed related entities  (<a href="https://redirect.github.com/typeorm/typeorm/issues/9913">#9913</a>) (<a href="https://github.com/typeorm/typeorm/commit/f530811b0da2863711db3467e55bf815c66b4b4b">f530811</a>)</li>
<li>leftJoinAndMapOne and innerJoinAndMapOne map result to entity (<a href="https://redirect.github.com/typeorm/typeorm/issues/9354">#9354</a>) (<a href="https://github.com/typeorm/typeorm/commit/947ffc34324c1d692496804e43dafa6302efc1db">947ffc3</a>)</li>
</ul>
<h2>0.3.12</h2>
<h3>Bug Fixes</h3>
<ul>
<li>allow to pass ObjectLiteral in mongo find where condition (<a href="https://redirect.github.com/typeorm/typeorm/issues/9632">#9632</a>) (<a href="https://github.com/typeorm/typeorm/commit/4eda5df8693d1a659ff5c3461124cf05619fdd72">4eda5df</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9518">#9518</a></li>
<li>DataSource.setOptions doesn't properly update the database in the drivers (<a href="https://redirect.github.com/typeorm/typeorm/issues/9635">#9635</a>) (<a href="https://github.com/typeorm/typeorm/commit/a95bed7c05d10eb4b508e225faa4cb3c7ea7944f">a95bed7</a>)</li>
<li>Fix grammar error in no migrations found log (<a href="https://redirect.github.com/typeorm/typeorm/issues/9754">#9754</a>) (<a href="https://github.com/typeorm/typeorm/commit/6fb212187fdf97c07c41aad20d4f5503dfd44215">6fb2121</a>)</li>
<li>improved <code>FindOptionsWhere</code> behavior with union types (<a href="https://redirect.github.com/typeorm/typeorm/issues/9607">#9607</a>) (<a href="https://github.com/typeorm/typeorm/commit/7726f5ad1ec0c826510202a0f2cbeea705547eee">7726f5a</a>)</li>
<li>Incorrect enum default value when table name contains dash character (<a href="https://redirect.github.com/typeorm/typeorm/issues/9685">#9685</a>) (<a href="https://github.com/typeorm/typeorm/commit/b3b0c118a40441b31ac18ee7ce0cea0696b701ab">b3b0c11</a>)</li>
<li>incorrect sorting of entities with multi-inheritances (<a href="https://redirect.github.com/typeorm/typeorm/issues/9406">#9406</a>) (<a href="https://github.com/typeorm/typeorm/commit/54ca9dd801a77e011c2faf056b9e12845ccde82b">54ca9dd</a>)</li>
<li>make sure &quot;require&quot; is defined in the environment (<a href="https://github.com/typeorm/typeorm/commit/1a9b9fbcd683b2a28acbd26e39ac98dc6b60f001">1a9b9fb</a>)</li>
<li>materialized hints support for cte (<a href="https://redirect.github.com/typeorm/typeorm/issues/9605">#9605</a>) (<a href="https://github.com/typeorm/typeorm/commit/67973b4726500fc835639ffc302e0b6b20093df4">67973b4</a>)</li>
<li>multiple select queries during db sync in sqlite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9639">#9639</a>) (<a href="https://github.com/typeorm/typeorm/commit/6c928a4aa002cf5db0733055c0a754e97e4b43b3">6c928a4</a>)</li>
<li>overriding caching settings when alwaysEnabled is true (<a href="https://redirect.github.com/typeorm/typeorm/issues/9731">#9731</a>) (<a href="https://github.com/typeorm/typeorm/commit/4df969ea6254f9f69c371a72d80e857ab7c1f62d">4df969e</a>)</li>
<li>redundant Unique constraint on primary join column in Postgres (<a href="https://redirect.github.com/typeorm/typeorm/issues/9677">#9677</a>) (<a href="https://github.com/typeorm/typeorm/commit/b8704f87d2e06c048dea3f0b408ab18738acf7d7">b8704f8</a>)</li>
<li>remove unnecessary .js extension in imports (<a href="https://redirect.github.com/typeorm/typeorm/issues/9713">#9713</a>) (<a href="https://github.com/typeorm/typeorm/commit/6b37e3818bd74541cadbd44e55c84df510e41e3a">6b37e38</a>)</li>
<li>resolve issue with &quot;simple-enum&quot; synchronization in SQLite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9716">#9716</a>) (<a href="https://github.com/typeorm/typeorm/commit/c77c43e2423201bdc2ede85ae921447570685585">c77c43e</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9715">#9715</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/typeorm/typeorm/blob/master/CHANGELOG.md">typeorm's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/typeorm/typeorm/compare/0.3.12...0.3.14">0.3.14</a> (2023-04-09)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>drop xml &amp; yml connection option support. Addresses security issues in underlying dependency (<a href="https://redirect.github.com/typeorm/typeorm/issues/9930">#9930</a>) (<a href="https://github.com/typeorm/typeorm/commit/7dac12c2b18be34fb63ebfde988eb0825ec21384">7dac12c</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>QueryBuilder performance optimizations (<a href="https://redirect.github.com/typeorm/typeorm/issues/9914">#9914</a>) (<a href="https://github.com/typeorm/typeorm/commit/12e9db07b6b9676e63fff5f55a45b1d269716ed9">12e9db0</a>)</li>
</ul>
<h2><a href="https://github.com/typeorm/typeorm/compare/0.3.12...0.3.13">0.3.13</a> (2023-04-06)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>firstCapital=true not working in camelCase() function (<a href="https://github.com/typeorm/typeorm/commit/f1330ad6e23bea65a16b4f1c4199f10f3fa7282b">f1330ad</a>)</li>
<li>handles &quot;query&quot; relation loading strategy for TreeRepositories (<a href="https://redirect.github.com/typeorm/typeorm/issues/9680">#9680</a>) (<a href="https://github.com/typeorm/typeorm/commit/a11809e1b20cc77fd2767b8bab2500a0c7e20d23">a11809e</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9673">#9673</a></li>
<li>improve EntityNotFound error message in QueryBuilder.findOneOrFail (<a href="https://redirect.github.com/typeorm/typeorm/issues/9872">#9872</a>) (<a href="https://github.com/typeorm/typeorm/commit/f7f68178640120d8c1e92b8c9be0eeaa8262b4f3">f7f6817</a>)</li>
<li>loading tables with fk in sqlite query runner (<a href="https://redirect.github.com/typeorm/typeorm/issues/9875">#9875</a>) (<a href="https://github.com/typeorm/typeorm/commit/4997da054b5cfafdbdf374b3e554e5c4e0590da7">4997da0</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9266">#9266</a></li>
<li>prevent foreign key support during migration batch under sqlite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9775">#9775</a>) (<a href="https://github.com/typeorm/typeorm/commit/197cc05e90c0182357d85aa1ce7ae45de99d9d98">197cc05</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9770">#9770</a></li>
<li>proper default value on generating migration when default value is a function calling [Postgres] (<a href="https://redirect.github.com/typeorm/typeorm/issues/9830">#9830</a>) (<a href="https://github.com/typeorm/typeorm/commit/bebba05388a40a9f278a450d4a988865c158abb7">bebba05</a>)</li>
<li>react-native doesn't properly work in ESM projects because of circular dependency (<a href="https://redirect.github.com/typeorm/typeorm/issues/9765">#9765</a>) (<a href="https://github.com/typeorm/typeorm/commit/099fcd9b104bc930faea08f97ee3d5610118e0c4">099fcd9</a>)</li>
<li>resolve issues for mssql migration when simple-enum was changed (<a href="https://github.com/typeorm/typeorm/commit/cb154d4ca36cda251fcb9eb05a29b7758ae813cf">cb154d4</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/7785">#7785</a> <a href="https://redirect.github.com/typeorm/typeorm/issues/9457">#9457</a> <a href="https://redirect.github.com/typeorm/typeorm/issues/7785">#7785</a> <a href="https://redirect.github.com/typeorm/typeorm/issues/9457">#9457</a></li>
<li>resolves issue with mssql column recreation (<a href="https://redirect.github.com/typeorm/typeorm/issues/9773">#9773</a>) (<a href="https://github.com/typeorm/typeorm/commit/07221a364682b567533c93130efb4f5189e009a9">07221a3</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9399">#9399</a></li>
<li>transform values for FindOperators <a href="https://redirect.github.com/typeorm/typeorm/issues/9381">#9381</a> (<a href="https://redirect.github.com/typeorm/typeorm/issues/9777">#9777</a>) (<a href="https://github.com/typeorm/typeorm/commit/de1228deace974eca3e9dd3956208ebe4cd9347f">de1228d</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9816">#9816</a></li>
<li>use forward slashes when normalizing path (<a href="https://redirect.github.com/typeorm/typeorm/issues/9768">#9768</a>) (<a href="https://github.com/typeorm/typeorm/commit/58fc08840a4a64ca1935391f4709a784c3f0b373">58fc088</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9766">#9766</a></li>
<li>use object create if entity skip constructor is set (<a href="https://redirect.github.com/typeorm/typeorm/issues/9831">#9831</a>) (<a href="https://github.com/typeorm/typeorm/commit/a8689795dad796338e2a291a6a2fda89b00ef243">a868979</a>)</li>
</ul>
<h3>Features</h3>
<ul>
<li>add support for json datatype for sqlite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9744">#9744</a>) (<a href="https://github.com/typeorm/typeorm/commit/4ac8c00117417ae622368aabe36d0fd5c676bd00">4ac8c00</a>)</li>
<li>add support for STI on EntitySchema (<a href="https://redirect.github.com/typeorm/typeorm/issues/9834">#9834</a>) (<a href="https://github.com/typeorm/typeorm/commit/bc306fb5a2c4dc02d04632af2b2f6c697a684356">bc306fb</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9833">#9833</a></li>
<li>allow type FindOptionsOrderValue for order by object property (<a href="https://redirect.github.com/typeorm/typeorm/issues/9895">#9895</a>) (<a href="https://redirect.github.com/typeorm/typeorm/issues/9896">#9896</a>) (<a href="https://github.com/typeorm/typeorm/commit/0814970a9cc2c958199c9d74d1ef313de43dab50">0814970</a>)</li>
<li>Broadcast identifier for removed related entities  (<a href="https://redirect.github.com/typeorm/typeorm/issues/9913">#9913</a>) (<a href="https://github.com/typeorm/typeorm/commit/f530811b0da2863711db3467e55bf815c66b4b4b">f530811</a>)</li>
<li>leftJoinAndMapOne and innerJoinAndMapOne map result to entity (<a href="https://redirect.github.com/typeorm/typeorm/issues/9354">#9354</a>) (<a href="https://github.com/typeorm/typeorm/commit/947ffc34324c1d692496804e43dafa6302efc1db">947ffc3</a>)</li>
</ul>
<h2><a href="https://github.com/typeorm/typeorm/compare/0.3.11...0.3.12">0.3.12</a> (2023-02-07)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>allow to pass ObjectLiteral in mongo find where condition (<a href="https://redirect.github.com/typeorm/typeorm/issues/9632">#9632</a>) (<a href="https://github.com/typeorm/typeorm/commit/4eda5df8693d1a659ff5c3461124cf05619fdd72">4eda5df</a>), closes <a href="https://redirect.github.com/typeorm/typeorm/issues/9518">#9518</a></li>
<li>DataSource.setOptions doesn't properly update the database in the drivers (<a href="https://redirect.github.com/typeorm/typeorm/issues/9635">#9635</a>) (<a href="https://github.com/typeorm/typeorm/commit/a95bed7c05d10eb4b508e225faa4cb3c7ea7944f">a95bed7</a>)</li>
<li>Fix grammar error in no migrations found log (<a href="https://redirect.github.com/typeorm/typeorm/issues/9754">#9754</a>) (<a href="https://github.com/typeorm/typeorm/commit/6fb212187fdf97c07c41aad20d4f5503dfd44215">6fb2121</a>)</li>
<li>improved <code>FindOptionsWhere</code> behavior with union types (<a href="https://redirect.github.com/typeorm/typeorm/issues/9607">#9607</a>) (<a href="https://github.com/typeorm/typeorm/commit/7726f5ad1ec0c826510202a0f2cbeea705547eee">7726f5a</a>)</li>
<li>Incorrect enum default value when table name contains dash character (<a href="https://redirect.github.com/typeorm/typeorm/issues/9685">#9685</a>) (<a href="https://github.com/typeorm/typeorm/commit/b3b0c118a40441b31ac18ee7ce0cea0696b701ab">b3b0c11</a>)</li>
<li>incorrect sorting of entities with multi-inheritances (<a href="https://redirect.github.com/typeorm/typeorm/issues/9406">#9406</a>) (<a href="https://github.com/typeorm/typeorm/commit/54ca9dd801a77e011c2faf056b9e12845ccde82b">54ca9dd</a>)</li>
<li>make sure &quot;require&quot; is defined in the environment (<a href="https://github.com/typeorm/typeorm/commit/1a9b9fbcd683b2a28acbd26e39ac98dc6b60f001">1a9b9fb</a>)</li>
<li>materialized hints support for cte (<a href="https://redirect.github.com/typeorm/typeorm/issues/9605">#9605</a>) (<a href="https://github.com/typeorm/typeorm/commit/67973b4726500fc835639ffc302e0b6b20093df4">67973b4</a>)</li>
<li>multiple select queries during db sync in sqlite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9639">#9639</a>) (<a href="https://github.com/typeorm/typeorm/commit/6c928a4aa002cf5db0733055c0a754e97e4b43b3">6c928a4</a>)</li>
<li>overriding caching settings when alwaysEnabled is true (<a href="https://redirect.github.com/typeorm/typeorm/issues/9731">#9731</a>) (<a href="https://github.com/typeorm/typeorm/commit/4df969ea6254f9f69c371a72d80e857ab7c1f62d">4df969e</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/typeorm/typeorm/commit/5e3c565dce843b2deeefa3327340a79e0fc54e66"><code>5e3c565</code></a> version bump</li>
<li><a href="https://github.com/typeorm/typeorm/commit/7dac12c2b18be34fb63ebfde988eb0825ec21384"><code>7dac12c</code></a> fix: drop xml &amp; yml connection option support (<a href="https://redirect.github.com/typeorm/typeorm/issues/9930">#9930</a>)</li>
<li><a href="https://github.com/typeorm/typeorm/commit/daf1b47a609cb5090b71e537668ee115a98b1dc9"><code>daf1b47</code></a> fix: wrong dependency version in init command</li>
<li><a href="https://github.com/typeorm/typeorm/commit/0194f179fee8f346bbf82325716df6935aebda5e"><code>0194f17</code></a> version bump</li>
<li><a href="https://github.com/typeorm/typeorm/commit/12e9db07b6b9676e63fff5f55a45b1d269716ed9"><code>12e9db0</code></a> feat: QueryBuilder performance optimizations (<a href="https://redirect.github.com/typeorm/typeorm/issues/9914">#9914</a>)</li>
<li><a href="https://github.com/typeorm/typeorm/commit/f1330ad6e23bea65a16b4f1c4199f10f3fa7282b"><code>f1330ad</code></a> fix: firstCapital=true not working in camelCase() function</li>
<li><a href="https://github.com/typeorm/typeorm/commit/a11809e1b20cc77fd2767b8bab2500a0c7e20d23"><code>a11809e</code></a> fix: handles &quot;query&quot; relation loading strategy for TreeRepositories (<a href="https://redirect.github.com/typeorm/typeorm/issues/9680">#9680</a>)</li>
<li><a href="https://github.com/typeorm/typeorm/commit/947ffc34324c1d692496804e43dafa6302efc1db"><code>947ffc3</code></a> feat: leftJoinAndMapOne and innerJoinAndMapOne map result to entity (<a href="https://redirect.github.com/typeorm/typeorm/issues/9354">#9354</a>)</li>
<li><a href="https://github.com/typeorm/typeorm/commit/de1228deace974eca3e9dd3956208ebe4cd9347f"><code>de1228d</code></a> fix: transform values for FindOperators <a href="https://redirect.github.com/typeorm/typeorm/issues/9381">#9381</a> (<a href="https://redirect.github.com/typeorm/typeorm/issues/9777">#9777</a>)</li>
<li><a href="https://github.com/typeorm/typeorm/commit/197cc05e90c0182357d85aa1ce7ae45de99d9d98"><code>197cc05</code></a> fix: prevent foreign key support during migration batch under sqlite (<a href="https://redirect.github.com/typeorm/typeorm/issues/9775">#9775</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/typeorm/typeorm/compare/0.3.7...0.3.14">compare view</a></li>
</ul>
</details>
<br />

Updates `aws-sdk` from 2.1202.0 to 2.1354.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/aws/aws-sdk-js/releases">aws-sdk's releases</a>.</em></p>
<blockquote>
<h2>Release v2.1354.0</h2>
<p>See <a href="https://github.com/aws/aws-sdk-js/blob/master/CHANGELOG.md">changelog</a> for more information.</p>
<h2>Release v2.1353.0</h2>
<p>See <a href="https://github.com/aws/aws-sdk-js/blob/master/CHANGELOG.md">changelog</a> for more information.</p>
<h2>Release v2.1352.0</h2>
<p>See <a href="https://github.com/aws/aws-sdk-js/blob/master/CHANGELOG.md">changelog</a> for more information.</p>
<h2>Release v2.1351.0</h2>
<p>See <a href="https://github.com/aws/aws-sdk-js/blob/master/CHANGELOG.md">changelog</a> for more information.</p>
<h2>Release v2.1350.0</h2>
<p>See <a href="https://github.com/aws/aws-sdk-js/blob/master/CHANGELOG.md">changelog</a> for more information.</p>
<h2>Release v2.1349.0</h2>
<p>See <a href="https://github.com/aws/aws-sdk-js/blob/master/CHANGELOG.md">changelog</a> for more information.</p>
<h2>Release v2.1348.0</h2>
<p>See <a href="https://github.com/aws/aws-sdk-js/blob/master/CHANGELOG.md">changelog</a> for more information.</p>
<h2>Release v2.1347.0</h2>
<p>See <a href="https://github.com/aws/aws-sdk-js/blob/master/CHANGELOG.md">changelog</a> for more information.</p>
<h2>Release v2.1346.0</h2>
<p>See <a href="https://github.com/aws/aws-sdk-js/blob/master/CHANGELOG.md">changelog</a> for more information.</p>
<h2>Release v2.1345.0</h2>
<p>See <a href="https://github.com/aws/aws-sdk-js/blob/master/CHANGELOG.md">changelog</a> for more information.</p>
<h2>Release v2.1344.0</h2>
<p>See <a href="https://github.com/aws/aws-sdk-js/blob/master/CHANGELOG.md">changelog</a> for more information.</p>
<h2>Release v2.1343.0</h2>
<p>See <a href="https://github.com/aws/aws-sdk-js/blob/master/CHANGELOG.md">changelog</a> for more information.</p>
<h2>Release v2.1342.0</h2>
<p>See <a href="https://github.com/aws/aws-sdk-js/blob/master/CHANGELOG.md">changelog</a> for more information.</p>
<h2>Release v2.1341.0</h2>
<p>See <a href="https://github.com/aws/aws-sdk-js/blob/master/CHANGELOG.md">changelog</a> for more information.</p>
<h2>Release v2.1340.0</h2>
<p>See <a href="https://github.com/aws/aws-sdk-js/blob/master/CHANGELOG.md">changelog</a> for more information.</p>
<h2>Release v2.1339.0</h2>
<p>See <a href="https://github.com/aws/aws-sdk-js/blob/master/CHANGELOG.md">changelog</a> for more information.</p>
<h2>Release v2.1338.0</h2>
<p>See <a href="https://github.com/aws/aws-sdk-js/blob/master/CHANGELOG.md">changelog</a> for more information.</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/aws/aws-sdk-js/blob/master/CHANGELOG.md">aws-sdk's changelog</a>.</em></p>
<blockquote>
<h2>2.1354.0</h2>
<ul>
<li>feature: Connect: This release adds the ability to configure an agent's routing profile to receive contacts from multiple channels at the same time via extending the UpdateRoutingProfileConcurrency, CreateRoutingProfile and DescribeRoutingProfile APIs.</li>
<li>feature: ECS: This release adds support for enabling FIPS compliance on Amazon ECS Fargate tasks</li>
<li>feature: MarketplaceCatalog: Added three new APIs to support resource sharing: GetResourcePolicy, PutResourcePolicy, and DeleteResourcePolicy. Added new OwnershipType field to ListEntities request to let users filter on entities that are shared with them. Increased max page size of ListEntities response from 20 to 50 results.</li>
<li>feature: MediaConvert: AWS Elemental MediaConvert SDK now supports conversion of 608 paint-on captions to pop-on captions for SCC sources.</li>
<li>feature: Omics: Remove unexpected API changes.</li>
<li>feature: Rekognition: This release adds support for Face Liveness APIs in Amazon Rekognition. Updates UpdateStreamProcessor to return ResourceInUseException Exception. Minor updates to API documentation.</li>
</ul>
<h2>2.1353.0</h2>
<ul>
<li>feature: DLM: Updated timestamp format for GetLifecyclePolicy API</li>
<li>feature: DocDB: This release adds a new parameter 'DBClusterParameterGroupName' to 'RestoreDBClusterFromSnapshot' API to associate the name of the DB cluster parameter group while performing restore.</li>
<li>feature: Lambda: This release adds a new Lambda InvokeWithResponseStream API to support streaming Lambda function responses. The release also adds a new InvokeMode parameter to Function Url APIs to control whether the response will be streamed or buffered.</li>
<li>feature: QuickSight: This release has two changes: adding the OR condition to tag-based RLS rules in CreateDataSet and UpdateDataSet; adding RefreshSchedule and Incremental RefreshProperties operations for users to programmatically configure SPICE dataset ingestions.</li>
</ul>
<h2>2.1352.0</h2>
<ul>
<li>feature: CloudFormation: Including UPDATE_COMPLETE as a failed status for DeleteStack waiter.</li>
<li>feature: GreengrassV2: Add support for SUCCEEDED value in coreDeviceExecutionStatus field. Documentation updates for Greengrass V2.</li>
<li>feature: Proton: This release adds support for the AWS Proton service sync feature. Service sync enables managing an AWS Proton service (creating and updating instances) and all of it's corresponding service instances from a Git repository.</li>
</ul>
<h2>2.1351.0</h2>
<ul>
<li>feature: AppRunner: App Runner adds support for seven new vCPU and memory configurations.</li>
<li>feature: ConfigService: This release adds resourceType enums for types released in March 2023.</li>
<li>feature: IVSRealTime: Fix ParticipantToken ExpirationTime format</li>
<li>feature: NetworkFirewall: AWS Network Firewall now supports IPv6-only subnets.</li>
<li>feature: ServiceCatalog: removed incorrect product type value</li>
</ul>
<h2>2.1350.0</h2>
<ul>
<li>feature: AmplifyUIBuilder: Support StorageField and custom displays for data-bound options in form builder. Support non-string operands for predicates in collections. Support choosing client to get token from.</li>
<li>feature: DataExchange: This release updates the value of MaxResults.</li>
<li>feature: EC2: C6in, M6in, M6idn, R6in and R6idn bare metal instances are powered by 3rd Generation Intel Xeon Scalable processors and offer up to 200 Gbps of network bandwidth.</li>
<li>feature: ElasticInference: Updated public documentation for the Describe and Tagging APIs.</li>
<li>feature: SageMaker: Amazon SageMaker Asynchronous Inference now allows customer's to receive failure model responses in S3 and receive success/failure model responses in SNS notifications.</li>
<li>feature: SageMakerRuntime: Amazon SageMaker Asynchronous Inference now provides customers a FailureLocation as a response parameter in InvokeEndpointAsync API to capture the model failure responses.</li>
<li>feature: WAFV2: This release rolls back association config feature for webACLs that protect CloudFront protections.</li>
</ul>
<h2>2.1349.0</h2>
<ul>
<li>feature: Glue: Add support for database-level federation</li>
<li>feature: LakeFormation: Add support for database-level federation</li>
<li>feature: LicenseManager: This release adds grant override options to the CreateGrantVersion API. These options can be used to specify grant replacement behavior during grant activation.</li>
<li>feature: MWAA: This Amazon MWAA release adds the ability to customize the Apache Airflow environment by launching a shell script at startup. This shell script is hosted in your environment's Amazon S3 bucket. Amazon MWAA runs the script before installing requirements and initializing the Apache Airflow process.</li>
<li>feature: ServiceCatalog: This release introduces Service Catalog support for Terraform open source. It enables 1. The notify* APIs to Service Catalog. These APIs are used by the terraform engine to notify the result of the provisioning engine execution. 2. Adds a new TERRAFORM_OPEN_SOURCE product type in CreateProduct API.</li>
<li>feature: WAFV2: For web ACLs that protect CloudFront protections, the default request body inspection size is now 16 KB, and you can use the new association configuration to increase the inspection size further, up to 64 KB. Sizes over 16 KB can incur additional costs.</li>
</ul>
<h2>2.1348.0</h2>
<ul>
<li>feature: InternetMonitor: This release adds a new feature for Amazon CloudWatch Internet Monitor that enables customers to deliver internet measurements to Amazon S3 buckets as well as CloudWatch Logs.</li>
<li>feature: SMS: Deprecating AWS Server Migration Service.</li>
<li>feature: SageMakerFeatureStoreRuntime: In this release, you can now chose between soft delete and hard delete when calling the DeleteRecord API, so you have more flexibility when it comes to managing online store data.</li>
</ul>
<h2>2.1347.0</h2>
<ul>
<li>feature: Athena: Make DefaultExecutorDpuSize and CoordinatorDpuSize  fields optional  in StartSession</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/aws/aws-sdk-js/commit/a99fac57b17e20b7b33e5c9068c36dcb275fef1a"><code>a99fac5</code></a> Updates SDK to v2.1354.0</li>
<li><a href="https://github.com/aws/aws-sdk-js/commit/62847a45ae58deace88e58f75dfc09e0ae1c0b75"><code>62847a4</code></a> Bump xml2js to 0.5.0 (<a href="https://redirect.github.com/aws/aws-sdk-js/issues/4389">#4389</a>)</li>
<li><a href="https://github.com/aws/aws-sdk-js/commit/56ad952b39efbe26393af9dd80f168ff7ccd8cd6"><code>56ad952</code></a> Updates SDK to v2.1353.0</li>
<li><a href="https://github.com/aws/aws-sdk-js/commit/8a20e164cceeb1a09ddb3a3b1a6e581bcda518cf"><code>8a20e16</code></a> Updates SDK to v2.1352.0</li>
<li><a href="https://github.com/aws/aws-sdk-js/commit/d39ba59f8f62430e468e937ea0f937fb8ed102e6"><code>d39ba59</code></a> Updates SDK to v2.1351.0</li>
<li><a href="https://github.com/aws/aws-sdk-js/commit/3ee782cb76c328b1764be35edbec5c2eb8d81832"><code>3ee782c</code></a> Updates SDK to v2.1350.0</li>
<li><a href="https://github.com/aws/aws-sdk-js/commit/8dcb3e224e52ec6eb2bafed5bc88b58e31590972"><code>8dcb3e2</code></a> Updates SDK to v2.1349.0</li>
<li><a href="https://github.com/aws/aws-sdk-js/commit/cc11160e1cd5d8e0a3c9e9083b11f5787db4d657"><code>cc11160</code></a> Updates SDK to v2.1348.0</li>
<li><a href="https://github.com/aws/aws-sdk-js/commit/c58ec677ed65df69d0ce496c7a6adb694e2402fa"><code>c58ec67</code></a> Updates SDK to v2.1347.0</li>
<li><a href="https://github.com/aws/aws-sdk-js/commit/ded882e507caca815b0ae525c3c7489d1091cf73"><code>ded882e</code></a> Updates SDK to v2.1346.0</li>
<li>Additional commits viewable in <a href="https://github.com/aws/aws-sdk-js/compare/v2.1202.0...v2.1354.0">compare view</a></li>
</ul>
</details>
<br />


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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/karma-charity-platform/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-10 22:39:08 +0000 UTC
    </div>
</div>

