---
title: ElevenLabs GraphQL Schema
description: Conceptual GraphQL schema for the ElevenLabs AI voice and speech synthesis platform.
provider: ElevenLabs
baseURL: https://api.elevenlabs.io
docsURL: https://elevenlabs.io/docs/api-reference/
schemaFile: elevenlabs-schema.graphql
version: 1.0.0
created: 2026-06-14
---

# ElevenLabs GraphQL Schema

This is a conceptual GraphQL schema representing the ElevenLabs AI voice and speech synthesis platform. ElevenLabs provides a REST API; this schema translates those REST capabilities into a strongly-typed GraphQL surface, making it straightforward to compose voice, audio, and conversational AI operations in a single query layer.

## Coverage

The schema covers the full breadth of the ElevenLabs platform:

- **Voice Management** — list, retrieve, add, edit, delete, and share voices; manage voice settings; browse the public voice library.
- **Text-to-Speech (TTS)** — synthesize speech from text using any voice and model, with control over output format, latency optimization, seed, and text normalization.
- **Speech-to-Speech (STS)** — convert an uploaded audio recording to a target voice while preserving timing and emotion.
- **Voice Cloning** — instant voice cloning from short audio samples and professional voice cloning with verification.
- **Voice Design** — generate novel AI voices from text descriptions specifying gender, age, accent, and strength, then save them to the library.
- **Sound Effects** — generate cinematic sound effects from natural language descriptions.
- **Audio Isolation** — remove background noise from uploaded audio.
- **Dubbing** — create and manage dubbing projects that translate video or audio into target languages while preserving speaker voice characteristics.
- **Generation History** — browse and manage TTS and STS generation history.
- **Studio Projects** — create and render long-form audio projects organized into chapters with per-chapter voice and model assignments.
- **Conversational AI Agents** — configure, deploy, and query real-time voice agents with LLM prompts, knowledge bases, and tool integrations.
- **Pronunciation Dictionaries** — manage custom pronunciation dictionaries referenced in TTS requests.
- **Subscription and Usage** — retrieve current plan, character usage, quotas, and invoice information.
- **API Keys and Webhooks** — manage API credentials and register webhook endpoints for async event delivery.

## Types

| Type | Purpose |
|---|---|
| `Voice` | Full voice resource with metadata, samples, and settings |
| `VoiceDetails` | Extended voice metadata including sharing and fine-tuning state |
| `VoiceID` | Scalar — unique voice identifier |
| `VoiceName` | Scalar — display name for a voice |
| `VoiceCategory` | Enum — PREMADE, CLONED, GENERATED, PROFESSIONAL |
| `VoiceLabels` | Accent, description, age, gender, and use-case tags |
| `VoiceSamples` | Collection of audio samples for a voice |
| `VoiceSample` | A single audio sample with file metadata |
| `SampleID` | Scalar — unique sample identifier |
| `VoiceSettings` | Stability, similarity boost, style, and speaker boost parameters |
| `Stability` | Scalar — delivery consistency (0.0–1.0) |
| `SimilarityBoost` | Scalar — voice likeness strength (0.0–1.0) |
| `Style` | Scalar — style exaggeration level (0.0–1.0) |
| `SpeakerBoost` | Scalar — speaker boost toggle |
| `VoiceDesign` | Parameters for generating a new voice from a text description |
| `VoiceDescription` | Scalar — natural language voice description |
| `VoiceCreation` | Input parameters for creating a voice from audio files |
| `ClonedVoice` | A cloned voice resource returned after creation |
| `VoiceClone` | Clone creation result with verification status |
| `VoiceSharingEnabled` | Scalar — sharing toggle state |
| `AddVoiceRequest` | Input for adding a new voice |
| `SharedVoice` | A voice shared publicly in the library |
| `VoiceSharing` | Sharing metadata including likes, clones, and review status |
| `VoiceLibrary` | Paginated listing of shared voices |
| `VoiceFineTuning` | Fine-tuning progress and model association |
| `VoiceVerification` | Professional clone verification status |
| `VoiceVerificationAttempt` | Individual verification attempt record |
| `TextToSpeech` | TTS operation context |
| `TTSRequest` | Request parameters for a TTS synthesis |
| `TTSResult` | Synthesized audio with metadata |
| `AudioOutput` | Downloadable audio descriptor |
| `OutputFormat` | Enum — MP3/PCM/ULAW at various bitrates and sample rates |
| `AudioStream` | WebSocket streaming session descriptor |
| `LatencyOptimization` | Enum — DEFAULT, NORMAL, STRONG, MAX, MAX_TEXT_NORMALIZER |
| `ModelID` | Scalar — unique model identifier |
| `TTSModel` | Synthesis model with capabilities and limits |
| `ModelLanguage` | A language supported by a model |
| `SpeechToSpeech` | STS operation context |
| `STSRequest` | Request parameters for a speech-to-speech conversion |
| `STSResult` | Converted audio with metadata |
| `AudioInput` | Metadata descriptor for an uploaded audio file |
| `DubbingProject` | A dubbing project summary |
| `Dubbing` | Full dubbing resource with segment detail |
| `DubLanguage` | Enum — supported dubbing target/source languages |
| `DubSegment` | A timed segment within a dubbing project |
| `DubSource` | Source media descriptor |
| `SoundEffect` | A generated sound effect result |
| `SoundEffectRequest` | Request parameters for sound effect generation |
| `VoiceGeneration` | A generated voice preview from a design prompt |
| `GenerationHistory` | Paginated generation history |
| `HistoryItem` | A single generation history record |
| `ItemDetails` | Detailed metadata for a history item |
| `CharacterCount` | Scalar — character usage count |
| `TTSUsage` | Aggregate TTS usage statistics |
| `SubscriptionPlan` | Enum — FREE, STARTER, CREATOR, PRO, SCALE, BUSINESS, ENTERPRISE |
| `SubscriptionInfo` | Current subscription and character usage |
| `PlanQuota` | Hard limits for a given subscription plan |
| `SubscriptionInvoice` | Next invoice details |
| `APIKey` | An ElevenLabs API key resource |
| `Token` | A session authentication token |
| `Webhook` | A registered webhook endpoint |
| `WebhookEvent` | An event payload delivered to a webhook |
| `WebhookEventType` | Enum — async event types (TTS_COMPLETED, DUBBING_COMPLETED, etc.) |
| `PronunciationDictionary` | A custom pronunciation dictionary |
| `PronunciationDictionaryLocator` | Reference to a dictionary version for TTS requests |
| `ConversationalAgent` | An AI voice agent configuration |
| `AgentPrompt` | System prompt and LLM parameters for an agent |
| `AgentTool` | A tool available to a conversational agent |
| `KnowledgeBaseDocument` | A document in an agent's knowledge base |
| `Conversation` | A conversation session with an agent |
| `ConversationTurn` | A single turn in a conversation |
| `StudioProject` | A long-form audio project |
| `ProjectChapter` | A chapter within a Studio project |
| `VoiceSettingsInput` | Input type for voice settings mutations |

