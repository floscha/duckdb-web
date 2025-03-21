---
warning: DO NOT CHANGE THIS MANUALLY, THIS IS GENERATED BY https://github/duckdb/community-extensions repository, check README there
title: tarfs
excerpt: |
  DuckDB Community Extensions
  glob, open and read files within `.tar` archives

extension:
  name: tarfs
  description: glob, open and read files within `.tar` archives
  version: 1.0.0
  language: C++
  build: cmake
  license: MIT
  maintainers:
    - Maxxen

repo:
  github: Maxxen/duckdb_tarfs
  ref: 6d468b45f38f16d58e49032edd76aa76c2a2b078

docs:
  hello_world: |
    SELECT filename FROM read_blob('tar://data/csv/tar/ab.tar/*');
  extended_description: |
    This extension provides a duckdb file-system abstraction to read and glob files within __uncompressed__ tar archives.
    For more information and information regarding usage, limitations and performance, see the [tarfs README](https://github.com/Maxxen/duckdb_tarfs).

extension_star_count: 8
extension_star_count_pretty: 8
extension_download_count: 447
extension_download_count_pretty: 447
image: '/images/community_extensions/social_preview/preview_community_extension_tarfs.png'
layout: community_extension_doc
---

### Installing and Loading
```sql
INSTALL {{ page.extension.name }} FROM community;
LOAD {{ page.extension.name }};
```

{% if page.docs.hello_world %}
### Example
```sql
{{ page.docs.hello_world }}```
{% endif %}

{% if page.docs.extended_description %}
### About {{ page.extension.name }}
{{ page.docs.extended_description }}
{% endif %}


