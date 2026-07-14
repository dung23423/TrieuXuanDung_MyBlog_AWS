---
title: "Week 8: File Upload API & Demo UI Support"
date: 2026-07-10
weight: 8
chapter: false
---

## Week 8: File Upload API & Supporting the Demo UI

### Daily log

| Day | Work done | Start date | Completion date | Reference |
| ---- | ---- | ---- | ---- | ---- |
| Mon | Built the API for uploading student avatar photos and ID card images, temporarily stored in the Backend's `wwwroot/uploads` folder. | 06/08/2026 | 06/08/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Tue | Added file-type validation (only `.jpg`/`.png` accepted), with a 5MB size limit. | 06/09/2026 | 06/09/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Wed | Generated filenames using GUIDs to avoid collisions/overwrites, finalized the upload API. | 06/10/2026 | 06/10/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Thu | Spent about half a day helping the team put together two very simple demo pages (a homepage and a rental request form) in plain HTML/CSS — not my main focus, kept as basic as possible. | 06/11/2026 | 06/11/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Fri | Tried calling the `/api/requests` API from the demo page using `fetch()` to confirm the submitted data matches what the backend expects. | 06/12/2026 | 06/12/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |
| Sat | Tested the upload API against various cases (valid format, invalid format, oversized file), confirming appropriate errors in each case. | 06/13/2026 | 06/14/2026 | [AWS Study Group Docs](https://cloudjourney.awsstudygroup.com/) |

### Outcomes
*   The file upload API works reliably.
*   The minimal demo UI was enough to test the request-submission flow end-to-end, and it surfaced a small bug in the backend's date-of-birth validation.
