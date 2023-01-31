

---
title: "{{ .Name }}"
date: {{ .Date }}
draft: false
---

{{ if (index .Site.Data.externalPost .Name) }}
    {{- index .Site.Data.externalPost .Name "content" }}
{{end}}