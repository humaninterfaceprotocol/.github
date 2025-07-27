# Human Interface Protocol (HIP) - A Standard for Agent ↔ Human Communication

Welcome to the official GitHub organization for **Human Interface Protocol (HIP)** — an open, channel-agnostic standard for enabling structured, contextual interactions between applications (or agents) and human users across any medium: web, mobile, chat, email, voice, or beyond.

HIP abstracts the *how* of human communication so developers can focus on *what* they want to say — not how to deliver it. Write once, interact anywhere.

> **Early Stage Project**: The HIP repositories are in active development. Initial code, spec drafts, and reference implementations are coming soon. Follow this space and watch the repos to stay updated!

---

## What is HIP?

HIP enables systems (like apps, backend services, or AI agents) to deliver information and gather input from humans, using a unified protocol. Instead of building channel-specific logic (e.g., a chatbot UI, email system, or IVR call flow), developers can use HIP to:

- Prompt the user for input (`input_request`)
- Send updates or messages (`display_data`)
- Receive structured responses (`user_response`)
- Maintain conversational state (`session_start`, `session_end`, `error`, etc.)

All communication happens via **structured JSON messages** exchanged between:

- **HIP Server** (the conversation orchestrator)
- **HIP Clients** (channel-specific UI adapters, like web widgets, SMS bots, email renderers)

Inspired by [Multi-Context Protocol (MCP)](https://github.com/modelcontextprotocol), HIP brings the same rigor and interoperability to human-facing interfaces.

---

## Architecture

<pre>
+------------------+                           +------------------+
|    HIP Server    | <-------- JSON -------->  |    HIP Client     |
|  (App/Agent Side)|                           | (UI/Channel Side) |
+------------------+                           +------------------+

Responsibilities:                             Responsibilities:

• Maintains session state                     • Renders prompts
• Decides what to say                         • Collects user input
• Sends display/input messages                • Sends responses
</pre>


 Each HIP Client adapts the standard protocol to a specific medium (e.g. a web chat widget, SMS bot, voice IVR, etc.). The HIP Server manages the interaction logic and state.

---

## Repository Overview (tenative)

| Repo | Description |
|------|-------------|
| `hip-spec` | The formal HIP specification and JSON schema definitions. All core protocol details live here. *(Coming soon)* |
| `hip-server` | Reference server that handles session orchestration, message routing, and conversational flow logic. *(Coming soon)* |
| `hip-web-client` | Web UI widget that renders HIP messages as interactive components in a browser. *(Coming soon)* |
| `hip-sdk-js` | JavaScript/TypeScript SDK for developers building HIP-compatible servers or clients. *(Coming soon)* |
| `hip-sdk-py` | *(Planned)* Python SDK for server-side HIP developers. |
| `hip-email-client`, `hip-sms-client`, `hip-voice-client` | *(Planned)* Reference clients for alternate communication channels. |

---

## Getting Started

**Coming soon:** We’re preparing the first working examples and developer guides. Once released, this section will walk you through:

- Running the HIP Server locally
- Connecting the Web Client
- Viewing and inspecting HIP message flows

For now, watch this space and star the repos to stay in the loop!

---

## Roadmap Highlights

| Timeline | Goals |
|----------|-------|
| Milestone 1 | MVP spec, web client, server |
| Next | Add email/SMS clients, session state across channels, capability negotiation |
| Mid-term | Voice channel, mobile SDKs, HIP–MCP integration examples |
| v1.0 Release | Spec freeze, compliance test suite, governance council |

See `ROADMAP.md` for full details.

---

## Contributing

HIP is an open standard built for and by the community. Contributions of all types are welcome:

- Code (fixes, features, clients)
- Docs (examples, tutorials, clarifications)
- Feedback (issues, ideas, use cases)
- Integrations (chat, IVR, mobile, AR/VR, etc.)

Want to get involved early? Email us at `manish@humaninterfaceprotocol.io` and we’ll share how you can help.

Start with `CONTRIBUTING.md` and browse open issues with the label `good first issue`. *(Coming soon)*

---

## License

All code and specifications in this organization are released under the **MIT License**. You’re free to use, fork, extend, and integrate HIP however you’d like — with attribution.

---

## Join the Community

- GitHub Discussions – for design ideas, use cases, and Q&A  
- Discord (Coming soon) – for real-time collaboration  

---

### Let’s standardize how machines talk to humans

HIP is built on the belief that AI agents, apps, and backends should speak the *same human language*, no matter the medium. Let’s build this protocol together.

Made by the HIP core team and contributors across the world.
