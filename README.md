# Numbers API (numbers)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Numbers API by David Hu and Mack Duan — a free, community-contributed HTTP API for interesting facts about numbers. Returns trivia, math, date, and year facts as plain text or JSON. Supports random numbers, ranges/batches, JSONP callbacks, document.write embedding, sentence-fragment responses, and configurable not-found behavior.

**APIs.json:** [http://numbersapi.com/](http://numbersapi.com/)

## Tags

- Science And Math
- Public APIs
- Trivia
- Numbers
- Dates
- Open Source

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## APIs

### Numbers API

HTTP API for trivia, math, date, and year facts about numbers. URL pattern is `/{number}/{type}` where type is one of `trivia`, `math`, `date`, or `year`. Numbers may be integers, the keyword `random`, a `month/day` date, or batch ranges. Responses default to plain text and can be returned as JSON via the `json` query parameter.

- **Human URL:** [http://numbersapi.com/](http://numbersapi.com/)
- **Base URL:** `http://numbersapi.com/`

#### Tags

- Science And Math
- Trivia
- Numbers

#### Properties

- [Documentation](http://numbersapi.com/#api)
- [API Reference](http://numbersapi.com/#api)
- [Getting Started](http://numbersapi.com/#api)
- [OpenAPI](openapi/numbers-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/numbers.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/numbers.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/numbers-fact-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/numbers-batch-facts-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/numbers-fact-structure.json)
- [JSON Structure](json-structure/numbers-batch-facts-structure.json)
- [Example](examples/numbers-fact-example.json)
- [Example](examples/numbers-trivia-fact-example.json)
- [Example](examples/numbers-math-fact-example.json)
- [Example](examples/numbers-date-fact-example.json)
- [Example](examples/numbers-year-fact-example.json)
- [Example](examples/numbers-batch-facts-example.json)

## Common Properties

- [Website](http://numbersapi.com/)
- [Documentation](http://numbersapi.com/#api)
- [Blog](http://david-hu.com/2012/03/05/announcing-numbers-api.html)
- [Contact](mailto:numbersapi@gmail.com)
- [Public APIs Listing](https://github.com/public-apis/public-apis)
- [Spectral Rules](rules/numbers-rules.yml)
- [Vocabulary](vocabulary/numbers-vocabulary.yml)
- [JSON-LD](json-ld/numbers-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
