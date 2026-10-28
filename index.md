# AI Prompt Log — Vineyard Experience & Visitor Flow Management System

Requirements Engineering 2026/2027 — FCT NOVA — Deliverable 1
Group 5: João Rivera 73418, Simão Carrasco 76907, Tomás Simões 73894

---

## About this log

This page records the AI prompts our group used while preparing Deliverable 1, as required by the project's AI Use Declaration. For each prompt we record the date, the tool and model, the report section it contributed to, the context we gave, the prompting technique, the exact prompt, a summary of the output, and what we kept, changed or rejected.

Outputs are summarised rather than reproduced in full, because many responses were revised versions of the same report text. The summary records what each output contributed, and the "Kept / changed / rejected" line records how we used it.

Prompts were written together during group sessions, so they are not attributed to individual members.

Prompts are quoted exactly as sent, including typos. Prompts that were only about formatting or tools (e.g., Google Docs table borders, file formats) are not listed, because they did not affect the content of the report.

## Tools

| Tool | Model |
|---|---|
| Claude (Anthropic), via the Claude app | claude-opus-5-5 |

## How we prompted

We followed the prompting guidance from the AI4RE lecture (Moreira, 2026):

- **Context.** All prompts were sent within ongoing chat sessions, so each one also had the earlier conversation as context (session context). Most prompts gave no worked examples, but included our own drafts, the project brief, lab templates or lecture slides as user context, which kept outputs specific to our project.
- **Technique.** Most prompts were zero-shot (no worked examples). Some were template-based, using the templates from Lab 3 or the structure of the project brief. One (entry 11) used the SusAD examples from the sustainability lecture as reference.
- **Pattern.** Most prompts were plain requests or questions. The AI-assisted brainstorm (entry 13) used the RTF pattern (Role, Task, Format).

## How we checked outputs

We checked AI outputs with the five checks from the AI4RE lecture:

1. **Source:** every statement traced back to our Miro work or the project brief; anything without a source treated as an assumption.
2. **Omissions:** AI suggestions compared with our own stakeholder and POV lists.
3. **Quality:** requirements checked against the ISO/IEC/IEEE 29148 criteria (unambiguous, verifiable, singular, etc.).
4. **Consistency:** checked against the glossary and the traceability table.
5. **Record:** this log.

Numeric thresholds suggested by AI (e.g., 5 minutes, 90%, ±20%) were treated as assumptions (A4 in the report). References were checked against the original sources. AI was not used to simulate stakeholders.

---

## Prompt entries

### Entry 1 — Lab 3 walkthrough
- **Date:** 28 Sep 2026
- **Tool / model:** Claude, claude-opus-5-5
- **Report section:** 4.2, 4.3, 6 (early drafts)
- **Context provided:** Lab 3 PDF (with the POV, user story and requirement templates) and the project brief
- **Technique:** Zero-shot, with templates from the lab
- **Prompt:**
  > help me do this lab taking into account this project :
- **Output (summary):** Brainstorm themes; example POVs for a tasting room manager; user stories; first FRs and NFRs; interview and survey questions; a mock interview kit.
- **Kept / changed / rejected:** The tasting room manager POVs became the basis for POV2 and POV3, rewritten by us. The mock interview kit was not used.

### Entry 2 — Refining POV1
- **Date:** 28 Sep 2026
- **Tool / model:** Claude, claude-opus-5-5
- **Report section:** 4.2, Table 16
- **Context provided:** Our own POV1 draft; the project brief and Lab 3 earlier in the chat
- **Technique:** Zero-shot (refining our draft)
- **Prompt:**
  > can you refine this pov POV1: A senior visitor needs good acessibility due to his bad joints, because typical vineyards are in the mountain so they dont have the best accesses.
- **Output (summary):** A critique (the need was vague, the insight obvious) and two refined versions.
- **Kept / changed / rejected:** Kept the first version as POV1; the before/after is recorded in Table 16.

### Entry 3 — User stories, FRs and NFRs for POV1
- **Date:** 28 Sep 2026
- **Tool / model:** Claude, claude-opus-5-5
- **Report section:** 4.3, 6.2, 6.3
- **Context provided:** Our refined POV1 and our own user stories; the lab templates earlier in the chat ("As a…, I want…, so that…"; "[Subject] shall [action] [object] [constraint]")
- **Technique:** Template-based (lab templates)
- **Prompts:**
  > user stories for this as well

  > help me write the nfr and fr for this US1: As a senior visitor with limited mobility i want to see each vineyards accessibility details before getting off, so that I only stop where I can visit. US2: As a senior visitor I want to see when the nect train will pick me up at each stop so that Im not waiting around for the next train for too long.
