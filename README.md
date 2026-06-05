# elevenlabs (elevenlabs)

Converts text into speech using a voice of your choice and returns audio.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/elevenlabs/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/elevenlabs/refs/heads/main/apis.yml)

## Timestamps

- **Modified:** 2026-05-19

## APIs

### ElevenLabs Text to Speech API

The ElevenLabs Text to Speech API converts text into lifelike spoken audio with nuanced intonation, pacing, and emotional awareness. It supports multiple output formats including MP3, PCM, and mu-law, and offers a range of models such as Flash v2.5 for ultra-low latency real-time applications and Multilingual v2 for support across 70+ languages. Developers can select from thousands of pre-built voices or use custom cloned voices to generate speech that sounds natural and expressive.

- **Human URL:** [https://elevenlabs.io/docs/api-reference/text-to-speech/convert](https://elevenlabs.io/docs/api-reference/text-to-speech/convert)
- **Base URL:** `https://api.elevenlabs.io`

#### Tags

- AI
- Audio
- Speech Synthesis
- Text to Speech
- Voice

#### Properties

- [Documentation](https://elevenlabs.io/docs/api-reference/text-to-speech/convert)
- [OpenAPI](openapi/elevenlabs-text-to-speech-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/elevenlabs-text-to-speech.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/elevenlabs-text-to-speech.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/elevenlabs-text-to-speech-streaming-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### ElevenLabs Speech to Text API

The ElevenLabs Speech to Text API provides state-of-the-art transcription capabilities, converting spoken audio into accurate text. It supports multiple audio formats and languages, enabling developers to build applications that require reliable audio transcription. The API is designed for both real-time and batch processing use cases.

- **Human URL:** [https://elevenlabs.io/docs/api-reference/speech-to-text/convert](https://elevenlabs.io/docs/api-reference/speech-to-text/convert)
- **Base URL:** `https://api.elevenlabs.io`

#### Tags

- AI
- Audio
- Speech to Text
- Transcription

#### Properties

- [Documentation](https://elevenlabs.io/docs/api-reference/speech-to-text/convert)
- [OpenAPI](openapi/elevenlabs-speech-to-text-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/elevenlabs-speech-to-text.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/elevenlabs-speech-to-text.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ElevenLabs Voice Cloning API

The ElevenLabs Voice Cloning API allows developers to create custom AI voices from audio recordings. Instant Voice Cloning requires as little as 60 seconds of clean audio to generate a usable voice clone, while Professional Voice Cloning produces higher fidelity results from a minimum of 30 minutes of recordings. Cloned voices can then be used with the Text to Speech API for generating speech that closely matches the original speaker.

- **Human URL:** [https://elevenlabs.io/docs/api-reference/voices/ivc/create](https://elevenlabs.io/docs/api-reference/voices/ivc/create)
- **Base URL:** `https://api.elevenlabs.io`

#### Tags

- AI
- Audio
- Voice
- Voice Cloning

#### Properties

- [Documentation](https://elevenlabs.io/docs/api-reference/voices/ivc/create)
- [OpenAPI](openapi/elevenlabs-voice-cloning-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/elevenlabs-voice-cloning.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/elevenlabs-voice-cloning.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ElevenLabs Voices API

The ElevenLabs Voices API provides management capabilities for the voice library, including listing, retrieving, creating, editing, and deleting voices. Developers can access a library of over 5,000 pre-built voices and manage their own custom voices. The API also supports voice design, allowing creation of new AI voices from text descriptions specifying desired characteristics such as accent, age, and tone.

- **Human URL:** [https://elevenlabs.io/docs/api-reference/voices/get](https://elevenlabs.io/docs/api-reference/voices/get)
- **Base URL:** `https://api.elevenlabs.io`

#### Tags

- AI
- Voice Library
- Voice Management
- Voices

#### Properties

- [Documentation](https://elevenlabs.io/docs/api-reference/voices/get)
- [OpenAPI](openapi/elevenlabs-voices-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/elevenlabs-voices.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/elevenlabs-voices.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ElevenLabs Sound Effects API

The ElevenLabs Sound Effects API generates cinematic sound effects from text descriptions. Developers can describe the desired sound in natural language and receive high-quality audio output. The API supports audio tags for controlling delivery, emotion, emphasis, pauses, and specific sound effects, making it suitable for game development, film production, and multimedia content creation.

- **Human URL:** [https://elevenlabs.io/docs/api-reference/sound-generation/create](https://elevenlabs.io/docs/api-reference/sound-generation/create)
- **Base URL:** `https://api.elevenlabs.io`

#### Tags

- AI
- Audio Generation
- Sound Effects

#### Properties

- [Documentation](https://elevenlabs.io/docs/api-reference/sound-generation/create)
- [OpenAPI](openapi/elevenlabs-sound-effects-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/elevenlabs-sound-effects.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/elevenlabs-sound-effects.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ElevenLabs Audio Isolation API

The ElevenLabs Audio Isolation API removes background noise from audio recordings, isolating vocal tracks from ambient sounds and interference. This is useful for cleaning up recordings, improving audio quality for podcasts and interviews, and preparing audio files for further processing such as voice cloning or transcription. The API processes audio files and returns cleaned versions with the vocal content preserved.

- **Human URL:** [https://elevenlabs.io/docs/api-reference/audio-isolation/audio-isolation](https://elevenlabs.io/docs/api-reference/audio-isolation/audio-isolation)
- **Base URL:** `https://api.elevenlabs.io`

#### Tags

- Audio Isolation
- Audio Processing
- Noise Removal

#### Properties

- [Documentation](https://elevenlabs.io/docs/api-reference/audio-isolation/audio-isolation)
- [OpenAPI](openapi/elevenlabs-audio-isolation-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/elevenlabs-audio-isolation.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/elevenlabs-audio-isolation.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ElevenLabs Dubbing API

The ElevenLabs Dubbing API enables automatic translation and voice-over of audio and video content into different languages. It preserves the original speaker's voice characteristics while translating the spoken content, supporting seamless localization of multimedia content. The API handles the full dubbing pipeline including transcription, translation, and speech synthesis with lip-sync timing.

- **Human URL:** [https://elevenlabs.io/docs/api-reference/dubbing/resources/dub-segment](https://elevenlabs.io/docs/api-reference/dubbing/resources/dub-segment)
- **Base URL:** `https://api.elevenlabs.io`

#### Tags

- Audio
- Dubbing
- Localization
- Translation
- Video

#### Properties

- [Documentation](https://elevenlabs.io/docs/api-reference/dubbing/resources/dub-segment)
- [OpenAPI](openapi/elevenlabs-dubbing-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/elevenlabs-dubbing.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/elevenlabs-dubbing.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ElevenLabs Voice Changer API

The ElevenLabs Voice Changer API performs speech-to-speech conversion, replacing one voice with another while preserving the original speech content, timing, and emotional delivery. Developers can transform audio recordings to sound like a different speaker using any voice from the ElevenLabs library or a custom cloned voice. This is useful for content creation, privacy protection, and character voice generation.

- **Human URL:** [https://elevenlabs.io/docs/api-reference/speech-to-speech/convert](https://elevenlabs.io/docs/api-reference/speech-to-speech/convert)
- **Base URL:** `https://api.elevenlabs.io`

#### Tags

- Audio Processing
- Voice Changer
- Voice Conversion

#### Properties

- [Documentation](https://elevenlabs.io/docs/api-reference/speech-to-speech/convert)
- [OpenAPI](openapi/elevenlabs-voice-changer-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/elevenlabs-voice-changer.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/elevenlabs-voice-changer.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ElevenLabs Music Generation API

The ElevenLabs Music Generation API creates music from text prompts, allowing developers to generate original musical compositions programmatically. Users describe the desired genre, mood, tempo, and instrumentation in natural language and receive generated audio output. The API is designed for applications that need background music, jingles, or custom soundtracks without requiring manual composition.

- **Human URL:** [https://elevenlabs.io/docs/overview/capabilities/music](https://elevenlabs.io/docs/overview/capabilities/music)
- **Base URL:** `https://api.elevenlabs.io`

#### Tags

- AI
- Audio Generation
- Music

#### Properties

- [Documentation](https://elevenlabs.io/docs/overview/capabilities/music)
- [OpenAPI](openapi/elevenlabs-music-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/elevenlabs-music.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/elevenlabs-music.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### ElevenLabs Conversational AI API

The ElevenLabs Conversational AI API enables developers to build interactive voice agents that can engage in natural, real-time conversations. It combines speech recognition, language understanding, and speech synthesis into a unified interface supporting multi-turn dialogue across 70+ languages. The API is designed for building customer service agents, voice assistants, and interactive voice response systems with expressive, human-sounding voices.

- **Human URL:** [https://elevenlabs.io/docs/overview/capabilities/conversational-ai](https://elevenlabs.io/docs/overview/capabilities/conversational-ai)
- **Base URL:** `https://api.elevenlabs.io`

#### Tags

- AI
- Conversational AI
- Real-Time
- Voice Agents

#### Properties

- [Documentation](https://elevenlabs.io/docs/overview/capabilities/conversational-ai)
- [OpenAPI](openapi/elevenlabs-conversational-ai-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/elevenlabs-conversational-ai.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/elevenlabs-conversational-ai.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/elevenlabs-conversational-ai-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [AsyncAPI](asyncapi/elevenlabs-webhooks-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)

### ElevenLabs Studio API

The ElevenLabs Studio API provides programmatic access to the ElevenLabs Studio project management system. Developers can create, manage, and render long-form audio content projects through the API, organizing text into chapters and assigning different voices to different sections. The Studio is designed for producing audiobooks, podcasts, and other long-form audio content at scale.

- **Human URL:** [https://elevenlabs.io/docs/overview/capabilities/projects](https://elevenlabs.io/docs/overview/capabilities/projects)
- **Base URL:** `https://api.elevenlabs.io`

#### Tags

- Content Management
- Projects
- Studio

#### Properties

- [Documentation](https://elevenlabs.io/docs/overview/capabilities/projects)
- [OpenAPI](openapi/elevenlabs-studio-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/elevenlabs-studio.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/elevenlabs-studio.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/elevenlabs)
- [LinkedIn](https://www.linkedin.com/company/elevenlabsio)
- [JSON-LD](json-ld/elevenlabs-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON Schema](json-schema/elevenlabs-voice-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/elevenlabs-agent-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/elevenlabs-webhook-event-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Features](undefined)
- [L L Ms Txt](https://elevenlabs.io/llms.txt)
