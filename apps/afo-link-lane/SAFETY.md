# Lab binding safety checklist

Before deploying this lab Worker, confirm:

- `wrangler.jsonc` has `name: afo-link-lane-v235-lab-2`.
- D1 binding points to `afo-link-lane-v235-lab-2-db`.
- R2 binding points to `afo-link-lane-v235-lab-2-content`.
- No production deploy workflow is present.
- No production D1/R2 IDs are reintroduced.
- The live production Worker `afo-link-lane` remains untouched.

Current lab resources:

- Worker target: `afo-link-lane-v235-lab-2`
- D1 database UUID: `c0253996-9e04-4a05-99b2-7fc6a3f0111c`
- R2 bucket: `afo-link-lane-v235-lab-2-content`