## Queries

- `voices` — list all voices accessible to the authenticated user
- `voice(voiceId)` — retrieve full details for a single voice
- `defaultVoiceSettings` — retrieve system default voice settings
- `voiceLibrary(...)` — search and paginate the public shared voice library
- `models` — list all available synthesis models
- `history(...)` — paginate generation history
- `historyItem(historyItemId)` — retrieve a single history record
- `subscription` — current plan tier, character usage, and limits
- `planQuota(plan)` — hard limits for any given plan tier
- `apiKeys` — list API keys
- `webhooks` — list registered webhook endpoints
- `dubbingProject(dubbingId)` — retrieve a dubbing project with segments
- `studioProjects` — list all Studio projects
- `studioProject(projectId)` — retrieve a single Studio project
- `pronunciationDictionaries` — list pronunciation dictionaries
- `conversationalAgents` — list configured voice agents
- `conversationalAgent(agentId)` — retrieve a single agent configuration
- `conversation(conversationId)` — retrieve a conversation session with transcript

## Mutations

- `textToSpeech` — synthesize text to audio
- `speechToSpeech` — convert audio to a target voice
- `generateSoundEffect` — generate a sound effect from a description
- `designVoice` — preview generated voices from demographic parameters
- `saveDesignedVoice` — save a generated voice preview to the library
- `addVoice` — create a new cloned voice from audio samples
- `editVoice` — update a voice name, description, or labels
- `deleteVoice` — remove a voice
- `shareVoice` — enable or disable public sharing for a voice
- `addSharedVoice` — copy a shared voice to the authenticated user's library
- `updateVoiceSettings` — update fine-grained synthesis parameters for a voice
- `createDubbing` — start a dubbing project
- `deleteDubbing` — remove a dubbing project
- `isolateAudio` — strip background noise from an audio file
- `deleteHistoryItems` — remove history records
- `createStudioProject` — initialize a new long-form audio project
- `addProjectChapter` — add a chapter to a Studio project
- `convertProject` — render a Studio project to audio
- `createConversationalAgent` — configure a new voice agent
- `updateConversationalAgent` — update an existing agent
- `deleteConversationalAgent` — remove an agent
- `createWebhook` — register a webhook endpoint
- `deleteWebhook` — remove a webhook
- `createAPIKey` — generate a new API key
- `deleteAPIKey` — revoke an API key
- `createPronunciationDictionary` — upload a pronunciation dictionary

## References

- API Reference: https://elevenlabs.io/docs/api-reference/
- GitHub: https://github.com/elevenlabs
- Pricing: https://elevenlabs.io/pricing
