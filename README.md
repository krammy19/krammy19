## Mark Noack
 
Technical writer. I build developer documentation and the automation that keeps
it accurate — code-sample validation, style enforcement, and content quality
checks that run in CI.
 
Currently senior technical writer at [Ocient](https://docs.ocient.com/), where I
maintain the public documentation and build the tooling behind it. Previously at
[Firebolt](https://docs.firebolt.io/). Before technical writing, a decade as a
newspaper reporter covering technology and local government.
 
### What's here
 
**[civic-engagement-app](https://github.com/krammy19/civic-engagement-app)** — a
content pipeline that ingests municipal meeting records from multiple government
platforms, extracts structured facts with Claude, and publishes plain-language
digests that can't go out until they pass an automated quality gate.
 
The part worth looking at is the measurement. Extraction is scored against a
hand-annotated gold set for precision, recall, hallucination rate, and confidence
calibration, with a CI gate that fails on regression. Every extracted value has to
cite a verbatim source span that gets checked back against the document, so
fabrications are caught deterministically rather than by asking another model. The
generated digests are checked against a style guide by a two-tier checker that is
itself scored for precision and recall.
 
Results, including where it does poorly and why, are in
[`docs/evals.md`](https://github.com/krammy19/civic-engagement-app/blob/main/docs/evals.md).
 
**[city-agenda-scraper](https://github.com/codeforsanjose/city-agenda-scraper)** —
earlier civic-data work with Code for America San José.
 
### Documentation I've built
 
[docs.ocient.com](https://docs.ocient.com/) ·
[docs.firebolt.io](https://docs.firebolt.io/) ·
[python-sdk.docs.firebolt.io](https://python-sdk.docs.firebolt.io/en/latest/)
