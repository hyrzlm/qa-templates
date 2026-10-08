# Release checklist: <version or date>

Release owner: 
QA sign-off: 

## Before deploying

- [ ] Every ticket in the release has been tested on stage
- [ ] No open Critical or Major bugs against this release
- [ ] Known issues are written down and accepted by the product owner
- [ ] Regression suite passed on the release build (link the run)
- [ ] Database migrations reviewed and tested on a copy of production data
- [ ] New environment variables and feature flags are set in production
- [ ] Rollback plan agreed: who decides, and how

## Smoke test right after deploying

- [ ] App loads, no errors in the console
- [ ] Log in and log out
- [ ] The core flow works end to end (e.g. create → edit → delete)
- [ ] Each feature in this release, one happy path each
- [ ] Emails, webhooks and background jobs fire (check one of each)
- [ ] Third-party integrations still connect
- [ ] Error tracking and logs show no new spikes

## After release

- [ ] Release notes published
- [ ] Tickets moved to Done
- [ ] Monitoring checked again after 1 hour and the next morning
- [ ] Anything found during smoke test is logged as a bug
