# Smallest AI (smallest-ai)

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