- **Output (summary):** Three user stories; FR1–FR3 and NFR1–NFR2 with quality notes.
- **Kept / changed / rejected:** We kept our own US1 and US2. The FR/NFR drafts were edited by us (e.g., NFR2 threshold changed from 3 to 5 minutes).

### Entry 4 — Telling FRs from NFRs
- **Date:** 28 Sep 2026
- **Tool / model:** Claude, claude-opus-5-5
- **Report section:** 6.2, 6.3, Table 16
- **Context provided:** Our FR/NFR drafts and the earlier conversation
- **Technique:** Zero-shot (questions)
- **Prompts:**
  > would the app working offline or like displaying the latest updated timetable offline be nfr or fr how do you distinguishe between them

  > so the app being intuitive would be an nfr right
- **Output (summary):** A rule for telling FRs from NFRs; the offline requirement split into NFR4 (quality) and FR5 (behaviour); a measurable rewrite of "intuitive".
- **Kept / changed / rejected:** Kept both. NFR3 rewritten and FR5 added (Table 16).

### Entry 5 — Visitor-oriented interview and survey
- **Date:** 28 Sep 2026
- **Tool / model:** Claude, claude-opus-5-5
- **Report section:** 3.4, 3.5
- **Context provided:** Our existing interview and survey questions; our POVs and requirements in the chat
- **Technique:** Zero-shot
- **Prompt:**
  > do the inteview and survey more directed to the clients
- **Output (summary):** Five visitor interview questions and five survey questions, each mapped to the requirement it checks.
- **Kept / changed / rejected:** Our group wrote its own question set in Miro; the AI version was later used to review it (entry 6).

### Entry 6 — Review of our Miro work
- **Date:** 18 Oct 2026
- **Tool / model:** Claude, claude-opus-5-5
- **Report section:** Whole report, Table 16
- **Context provided:** Screenshots of our Miro boards (stakeholders, POVs, user stories, requirements with trace arrows, interview and survey) and the brief's Deliverable 1 list
- **Technique:** Zero-shot
- **Prompts:**
  > okay for the first delivery of the project what do we need

  > okay im going to make a google docs to share with my group members to start this we have already done some stuff in miro
- **Output (summary):** The Deliverable 1 contents list; a report skeleton; a critique of our POVs, user stories, requirements and questions (missing insights, a leading survey question, NFR5 being a function).
- **Kept / changed / rejected:** Most of the critique was accepted (Table 16). The surgery mind map in Miro was from a class exercise and was left out.

