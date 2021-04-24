---
layout: default
title: Release {{.Repository.Name}}
parent: {{.Organization.Name}}
grand_parent: Releases
has_children: false
permalink: /releases/{{.Organization.Github}}/{{.Repository.Name}}
---

# {{.Repository.Name}}

[Goto GitHub]({{.Repository.Link}}){: .btn .btn-blue }

{{range .Releases}}
<div class="code-example" markdown="1">
| | {{.Name}} |
|:-----|:-----------|
| {{.TagName}}{: .label-grey } | {{.Body}} |
[View on GitHub]({{.URL}}){: .btn }
</div>
{{end}}
