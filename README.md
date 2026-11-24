# exam-practice-papers

Full-length generated papers are organized under the canonical exam slug:

```text
exam-practice-papers/
  neet-ug/
  jee-main/
  jee-advanced/
  wbjee/
```

These output folder names use kebab-case even when the corresponding template IDs use underscores (for example, `neet_ug`).

## Resuming paper generation

Keep the `*_batch_generation.json` manifest, completed paper XML files, saved
`.response.txt` files, pending `_candidate.xml` files, and reference style
profiles in the hidden `.*_batch_generation` directory. They support resuming
completed or interrupted batches without losing work. Keep the original specs,
syllabi and reference inputs as well. Reference analysis artifacts under
`reference/` are retained to support resuming interrupted analysis.

Per-attempt directories inside `.*_batch_generation` contain regenerated
intermediate files and are ignored by Git. Ignoring them does not delete them
or reduce local disk usage; they can be useful for diagnosing failed attempts.