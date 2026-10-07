---
name: writing-plain-english
description: Writes and edits pages of the public Agent Market documentation in plain English. ALWAYS invoke this skill when the user asks to write a docs page, add a guide, edit or rewrite a page or section, fix the wording of a page, or review docs for plain English. Do not write or edit an .mdx page directly — use this skill first.
---

# Writing Plain English

Writing rules for the public Agent Market documentation. Every page under this repo must follow them. The rules cover the words and sentences on a page. They do not cover Mintlify components, frontmatter, or navigation.

## Table of Contents

- [🚨 CRITICAL RULES (NEVER VIOLATE)](#-critical-rules-never-violate)
- [Workflow](#workflow)
- [Who reads the docs](#who-reads-the-docs)
- [Voice](#voice)
- [Sentences](#sentences)
- [Paragraphs and lists](#paragraphs-and-lists)
- [Headings](#headings)
- [Words](#words)
- [Product terms](#product-terms)
- [⚠️ Common Mistakes](#️-common-mistakes)

## 🚨 CRITICAL RULES (NEVER VIOLATE)

1. **ALWAYS run the self-check before you save a page.** A page that skips it ships idioms, two names for one concept, and lost facts.
2. **NEVER trade a fact for a simpler word.** Plain is not fuzzy. If a fee is 10%, write 10%. If a key shows once, write that it shows once.
3. **NEVER rename a technical term, tool name, config key, status value, or UI label.** Simplify the prose around the name, not the name.
4. **ALWAYS use one name per concept.** The product terms table decides which. Two names for one thing on one page is a bug.
5. **NEVER use idioms or metaphors.** No "out of the box", "under the hood", "rabbit hole", "low-hanging fruit", "boils down to". A reader who did not grow up with English stops to decode them.
6. **NEVER put a metaphor in place of a technical fact.** No "blast radius", "footgun", "surface area", "north star", "happy path". Say what breaks, where, and when.
7. **NEVER coin compounds.** No "hire-flow", "escrow-aware", "brief-driven", "MCP-native". If two words need a hyphen to mean something new, find the plain sentence instead.
8. **NEVER use rare phrasal verbs.** "Cancel" not "call off". "Postpone" not "put off". Common ones are fine: "set up", "turn on", "sign in", "find out".
9. **NEVER chain nouns.** "The assignment status update webhook payload" is four nouns too many. Write "the payload the webhook sends when the assignment status changes".
10. **NEVER market.** No exclamation marks. No "amazing", "powerful", "cutting-edge", "state-of-the-art".
11. **NEVER talk down.** Only the language is simple, not the reader. Do not write "don't worry" or "it's easy".
12. **NEVER use time words that go stale.** No "new", "recently", "currently", "soon", "now supports". Write what the product does today as if it always did.
13. **NEVER refer to another page by position.** Not "see above", "as mentioned earlier", "in the previous section". Link to the page or name the section.

## Workflow

### 1. Read before you write

Read the page you edit, or the pages next to the one you add. Note the terms and the voice already in use.

### 2. Write under the rules

Follow every section below. Write for all three readers at once.

### 3. Self-check before you save

Read the finished page once and answer five questions:

1. Is there an idiom, a metaphor, a coined word, or a marketing word? Replace it with the plain fact.
2. Is there a word a non-native engineer has to stop and decode, like the examples in *Words*? Swap it, unless it is a technical word, a tool name, or a UI label.
3. Does any concept use two names on the page? Pick the one from the product terms table and use it everywhere.
4. Is any paragraph over 5 sentences? Split it if the split keeps every fact.
5. Did a simpler word drop a fact, a name, a number, or a status? Put the fact back.

If a fix makes a sentence wrong or strange, keep the original. The rules serve clarity, not the other way round.

## Who reads the docs

Three kinds of people open these pages, often on the same day:

- A developer who connects over MCP or A2A and wants the exact tool name, the exact command, and the expected result.
- A developer whose first language is not English. Rare words slow them down. Technical words do not.
- A non-technical person, such as a product manager or a founder, who hires agents from Claude Desktop and never opens a terminal.

Write for all three at once. Use the simplest word that is still exact. Keep every technical name exact. Never explain a term by making it vaguer.

## Voice

- Write to the reader as **you**. Never "the user", never "one", never "we".
- Use the imperative for steps: "Run the command", "Click **Hire**", "Paste the key".
- Use the present tense for what the system does: "The server returns the job id." Not "will return", not "is going to return".
- Name the actor. "The agent submits the deliverable" tells the reader who acts. "The deliverable is submitted" hides it.
- Do not say "please", "simply", "just", "easily", "note that", "it is worth noting", "basically", "actually", "of course".
- Do not promise or sell. No "powerful", "seamless", "robust", "effortless", "best-in-class". State what the thing does.

## Sentences

- One idea per sentence. If a sentence needs "and" to join two actions, split it.
- Put the result or the instruction first, the reason after. "Accept the deliverable to release payment" beats "To release payment, you need to accept the deliverable".
- Use the direct verb. "The call fails" not "a failure occurs". "The job starts" not "the job enters a started state".
- Say what happens, not what the reader should feel. "The key appears once. Copy it now." Not "Make sure you don't forget to copy the key!"
- Spell out conditions. "If the brief is empty, the API returns `400`." Not "Invalid briefs are rejected."

## Paragraphs and lists

- Five sentences or fewer per paragraph.
- The first sentence of a page says what the reader can do after reading it. The first sentence of a section says what the section covers.
- Use a numbered list when order matters. Use a bulleted list when it does not. Never use a list for one item.
- Each bullet starts with the key word or the action. Each bullet is one idea, one or two sentences.
- A list of steps ends with what the reader sees when the step worked. "The agent card shows a green dot."

## Headings

- Sentence case: "Connect over MCP", not "Connect Over MCP".
- A heading names the task or the thing. "Place a bid", "Job statuses". Not "Getting started with placing your first bid".
- A heading is not a sentence and has no final period.
- Page titles start with a verb for task pages ("Hire an agent over MCP") and with a noun for concept pages ("Escrow and disputes").

## Words

Do not use truly complex English. A word is complex when a non-native engineer has to stop and decode it: a rare Latin verb, an opaque phrasal verb, a phrase that says in four words what one word says. When you meet one, ask: is there a commoner word that means the same thing? If yes, use it.

Technical words stay. *Parameter, payload, endpoint, token, webhook, enabled, required, execute, fetch, cache, async* are exact and every developer knows them. Do not swap a word that is a tool name, a config key, a status value, or a UI label.

A few examples of the kind of word to catch. The list is a prompt, not a rule. Treat any word of the same shape the same way.

| Not this | This |
|---|---|
| commence, cease | start, stop |
| ascertain | find out |
| spin up, tear down | start, stop |
| wire up, hook up | connect |
| errors out | fails |
| head over to | open, go to |

## Product terms

One name per concept. The first column is the only name the docs use for it.

| Use this | Not this | Means |
|---|---|---|
| Agent Market | Agents Market, AgentMarket, the platform, the product | the product. "The marketplace" is fine for the service that runs jobs and holds escrow. |
| agent | bot, AI, worker, assistant, service | an agent listed on Agent Market. "Worker" appears in code names and stays there. |
| buyer | client, customer, user, requester | the account that posts and pays for a job. |
| owner | builder, seller, provider, vendor | the account that lists an agent and gets paid. |
| job | task, order, request, gig, project | the unit of work a buyer posts. |
| brief | prompt, description, instructions, spec | the text the buyer writes and the agent receives. |
| hire | engagement, contract, booking | the act of giving a job to a specific agent. "Hire" is the verb and the noun. |
| assignment | hire (for the record), contract | the record of one agent on one job. Use it when the reader deals with the object, its status, or its id. |
| bid | offer, proposal, application, quote | an agent's response to an open standard job. |
| deliverable | result, output, submission, work product | what the agent submits. |
| escrow | hold, reserve, locked funds | the money set aside for a job until the buyer accepts. |
| payout | withdrawal, disbursement | money that leaves the marketplace to the owner. |
| balance | funds, credits, wallet (as a noun) | the amount an account holds. |
| fee | commission, cut, take rate | what the marketplace keeps. |
| dispute | claim, complaint, appeal | the buyer's challenge to a deliverable. |
| request changes | revision, rework, send back | the buyer asks the agent to redo part of the work. |
| instant job | direct hire, quick job | a job that goes to one chosen agent with no bidding. |
| standard job | open job, bidding job, public job | a job agents bid on. |
| self-hosted agent | external agent, remote agent, webhook agent, HTTP agent | an agent that runs on its owner's servers. |
| managed agent | marketplace-hosted, marketplace-managed, hosted agent, internal agent | an agent that runs on Agent Market. |
| webhook | callback, hook, listener | the URL the marketplace calls for a self-hosted agent. |
| MCP, A2A, x402 | spell-outs on every use | spell out once per page on first use, then use the short form. |

Some of these words are both a verb and a noun. "Hire an agent" and "the hire" are both fine. "Bid on a job" and "the bid" are both fine. Do not invent a third form such as "hiring request" or "bidding entry".

This table drifts from the code over time. From time to time, ask the engineers to check it against the Agent Market repository: entity names, status values, tool names, and the product name. Fix the table, not the code.

## ⚠️ Common Mistakes

| Issue | Solution |
|---|---|
