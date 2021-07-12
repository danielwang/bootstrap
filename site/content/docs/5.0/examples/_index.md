---
layout: single
title: Projects
description: One stop shop documentation for various projects.
aliases: "/examples/"
---

# Figma CAD 

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt.

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FGwcmnRFu2MmHaHfoyC7otD%2FCAD%3Fnode-id%3D0%253A1" allowfullscreen></iframe>

&nbsp;
&nbsp;
&nbsp;
&nbsp;
&nbsp;
&nbsp;

{{< list-examples.inline >}}
{{ range $entry := $.Site.Data.examples -}}
  <h1 id="{{ $entry.category | urlize }}">{{ $entry.category }}</h1>
  <p>{{ $entry.description }}</p>
  {{ if eq $entry.category "RTL" -}}
    <div class="bd-callout bd-callout-warning">
      <p>The RTL feature is still <strong>experimental</strong> and will probably evolve according to user feedback. Spotted something or have an improvement to suggest? <a href="{{ $.Site.Params.repo }}/issues/new">Open an issue</a>, we'd love to get your insights.</p>
    </div>
  {{ end -}}

  {{ range $i, $example := $entry.examples -}}
    {{- $len := len $entry.examples -}}
    {{ if (eq $i 0) }}<div class="row">{{ end }}
      <div class="col-sm-6 col-md-4 col-xl-3 mb-3">
        <a class="d-block" href="/docs/{{ $.Site.Params.docs_version }}/examples/{{ $example.name | urlize }}/"{{ if in $example.name "RTL" }} hreflang="ar"{{ end }}>
          <h3 class="mb-1 text-primary">{{ $example.name }}</h3>
        </a>
        <p class="text-muted">{{ $example.description }}</p>
      </div>
    {{ if (eq (add $i 1) $len) }}</div>{{ end }}
  {{ end -}}
{{ end -}}
{{< /list-examples.inline >}}
