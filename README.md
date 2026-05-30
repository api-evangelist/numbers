# Numbers API (numbers)
Numbers API by David Hu and Mack Duan — a free, community-contributed HTTP API for interesting facts about numbers. Returns trivia, math, date, and year facts as plain text or JSON. Supports random numbers, ranges/batches, JSONP callbacks, document.write embedding, sentence-fragment responses, and configurable not-found behavior.

**URL:** [Visit APIs.json URL](http://numbersapi.com/)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Science And Math, Public APIs, Trivia, Numbers, Dates, Open Source

## Timestamps

- **Created:** 2026-05-28
- **Modified:** 2026-05-30

## APIs

### Numbers API
HTTP API for trivia, math, date, and year facts about numbers. URL pattern is `/{number}/{type}` where type is one of `trivia`, `math`, `date`, or `year`. Numbers may be integers, the keyword `random`, a `month/day` date, or batch ranges. Responses default to plain text and can be returned as JSON via the `json` query parameter.

**Human URL:** [http://numbersapi.com/](http://numbersapi.com/)

#### Tags:

 - Science And Math, Trivia, Numbers

#### Properties

- [Documentation](http://numbersapi.com/#api)
- [APIReference](http://numbersapi.com/#api)
- [GettingStarted](http://numbersapi.com/#api)
- [OpenAPI](openapi/numbers-openapi.yml)
- [JSONSchema — Fact](json-schema/numbers-fact-schema.json)
- [JSONSchema — BatchFacts](json-schema/numbers-batch-facts-schema.json)
- [JSONStructure — Fact](json-structure/numbers-fact-structure.json)
- [JSONStructure — BatchFacts](json-structure/numbers-batch-facts-structure.json)
- [Example — Fact](examples/numbers-fact-example.json)
- [Example — Trivia Fact](examples/numbers-trivia-fact-example.json)
- [Example — Math Fact](examples/numbers-math-fact-example.json)
- [Example — Date Fact](examples/numbers-date-fact-example.json)
- [Example — Year Fact](examples/numbers-year-fact-example.json)
- [Example — Batch Facts](examples/numbers-batch-facts-example.json)
- [NaftikoCapability — Trivia](capabilities/numbers-trivia.yaml)
- [NaftikoCapability — Math](capabilities/numbers-math.yaml)
- [NaftikoCapability — Date](capabilities/numbers-date.yaml)
- [NaftikoCapability — Year](capabilities/numbers-year.yaml)
- [NaftikoCapability — Batch](capabilities/numbers-batch.yaml)

## Common Properties

- [Website](http://numbersapi.com/)
- [Documentation](http://numbersapi.com/#api)
- [Blog](http://david-hu.com/2012/03/05/announcing-numbers-api.html)
- [Contact](mailto:numbersapi@gmail.com)
- [PublicAPIsListing](https://github.com/public-apis/public-apis)
- [SpectralRules](rules/numbers-rules.yml)
- [Vocabulary](vocabulary/numbers-vocabulary.yml)
- [JSONLD](json-ld/numbers-context.jsonld)

## Features

| Name | Description |
|------|-------------|
| Trivia Facts | Return a piece of trivia about a number, e.g. `42 is the number of little squares forming the left side trail of Microsoft's Windows 98 logo`. |
| Math Facts | Return a mathematical property of a number, e.g. `5 is the number of platonic solids`. |
| Date Facts | Return a fact about a day of the year (month/day), e.g. `February 29 is the day in 1504 that Christopher Columbus uses his knowledge of a lunar eclipse to convince Native Americans to provide him with supplies`. |
| Year Facts | Return a fact about a year, e.g. `1969 is the year that an estimated 500 million people worldwide watch Neil Armstrong take his historic first steps on the Moon`. |
| Random Numbers | Use the keyword `random` in place of a number to get a random fact, optionally bounded by `min` and `max` query parameters. |
| JSON Responses | Append `?json` (or send `Content-Type: application/json`) to receive the fact wrapped in an object with `text`, `found`, `number`, `type`, and optional `date`/`year` fields. |
| Sentence Fragment Mode | Append `?fragment` to get the fact rephrased as a lowercase, no-terminal-punctuation fragment suitable for embedding in a larger sentence. |
| Configurable Not Found Behavior | Use `notfound=default|floor|ceil` to control what happens when no fact exists for the requested number, with an optional custom `default=...` message. |
| JSONP Callback | Pass `callback=functionName` to wrap the response in a JSONP function call. |
| Document.write Embed | Pass `write` to wrap the response in `document.write(...)`, allowing a single `<script src="...">` to render the fact inline. |
| Batch Requests | Request facts for multiple numbers in one call using comma-separated values and `min..max` ranges (up to 100 numbers), returned as a JSON map. |
| CORS Support | Supports cross-origin requests, allowing direct browser calls from any domain. |

## Use Cases

| Name | Description |
|------|-------------|
| Engagement Copy | Insert living facts into marketing copy or dashboards, e.g. `We now have more users than the number of times Julius Caesar was stabbed`. |
| Calendar Widgets | Pair `month/day/date` with a date picker or daily widget to surface a historical fact for the current day. |
| Anniversary and Year-in-Review | Use `/{year}/year` to enrich anniversary, retrospective, and year-in-review content with curated facts. |
| Daily Random Trivia | Power "fact of the day" features for chatbots, newsletters, screen savers, and home assistants using `/random/trivia`. |
| Math Education | Surface mathematical properties of numbers in educational tools and worksheets via `/{n}/math`. |
| Mock and Demo Data | Provide free, unauthenticated, low-latency text responses ideal for tutorials, demos, and beginner HTTP client exercises. |

## Integrations

| Name | Description |
|------|-------------|
| jQuery | The docs show a `$.get()` example loading a trivia fact directly into a DOM element. |
| Browser JavaScript | Direct cross-origin requests via fetch/XHR are supported because the service emits permissive CORS headers. |
| JSONP Consumers | The `callback` query parameter lets legacy JSONP clients consume facts as `functionName("...")` invocations. |
| HTML script tag | The `write` query parameter wraps responses in `document.write()`, so a single `<script src="numbersapi.com/...">` tag can render a fact inline in static HTML. |
| Public APIs Directory | Listed in public-apis/public-apis under the Science & Math category as a free, no-auth API. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Numbers API](openapi/numbers-openapi.yml)

### JSON Schema

- [Fact](json-schema/numbers-fact-schema.json)
- [BatchFacts](json-schema/numbers-batch-facts-schema.json)

### JSON Structure

- [Fact](json-structure/numbers-fact-structure.json)
- [BatchFacts](json-structure/numbers-batch-facts-structure.json)

### JSON-LD

- [Numbers Context](json-ld/numbers-context.jsonld)

### Examples

- [Fact](examples/numbers-fact-example.json)
- [Trivia Fact](examples/numbers-trivia-fact-example.json)
- [Math Fact](examples/numbers-math-fact-example.json)
- [Date Fact](examples/numbers-date-fact-example.json)
- [Year Fact](examples/numbers-year-fact-example.json)
- [Batch Facts](examples/numbers-batch-facts-example.json)

## Capabilities

Naftiko capabilities organized as one self-contained file per business surface (OpenAPI tag), each with inline REST and MCP exposers.

### Numbers API

| Workflow | Operations | Tools | Persona |
|----------|-----------|-------|---------|
| [Numbers API — Trivia](capabilities/numbers-trivia.yaml) | 3 | 3 | Content Creator, Developer |
| [Numbers API — Math](capabilities/numbers-math.yaml) | 2 | 2 | Educator, Developer |
| [Numbers API — Date](capabilities/numbers-date.yaml) | 2 | 2 | Content Creator, Educator |
| [Numbers API — Year](capabilities/numbers-year.yaml) | 2 | 2 | Content Creator, Educator |
| [Numbers API — Batch](capabilities/numbers-batch.yaml) | 1 | 1 | Developer |

## Vocabulary

- [Numbers API Vocabulary](vocabulary/numbers-vocabulary.yml) — Unified taxonomy mapping 5 resources, 2 actions, 5 workflows, and 3 personas across operational (OpenAPI) and capability (Naftiko) dimensions

## Rules

- [Numbers API Rules](rules/numbers-rules.yml) — 30 rules across 12 categories enforcing Numbers API conventions (Title prefix, lowercase paths, camelCase operationIds, snake_case query params, GET-only methods, plain-text + JSON dual responses, no auth)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
