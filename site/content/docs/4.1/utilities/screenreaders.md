---
layout: docs
title: Screenreaders
description: Use screenreader utilities to hide elements on all devices except screen readers.
group: utilities
toc: true
---

Hide an element to all devices **except screen readers** with `.sr-only`. Combine `.sr-only` with `.sr-only-focusable` to show the element again when it's focused (e.g. by a keyboard-only user). Can also be used as mixins.

{{/*
Necessary for following [accessibility best practices]({{ .Site.BaseURL }}/docs/{{ .Site.Params.docs_version }}/getting-started/#accessibility).
*/}}

{{< example html >}}
<a class="sr-only sr-only-focusable" href="#content">Skip to main content</a>
{{< /example >}}

{{< highlight scss >}}
// Usage as a mixin
.skip-navigation {
  @include sr-only;
  @include sr-only-focusable;
}
{{< /highlight >}}
