---
layout: default
title: Issue {{.Repository.Name}}
parent: {{.Organization.Name}}
grand_parent: Issues
has_children: false
permalink: /issues/{{.Organization.Github}}/{{.Repository.Name}}
---

# {{.Repository.Name}}

{{.Repository.About}}

[Goto GitHub]({{.Repository.Link}}){: .btn .btn-blue }

{{range .Issues}}
<div class="code-example" markdown="1">
| | {{.Title}} |
|:-----|:-----------|
| {{range .Labels}}{{.Name}}{: .label-grey }{{end}} | {{.Body}} |
[View on GitHub]({{.URL}}){: .btn }
</div>
{{end}}
