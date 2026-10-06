# conformance-oracle

**Public.** Workflows that run on GitHub's own hosted runners, so that bant's
conformance suite (the private `bant-conformance`) has GitHub's ground truth
to compare against. This repository contains test workflows and nothing else.

Every workflow here runs on `workflow_dispatch` only, reads no secret, and
refuses to upload output that contains a masked value or anything shaped like
a token: its artifacts are as public as the repository.
