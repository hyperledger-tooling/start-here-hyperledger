---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/363" class=".btn">#363</a>
            </td>
            <td>
                <b>
                    build(deps): bump aws-sdk from 2.793.0 to 2.814.0 in /utility-emissions-channel/typescript_app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [aws-sdk](https://github.com/aws/aws-sdk-js) from 2.793.0 to 2.814.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/aws/aws-sdk-js/blob/master/CHANGELOG.md">aws-sdk's changelog</a>.</em></p>
<blockquote>
<h2>2.814.0</h2>
<ul>
<li>bugfix: Credentials: SDK will throw if shared ini file's profile name can be resolved to <strong>proto</strong></li>
<li>feature: EC2: EBS io2 volumes now supports Multi-Attach</li>
<li>feature: PersonalizeRuntime: Updated FilterValues regex pattern to align with Filter Expression.</li>
<li>feature: RDS: Adds IAM DB authentication information to the PendingModifiedValues output of the DescribeDBInstances API. Adds ClusterPendingModifiedValues information to the output of the DescribeDBClusters API.</li>
</ul>
<h2>2.813.0</h2>
<ul>
<li>feature: ConfigService: Adding PutExternalEvaluation API which grants permission to deliver evaluation result to AWS Config</li>
<li>feature: DLM: Provide Cross-account copy event based policy support in DataLifecycleManager (DLM)</li>
<li>feature: EC2: C6gn instances are powered by AWS Graviton2 processors and offer 100 Gbps networking bandwidth. These instances deliver up to 40% better price-performance benefit versus comparable x86-based instances</li>
<li>feature: Imagebuilder: This release adds support for building and distributing container images within EC2 Image Builder.</li>
<li>feature: KMS: Added CreationDate and LastUpdatedDate timestamps to ListAliases API response</li>
<li>feature: Route53: This release adds support for DNSSEC signing in Amazon Route 53.</li>
<li>feature: Route53Resolver: Route 53 Resolver adds support for enabling resolver DNSSEC validation in virtual private cloud (VPC).</li>
<li>feature: SQS: Amazon SQS adds queue attributes to enable high throughput FIFO.</li>
<li>feature: ServiceCatalog: Support TagOptions sharing with Service Catalog portfolio sharing.</li>
</ul>
<h2>2.812.0</h2>
<ul>
<li>feature: CostExplorer: This release updates the &quot;MonitorArnList&quot; from a list of String to be a list of Arn for both CreateAnomalySubscription and UpdateAnomalySubscription APIs</li>
<li>feature: Location: Initial release of Amazon Location Service. A new geospatial service providing capabilities to render maps, geocode/reverse geocode, track device locations, and detect geofence entry/exit events.</li>
<li>feature: QuickSight: QuickSight now supports connecting to federated data sources of Athena</li>
<li>feature: WellArchitected: This is the first release of AWS Well-Architected Tool API support, use to review your workload and compare against the latest AWS architectural best practices.</li>
</ul>
<h2>2.811.0</h2>
<ul>
<li>feature: Amp: (New Service) Amazon Managed Service for Prometheus is a fully managed Prometheus-compatible monitoring service that makes it easy to monitor containerized applications securely and at scale.</li>
<li>feature: GreengrassV2: AWS IoT Greengrass V2 is a new major version of AWS IoT Greengrass. This release adds several updates such as modular components, continuous deployments, and improved ease of use.</li>
<li>feature: IoTAnalytics: FileFormatConfiguration enables data store to save data in JSON or Parquet format. S3Paths enables you to specify the S3 objects that save your channel messages when you reprocess the pipeline.</li>
<li>feature: IoTFleetHub: AWS IoT Fleet Hub, a new feature of AWS IoT Device Management that provides a web application for monitoring and managing device fleets connected to AWS IoT at scale.</li>
<li>feature: IoTWireless: AWS IoT for LoRaWAN enables customers to setup a private LoRaWAN network by connecting their LoRaWAN devices and gateways to the AWS cloud without managing a LoRaWAN Network Server.</li>
<li>feature: Iot: AWS IoT Rules Engine adds Kafka Action that allows sending data to Apache Kafka clusters inside a VPC. AWS IoT Device Defender adds custom metrics and machine-learning based anomaly detection.</li>
<li>feature: IotDeviceAdvisor: AWS IoT Core Device Advisor is fully managed test capability for IoT devices. Device manufacturers can use Device Advisor to test their IoT devices for reliable and secure connectivity with AWS IoT.</li>
<li>feature: Lambda: Added support for Apache Kafka as a event source. Added support for TumblingWindowInSeconds for streams event source mappings. Added support for FunctionResponseTypes for streams event source mappings</li>
<li>feature: SSM: Adding support for Change Manager API content</li>
</ul>
<h2>2.810.0</h2>
<ul>
<li>feature: DevOpsGuru: Documentation updates for DevOps Guru.</li>
<li>feature: EC2: Add c5n.metal to ec2 instance types list</li>
<li>feature: GlobalAccelerator: This release adds support for custom routing accelerators</li>
</ul>
<h2>2.809.0</h2>
<ul>
<li>feature: AutoScaling: Documentation updates and corrections for Amazon EC2 Auto Scaling API Reference and SDKs.</li>
<li>feature: CloudTrail: CloudTrailInvalidClientTokenIdException is now thrown when a call results in the InvalidClientTokenId error code. The Name parameter of the AdvancedEventSelector data type is now optional.</li>
<li>feature: IoTSiteWise: Added the ListAssetRelationships operation and support for composite asset models, which represent structured sets of properties within asset models.</li>
</ul>
<h2>2.808.0</h2>
<ul>
<li>feature: EC2: TGW connect simplifies connectivity of SD-WAN appliances; IGMP support for TGW multicast; VPC Reachability Analyzer for VPC resources connectivity analysis.</li>
<li>feature: Kendra: Amazon Kendra now supports adding synonyms to an index through the new Thesaurus resource.</li>
<li>feature: NetworkManager: This release adds API support for Transit Gateway Connect integration into AWS Network Manager.</li>
</ul>
<h2>2.807.0</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/aws/aws-sdk-js/commit/8875a35871b738388398ed5667ffc7d6eb1aa36f"><code>8875a35</code></a> Updates SDK to v2.814.0</li>
<li><a href="https://github.com/aws/aws-sdk-js/commit/dd83d672170e8cc0c52a20df29a43e7663e5336a"><code>dd83d67</code></a> throw at invalid profile name in shared ini file (<a href="https://github-redirect.dependabot.com/aws/aws-sdk-js/issues/3585">#3585</a>)</li>
<li><a href="https://github.com/aws/aws-sdk-js/commit/ee0c5a314ae1048e2f371f61fe32aa3d88a523f6"><code>ee0c5a3</code></a> Updates SDK to v2.813.0</li>
<li><a href="https://github.com/aws/aws-sdk-js/commit/468d15b92d8af65804f53a9734837a3a1636fb77"><code>468d15b</code></a> Updates SDK to v2.812.0</li>
<li><a href="https://github.com/aws/aws-sdk-js/commit/c50132f3a1f366e871f658fd796291997fe32b4e"><code>c50132f</code></a> Update README.md with references to JS SDK V3 (<a href="https://github-redirect.dependabot.com/aws/aws-sdk-js/issues/3582">#3582</a>)</li>
<li><a href="https://github.com/aws/aws-sdk-js/commit/3e19b081cae3b123e55223c767e95c30f200271a"><code>3e19b08</code></a> Updates SDK to v2.811.0</li>
<li><a href="https://github.com/aws/aws-sdk-js/commit/f26c00dc76653a703e8021593d7e1baebc9d390b"><code>f26c00d</code></a> Updates SDK to v2.810.0</li>
<li><a href="https://github.com/aws/aws-sdk-js/commit/b393a6e1e7824855b9d7ab59ff3ca4f4425d933c"><code>b393a6e</code></a> Adds automatic PreSignedUrl generation to RDS.StartDBInstanceAutomatedBackups...</li>
<li><a href="https://github.com/aws/aws-sdk-js/commit/fa579670cffa3ee902ab3f4dddb9e6245489b86f"><code>fa57967</code></a> Updates SDK to v2.809.0</li>
<li><a href="https://github.com/aws/aws-sdk-js/commit/9a52018b7c74eb7925c4929f186dfd9401a472f0"><code>9a52018</code></a> Updates SDK to v2.808.0</li>
<li>Additional commits viewable in <a href="https://github.com/aws/aws-sdk-js/compare/v2.793.0...v2.814.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aws-sdk&package-manager=npm_and_yarn&previous-version=2.793.0&new-version=2.814.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-16 22:35:21 +0000 UTC
    </div>
</div>