### Entry 7 — First report drafts
- **Date:** 18 Oct 2026
- **Tool / model:** Claude, claude-opus-5-5
- **Report section:** All sections first marked "AI-drafted"
- **Context provided:** Our Miro content as text, the brief's Deliverable 1 structure, and the review from entry 6
- **Technique:** Template-based (the brief's report structure)
- **Prompts:**
  > yes that exactly you can add some details that make sense from what we add and suggestions, where suggestions are done say it as a todo or something

  > okay i put it into the google docs the todos you said that are fixes you can just do them send me the text again with those ifxes, the todos i was refering was like stuff that was not done at all which I want you to but mark it as being done by you and needing review mark todo as only the syff that really needs our feeback and you cant infer from what I sent you
- **Output (summary):** Draft report versions 1 and 2. Our content kept as written; added sections labelled "AI-drafted, needs group review": stakeholder table, US9–US15, FR5–FR19, NFR5–NFR8, sustainability requirements, first SusAF analysis.
- **Kept / changed / rejected:** Reviewed by the group and kept with minor edits; no major errors found.

### Entry 8 — Restructuring for the updated brief
- **Date:** 19 Oct 2026
- **Tool / model:** Claude, claude-opus-5-5
- **Report section:** Whole report
- **Context provided:** The updated project brief (19 Oct) and our current draft
- **Technique:** Zero-shot
- **Prompts:**
  > there was an update to the project does this change anything

  > okaysend me the sections that need to be overwritten
- **Output (summary):** List of changes (iStar, UML and SIG moved to Deliverable 2; context diagram, contribution table, 15+ domain glossary terms and SusAD added); replacement sections; a context diagram image.
- **Kept / changed / rejected:** Report restructured into the new sections 1–7. Context diagram to be redrawn in our modelling tool.

### Entry 9 — AI use and verification
- **Date:** 26 Oct 2026
- **Tool / model:** Claude, claude-opus-5-5
- **Report section:** 3.6, AI Use Declaration
- **Context provided:** The AI4RE lecture slides
- **Technique:** Zero-shot
- **Prompts:**
  > I also have this

  > just give me the text ill paste it and complete wtv is needed
- **Output (summary):** How to apply the five checks; the prompt-logging format used on this page; an RTF prompt for the AI brainstorm; AI declaration text.
- **Kept / changed / rejected:** Used for the verification section and this log's format.

### Entry 10 — Stakeholder and scope reduction (rejected)
- **Date:** 26 Oct 2026
- **Tool / model:** Claude, claude-opus-5-5
- **Report section:** 2, 1.3
- **Context provided:** The project brief and our current report
- **Technique:** Zero-shot
- **Prompts:**
  > i think we would want to drop some stakeholders maybe to reduce the scope of the process, my professor asks for some reasoning about it do you think the current report already tackles some of this and to drop some i was thinking these, sponsor, shipping company,customs, local residents, suppliers something among these lines

  > our system might be too broad mayeb reducing the scope overall for the system this would casacde adn reduce everything else , what were the guide specifications for the system
- **Output (summary):** Scoping criteria; a table of stakeholders to exclude; a reduced scope of about 10 FRs.
- **Kept / changed / rejected:** Rejected. After talking to the professors, we kept all stakeholders and used MoSCoW to prioritise instead.

### Entry 11 — SusAF and SusAD
- **Date:** 26 Oct 2026
- **Tool / model:** Claude, claude-opus-5-5
- **Report section:** 7, 6.4
- **Context provided:** Our SusAF tables; then the sustainability lecture slides (with the Airbnb and mobility SusAD examples); then our teacher's feedback on arrow direction
- **Technique:** Zero-shot, refined using the lecture's SusAD examples as reference
- **Prompts:**
  > can you generate me the susaf diagram, one thing also the description of the effects across dimentions are too long i think to put in the susaf

  > okay about this do the threats appear in this i did not think they did, also my teahcer sad the arrows should be from inside to outside or in the same tier

  > the ist dimentsion social is not making mych sense to me is this according to the pdf i sent you and stuff thee seem like issues not just structural or types of sustainability if they are correct acording to the pdf thats fine

  > the todos in the table 22 what do you need me to do
- **Output (summary):** A first circular SusAD (which wrongly mixed threats into the diagram and had one inward arrow); a pentagon redraw following the lecture method; shorter labels; Social labels checked against the lecture's themes; an energy-use effect; synthesis tables; SR9–SR11.
- **Kept / changed / rejected:** The first version was rejected because it did not follow the lecture method or our teacher's feedback, which we noticed ourselves (Table 16). The final version is kept and redrawn in our modelling tool.

### Entry 12 — Consistency review
- **Date:** 26 Oct 2026
- **Tool / model:** Claude, claude-opus-5-5
- **Report section:** Whole report
- **Context provided:** The full current report text
- **Technique:** Zero-shot
- **Prompts:**
  > OKAY Heres the current state of the report

  > okay tell me everything then that neds changing again heres the latest , lets go from top to bottom
- **Output (summary):** A top-to-bottom list of fixes (outdated IDs, duplicate table numbers, missing requirements, wording implying the interview had been carried out).
- **Kept / changed / rejected:** The suggested fixes were reviewed and applied.

### Entry 13 — AI-assisted brainstorm (Section 3.6)
- **Date:** TODO
- **Tool / model:** Claude, claude-opus-5-5
- **Report section:** 3.6, Table 9
- **Context provided:** None beyond the prompt (run in a new chat)
- **Technique:** Zero-shot, RTF pattern (Role, Task, Format)
- **Prompt:**
  > You are a requirements engineer for a hop-on/hop-off wine route system. Identify where AI could add value for each stakeholder: visitors, tasting room managers, drivers, shipping companies and the route association. Output a table with the columns: AI opportunity, stakeholder, value, risk. Mark any idea where a deterministic rule would work better than AI.
- **Output (summary):** See Table 9 in the report (seven AI opportunities with stakeholder, value and risk).
- **Kept / changed / rejected:** Reviewed by the group; kept as Table 9. Shipping eligibility was identified as a deterministic rule rather than an AI task, and each AI risk was turned into an NFR or sustainability requirement (e.g., SR4, SR5).
