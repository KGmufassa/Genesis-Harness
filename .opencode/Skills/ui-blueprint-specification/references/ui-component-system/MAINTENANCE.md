# UI Component System Maintenance

Normal Stage 4 runs must not edit this library.

Record candidate updates when:

- the same missing pattern appears across multiple products
- a template recommendation repeatedly produces poor page architecture
- an extension needs the same new page/component/state across multiple products
- two templates duplicate the same guidance
- a contradiction rule catches repeated failures
- a responsive rule repeatedly fails

Template gap record:

```json
{
  "gap": "",
  "affected_template_or_pattern": "",
  "project_context": "",
  "repeated_across_projects": false,
  "recommended_resolution": "",
  "evidence_refs": []
}
```

Maintenance workflow:

1. Review accumulated Stage 4 `template_gaps`.
2. Group repeated gaps by template, extension, pattern, or contradiction rule.
3. Update the smallest useful reference file.
4. Update `TEMPLATE-REGISTRY.md` or version notes when a template changes.
5. Keep changes structural; do not add visual design language or frontend code.

