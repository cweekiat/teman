# Teman: a cancer care companion for Singapore

*Teman* means "companion" in Malay. Teman is a **concept and design repository** for an iOS app. The app would help people with cancer in Singapore, and the people who care for them, to:

- understand a diagnosis and the medical words around it
- find the right care: physical, emotional, psychological and financial
- keep track of appointments and get to them
- understand the treatment process and its side effects
- ask their doctors the right questions, and speak up for themselves

**Project site:** https://cweekiat.github.io/teman/

> **Status:** concept, design and architecture only. No app has shipped, so nothing here is a medical product.

---

## What Teman will never do

These are product boundaries, not disclaimers added at the end. Each one is enforced in the design (see [docs/safety-and-privacy.md](docs/safety-and-privacy.md)).

| Teman does **not** | Instead, Teman |
|---|---|
| Diagnose cancer or interpret a result as good or bad | Explains what a term *means*, cites the source, and suggests the question to ask the doctor |
| Choose, rank or recommend a treatment | Explains how a treatment the care team has named generally works, with citations, and helps the patient prepare questions about it |
| Determine clinical-trial eligibility | Explains what trials are and gives questions to ask the oncologist |
| Replace the medical team | Sends every clinical question back to the care team, and gives emergency numbers (995) prominence |
| Say anything medical without a source | Cites a named, trusted source for every medical statement and shows when it was last checked. If there is no source, it does not answer |
| Share patient information | Keeps all data on the device, with no accounts, analytics or ads. Data leaves the phone only when the patient exports it |

## Who it is for

The work is built around three things patients and caregivers say:

> "You have to be a huge patient advocate. Push for answers. Push for biopsies. Push for proper testing. Ask questions."

> "I need help navigating difficult conversations and advocating for myself."

> "The volume of doctors, documents, and insurance paperwork can quickly become overwhelming."

[docs/product.md](docs/product.md) maps each quote to features.

## The journey Teman follows

1. **Just diagnosed:** understand the words and know what to ask first.
2. **Building the care team:** know who is who and who to call.
3. **Planning treatment:** prepare questions, understand options the doctor has named, and get a second opinion.
4. **Paying for care:** MediShield Life, the Cancer Drug List, MediSave, MediFund and charity schemes.
5. **During treatment:** appointments, transport, side effects and when to call.
6. **Mind and family:** psychosocial support, caregivers and difficult conversations.
7. **After treatment, or when the goals of care change:** survivorship, or palliative and hospice care.

## Docs

| Doc | What's in it |
|---|---|
| [Product brainstorm](docs/product.md) | People, the journey, every feature, and the patient quotes each one answers |
| [Design (Apple HIG)](docs/design-hig.md) | Navigation, accessibility, onboarding, permissions, notifications and voice, each tied to the Human Interface Guideline it follows |
| [Native iOS frameworks](docs/frameworks.md) | Which Apple framework does which job, and why |
| [On-device LLMs](docs/on-device-llm.md) | How offline language models can help, the guardrails around them, and how to evaluate them |
| [Architecture](docs/architecture.md) | Modules, data model, citation pipeline and Swift sketches |
| [Safety and privacy](docs/safety-and-privacy.md) | Clinical boundaries, red flags, HSA software-as-a-medical-device positioning, and the PDPA |
| [Source registry](docs/sources.md) | Every trusted Singapore source Teman draws on, and the review cadence |

## In an emergency

Teman is not an emergency service. Call **995** for an emergency ambulance in Singapore. If you are on cancer treatment and feel unwell, call the number your care team gave you.

## Licence

Documentation: CC BY 4.0. Code samples: MIT. Source content belongs to its publishers. Teman links to and cites it, and does not republish it.
