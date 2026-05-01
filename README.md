# ElevenLabs (elevenlabs)
ElevenLabs is an AI audio platform that provides a comprehensive suite of APIs for generating, transforming, and managing audio content. Their developer platform offers capabilities spanning text-to-speech, speech-to-text, voice cloning, sound effects generation, music creation, dubbing, and conversational AI agents, all accessible through a unified API at api.elevenlabs.io.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/elevenlabs/refs/heads/main/apis.yml)

## Scope

- **Type:** Contract
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags:

 - AI, Audio, Voice, Text To Speech, Speech Synthesis, Conversational AI

## Timestamps

- **Created:** 2025-03-01
- **Modified:** 2026-04-28

## APIs

### ElevenLabs Text to Speech API
The ElevenLabs Text to Speech API converts text into lifelike spoken audio with nuanced intonation, pacing, and emotional awareness. It supports multiple output formats including MP3, PCM, and mu-law, and offers a range of models such as Flash v2.5 for ultra-low latency real-time applications and Multilingual v2 for support across 70+ languages. Developers can select from thousands of pre-built voices or use custom cloned voices to generate speech that sounds natural and expressive.

**Human URL:** [https://elevenlabs.io/docs/api-reference/text-to-speech/convert](https://elevenlabs.io/docs/api-reference/text-to-speech/convert)


#### Tags:

 - Text To Speech, Voice, Audio, AI, Speech Synthesis

#### Properties

- [Documentation](https://elevenlabs.io/docs/api-reference/text-to-speech/convert)
- [OpenAPI](openapi/elevenlabs-text-to-speech-openapi.yml)
- [AsyncAPI](asyncapi/elevenlabs-text-to-speech-streaming-asyncapi.yml)

### ElevenLabs Speech to Text API
The ElevenLabs Speech to Text API provides state-of-the-art transcription capabilities, converting spoken audio into accurate text. It supports multiple audio formats and languages, enabling developers to build applications that require reliable audio transcription. The API is designed for both real-time and batch processing use cases.

**Human URL:** [https://elevenlabs.io/docs/api-reference/speech-to-text/convert](https://elevenlabs.io/docs/api-reference/speech-to-text/convert)


#### Tags:

 - Speech To Text, Transcription, Audio, AI

#### Properties

- [Documentation](https://elevenlabs.io/docs/api-reference/speech-to-text/convert)
- [OpenAPI](openapi/elevenlabs-speech-to-text-openapi.yml)

### ElevenLabs Voice Cloning API
The ElevenLabs Voice Cloning API allows developers to create custom AI voices from audio recordings. Instant Voice Cloning requires as little as 60 seconds of clean audio to generate a usable voice clone, while Professional Voice Cloning produces higher fidelity results from a minimum of 30 minutes of recordings. Cloned voices can then be used with the Text to Speech API for generating speech that closely matches the original speaker.

**Human URL:** [https://elevenlabs.io/docs/api-reference/voices/ivc/create](https://elevenlabs.io/docs/api-reference/voices/ivc/create)


#### Tags:

 - Voice Cloning, Voice, AI, Audio

#### Properties

- [Documentation](https://elevenlabs.io/docs/api-reference/voices/ivc/create)
- [OpenAPI](openapi/elevenlabs-voice-cloning-openapi.yml)

### ElevenLabs Voices API
The ElevenLabs Voices API provides management capabilities for the voice library, including listing, retrieving, creating, editing, and deleting voices. Developers can access a library of over 5,000 pre-built voices and manage their own custom voices. The API also supports voice design, allowing creation of new AI voices from text descriptions specifying desired characteristics such as accent, age, and tone.

**Human URL:** [https://elevenlabs.io/docs/api-reference/voices/get](https://elevenlabs.io/docs/api-reference/voices/get)


#### Tags:

 - Voices, Voice Library, Voice Management, AI

#### Properties

- [Documentation](https://elevenlabs.io/docs/api-reference/voices/get)
- [OpenAPI](openapi/elevenlabs-voices-openapi.yml)

### ElevenLabs Sound Effects API
The ElevenLabs Sound Effects API generates cinematic sound effects from text descriptions. Developers can describe the desired sound in natural language and receive high-quality audio output. The API supports audio tags for controlling delivery, emotion, emphasis, pauses, and specific sound effects, making it suitable for game development, film production, and multimedia content creation.

**Human URL:** [https://elevenlabs.io/docs/api-reference/sound-generation/create](https://elevenlabs.io/docs/api-reference/sound-generation/create)


#### Tags:

 - Sound Effects, Audio Generation, AI

#### Properties

- [Documentation](https://elevenlabs.io/docs/api-reference/sound-generation/create)
- [OpenAPI](openapi/elevenlabs-sound-effects-openapi.yml)

### ElevenLabs Audio Isolation API
The ElevenLabs Audio Isolation API removes background noise from audio recordings, isolating vocal tracks from ambient sounds and interference. This is useful for cleaning up recordings, improving audio quality for podcasts and interviews, and preparing audio files for further processing such as voice cloning or transcription. The API processes audio files and returns cleaned versions with the vocal content preserved.

**Human URL:** [https://elevenlabs.io/docs/api-reference/audio-isolation/audio-isolation](https://elevenlabs.io/docs/api-reference/audio-isolation/audio-isolation)


#### Tags:

 - Audio Isolation, Noise Removal, Audio Processing

#### Properties

- [Documentation](https://elevenlabs.io/docs/api-reference/audio-isolation/audio-isolation)
- [OpenAPI](openapi/elevenlabs-audio-isolation-openapi.yml)

### ElevenLabs Dubbing API
The ElevenLabs Dubbing API enables automatic translation and voice-over of audio and video content into different languages. It preserves the original speaker's voice characteristics while translating the spoken content, supporting seamless localization of multimedia content. The API handles the full dubbing pipeline including transcription, translation, and speech synthesis with lip-sync timing.

**Human URL:** [https://elevenlabs.io/docs/api-reference/dubbing/resources/dub-segment](https://elevenlabs.io/docs/api-reference/dubbing/resources/dub-segment)


#### Tags:

 - Dubbing, Translation, Localization, Audio, Video

#### Properties

- [Documentation](https://elevenlabs.io/docs/api-reference/dubbing/resources/dub-segment)
- [OpenAPI](openapi/elevenlabs-dubbing-openapi.yml)

### ElevenLabs Voice Changer API
The ElevenLabs Voice Changer API performs speech-to-speech conversion, replacing one voice with another while preserving the original speech content, timing, and emotional delivery. Developers can transform audio recordings to sound like a different speaker using any voice from the ElevenLabs library or a custom cloned voice. This is useful for content creation, privacy protection, and character voice generation.

**Human URL:** [https://elevenlabs.io/docs/api-reference/speech-to-speech/convert](https://elevenlabs.io/docs/api-reference/speech-to-speech/convert)


#### Tags:

 - Voice Changer, Voice Conversion, Audio Processing

#### Properties

- [Documentation](https://elevenlabs.io/docs/api-reference/speech-to-speech/convert)
- [OpenAPI](openapi/elevenlabs-voice-changer-openapi.yml)

### ElevenLabs Music Generation API
The ElevenLabs Music Generation API creates music from text prompts, allowing developers to generate original musical compositions programmatically. Users describe the desired genre, mood, tempo, and instrumentation in natural language and receive generated audio output. The API is designed for applications that need background music, jingles, or custom soundtracks without requiring manual composition.

**Human URL:** [https://elevenlabs.io/docs/overview/capabilities/music](https://elevenlabs.io/docs/overview/capabilities/music)


#### Tags:

 - Music, Audio Generation, AI

#### Properties

- [Documentation](https://elevenlabs.io/docs/overview/capabilities/music)
- [OpenAPI](openapi/elevenlabs-music-openapi.yml)

### ElevenLabs Conversational AI API
The ElevenLabs Conversational AI API enables developers to build interactive voice agents that can engage in natural, real-time conversations. It combines speech recognition, language understanding, and speech synthesis into a unified interface supporting multi-turn dialogue across 70+ languages. The API is designed for building customer service agents, voice assistants, and interactive voice response systems with expressive, human-sounding voices.

**Human URL:** [https://elevenlabs.io/docs/overview/capabilities/conversational-ai](https://elevenlabs.io/docs/overview/capabilities/conversational-ai)


#### Tags:

 - Conversational AI, Voice Agents, Real-Time, AI

#### Properties

- [Documentation](https://elevenlabs.io/docs/overview/capabilities/conversational-ai)
- [OpenAPI](openapi/elevenlabs-conversational-ai-openapi.yml)
- [AsyncAPI](asyncapi/elevenlabs-conversational-ai-asyncapi.yml)
- [AsyncAPI](asyncapi/elevenlabs-webhooks-asyncapi.yml)

### ElevenLabs Studio API
The ElevenLabs Studio API provides programmatic access to the ElevenLabs Studio project management system. Developers can create, manage, and render long-form audio content projects through the API, organizing text into chapters and assigning different voices to different sections. The Studio is designed for producing audiobooks, podcasts, and other long-form audio content at scale.

**Human URL:** [https://elevenlabs.io/docs/overview/capabilities/projects](https://elevenlabs.io/docs/overview/capabilities/projects)


#### Tags:

 - Studio, Projects, Content Management

#### Properties

- [Documentation](https://elevenlabs.io/docs/overview/capabilities/projects)
- [OpenAPI](openapi/elevenlabs-studio-openapi.yml)

## Common Properties

- [Portal](https://elevenlabs.io/docs)
- [Documentation](https://elevenlabs.io/docs/api-reference)
- [Website](https://elevenlabs.io)
- [PrivacyPolicy](https://elevenlabs.io/privacy)
- [TermsOfService](https://elevenlabs.io/terms)
- [Blog](https://elevenlabs.io/blog)
- [Login](https://elevenlabs.io/app/sign-in)

## Maintainers

**FN:** API Evangelist

**Email:** info@apievangelist.com
