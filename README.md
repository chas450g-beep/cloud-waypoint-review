# Cloud Waypoint — review mirror

A **sanitized, read-only review mirror**. It exists so a reviewer can read the public surface and
the report set without access to the private repository. **No pull requests are accepted**; the
canonical source is the private repository `chas450g-beep/cloud-waypoint`, and this mirror is
regenerated from it on every deploy of the public site or the report explorer (source commit
`df52d231`).

- `site/` — the public site as served at https://cloud-waypoint.com/ : seven pages, the stylesheet,
  the marks, the robots file, the three-minute overview.
- `reports/natsec/`, `reports/pubsec/` — the fifteen standard deliverables printed in full from
  one complete **fictional** engagement record (USAF MC², invented end to end: every person, system,
  provider arrangement and figure), once per edition. NatSec reads against the DoD Cloud Computing
  SRG at IL5/IL6; PubSec against FedRAMP High and FISMA High; both on NIST SP 800-53. Each print is
  self-contained (styles inline, no script, nothing fetched).
- `REVIEW-MANIFEST.json` — every file with its role and SHA-256, the source commit, and the data
  boundary.

Nothing here takes evidence. No client material, credential, tenant, CUI, DoD/IC, interview,
transcript, mission, seller, studio or readiness data is present, by construction: the mirror is
assembled from an explicit include list and refuses to build if an excluded pattern appears.
