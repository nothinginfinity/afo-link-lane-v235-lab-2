# AFO Link Lane v2.3.5 Lab 2

Second independent clone for AFO Link Lane v2.3.5 Command Center overlay and control deck work.

Clone-of-clone source:
- `nothinginfinity/afo-link-lane-v235-command-center-lab`
- source ref: `main`
- source commit: `b96b167ea2f5e329d9d8137ac1d9f4942526c955`

Original upstream source of lab 1:
- `nothinginfinity/repo-copilot`
- `apps/afo-link-lane/`
- original source commit: `274ffd35e4e37f3e1f90c868f0bc21e0b57d3c56`

Lab-2 isolation:
- Worker name: `afo-link-lane-v235-lab-2`
- D1 database: `afo-link-lane-v235-lab-2-db`
- D1 UUID: `c0253996-9e04-4a05-99b2-7fc6a3f0111c`
- R2 bucket: `afo-link-lane-v235-lab-2-content`

Safety rules:
- This repo is not the production `repo-copilot` app.
- This repo is also separate from the first lab repo.
- Do not bind this lab to the production `afo-link-lane` Worker.
- Do not bind this lab to the first lab Worker `afo-link-lane-v235-lab`.
- Do not bind this lab to production or lab-1 D1/R2 resources.
- Keep deploy workflows absent or lab-only until the UI path is verified.

Intended flow:
1. Use this repo for parallel experiments or throwaway UI/UX branches of the Command Center work.
2. Validate `worker.js` and embedded browser scripts before any deploy.
3. Deploy only to the lab-2 Worker.
4. Compare lab-2 vs lab-1 vs production when needed.
5. Port only verified patches back into the canonical repo using AFO gitZip Patcher.
