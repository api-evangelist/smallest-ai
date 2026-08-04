# Smallest AI (smallest-ai)

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

Smallest AI builds ultra-low-latency voice infrastructure - the Waves text-to-speech engine (Lightning / Lightning v2 models) for realtime speech synthesis and instant voice cloning, plus the Atoms platform for building and deploying production voice agents. The Waves REST API at https://waves-api.smallest.ai/api/v1 generates speech with sub-100ms latency, supports SSE and WebSocket streaming, and exposes voice listing and cloning via a Bearer-authenticated interface.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/smallest-ai/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/smallest-ai/refs/heads/main/apis.yml)

## Tags

- AI
- Text to Speech
- Voice
- Realtime
- Voice Agents

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Smallest AI Text-to-Speech (Waves)

Synthesizes natural speech from text with the Lightning family of models (sub-100ms latency, up to 44.1 kHz) via POST /lightning/get_speech, with configurable voice, sample rate, speed, and language.

- **Human URL:** [https://docs.smallest.ai/waves/api-reference](https://docs.smallest.ai/waves/api-reference)
- **Base URL:** `https://waves-api.smallest.ai/api/v1`

#### Tags

- Text to Speech
- Waves
- Lightning

#### Properties

- [Documentation](https://docs.smallest.ai/waves/documentation/getting-started/introduction)
- [API Reference](https://docs.smallest.ai/waves/api-reference)
- [OpenAPI](openapi/smallest-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/smallest-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/smallest-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Smallest AI Streaming / Realtime TTS

Realtime, low-latency text-to-speech delivered as base64 audio chunks over HTTP Server-Sent Events (POST /lightning-v2/get_speech/stream) and over a bidirectional WebSocket (wss://.../lightning-v2/get_speech/stream).

- **Human URL:** [https://docs.smallest.ai/waves/api-reference](https://docs.smallest.ai/waves/api-reference)
- **Base URL:** `https://waves-api.smallest.ai/api/v1`

#### Tags

- Streaming
- Realtime
- WebSocket
- SSE

#### Properties

- [Documentation](https://docs.smallest.ai/waves/documentation/text-to-speech-lightning/streaming)
- [OpenAPI](openapi/smallest-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [AsyncAPI](asyncapi/smallest-ai-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [Postman Collection](collections/smallest-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/smallest-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Smallest AI Voices / Cloning

Lists available prebuilt voices, clones a new voice from a short audio sample, lists cloned voices, and deletes cloned voices for use as voice_id values in synthesis requests.

- **Human URL:** [https://docs.smallest.ai/waves/api-reference](https://docs.smallest.ai/waves/api-reference)
- **Base URL:** `https://waves-api.smallest.ai/api/v1`

#### Tags

- Voices
- Voice Cloning
- Catalog

#### Properties

- [Documentation](https://docs.smallest.ai/waves/documentation/voice-cloning)
- [OpenAPI](openapi/smallest-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/smallest-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/smallest-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Smallest AI Atoms (Voice Agents)

The Atoms platform for building, testing, and deploying production voice agents - orchestrating Waves TTS and Pulse STT with LLM-driven conversation flows, exposed through a developer API and dashboard.

- **Human URL:** [https://atoms-docs.smallest.ai/](https://atoms-docs.smallest.ai/)
- **Base URL:** `https://atoms-api.smallest.ai`

#### Tags

- Voice Agents
- Atoms
- Conversational AI

#### Properties

- [Documentation](https://atoms-docs.smallest.ai/)

## Common Properties

- [GitHub Organization](https://github.com/smallest-inc)
- [LinkedIn](https://www.linkedin.com/company/smallest)
- [Website](https://smallest.ai/)
- [Documentation](https://docs.smallest.ai/)
- [Plans](plans/smallest-ai-plans-pricing.yml)
- [Rate Limits](rate-limits/smallest-ai-rate-limits.yml)
- [Fin Ops](finops/smallest-ai-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
