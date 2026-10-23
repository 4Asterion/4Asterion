### Small tools that check what a change really does before it ships.

I build dependency-free developer tools for safer releases. Each one answers a single question with evidence, and states plainly what it cannot prove.

<p align="center"><a href="https://github.com/4Asterion/beforepull"><img src="https://github.com/4Asterion/beforepull/raw/main/docs/demo.svg" alt="BeforePull terminal demo: a Docker socket mounted by a new sidecar is flagged as critical"></a></p>

| Project | What it answers | Stack |
|---|---|---|
| **[BeforePull](https://github.com/4Asterion/beforepull)** | *What does this Docker Compose update really change?* Privileged containers, Docker socket mounts, public ports, major upgrades and downgrades, before you pull. Also a GitHub Action for pull requests. | Go · single binary |
| **[EraseLoop](https://github.com/4Asterion/eraseloop)** | *Is deleted user data really gone, and does it stay gone?* Synthetic users, real deletion through your API, then repeated checks across PostgreSQL, Redis and S3. | Node.js · zero deps |

More in progress: configuration provenance, failing-run trace diffs and accessibility regression checks.

**How I build**

- No runtime dependencies unless they earn their place.
- Findings show the evidence; every README lists the tool's limits.
- CI on Linux, macOS and Windows; release binaries ship with SHA-256 checksums.

**Contact**: open an issue on the project. For security problems, use the repository's *Report a vulnerability* button.
