---
title: "Invisible Labor of AI: The Truth About RAG, Agents, and 'Learning'"
description: "Most AI systems don’t actually learn — they rely on hidden human work to keep them useful."
date: "2025-09-23"
author: "Rohit Harsh"
tags: ["LLM", "RAG", "AgenticAI", "Learning", "AIReality"]
icon: "🛠️"
gradient: "from-purple-100 to-indigo-100"
patternGradient: "from-purple-200/50 to-indigo-200/50"
---

Last year companies spent around [$250 billion on AI](https://www.gartner.com/en/newsroom/press-releases/2025-03-31-gartner-forecasts-worldwide-genai-spending-to-reach-644-billion-in-2025). Yet an [MIT study](https://mlq.ai/media/quarterly_decks/v0.1_State_of_AI_in_Business_2025_Report.pdf) found that only 5% were able to deliver ROI. That leaves $238 billion in failed implementations — more than the entire GDP of New Zealand or Greece. An amount of money that could run Portugal's entire economy for most of a year, essentially vanished with nothing to show for it.

The statistics are shocking, but misleading if taken at face value. If 95% of the projects failed, the first instinct is to blame the technology. However, the same study shows that 5% of the projects succeeded, which means the technology does work — but many organizations cannot explain how to harness this new technology. They launch pilots without explaining what success looks like, try to replicate the demo into their own messy environment, measure outputs without explaining business impact, and abandon projects without explaining what went wrong.  

`It isn’t AI that needs rescuing but the explanations around it.`

---

## The Study

The MIT study revealed four patterns that define the **GenAI Divide**:  

- **Limited Disruption:** Only 2 of 8 major sectors show meaningful structural change.  
- **Enterprise Paradox:** Big firms lead in pilot volume but lag in scale-up.  
- **Investment Bias:** Budgets favor visible, top-line functions over high-ROI back office.  
- **Implementation Advantage:** External partnerships see twice the success rate of internal builds.  

And the core barrier to scaling is not infrastructure, regulation, or talent. It is **learning**. Most GenAI systems do not retain feedback, adapt to context, or improve over time.  

---

## What is Learning?

When we say *“AI learns”*, what exactly is happening?  

`The model itself is frozen — GPT-5, Claude, or any LLM does not update from your prompts.`  

Every interaction starts from scratch. The best answer today does not improve tomorrow’s. The worst mistake today does not prevent it from happening again. So where is the learning?  

---

## Three Types of “Learning” (That Mostly Don’t Happen)

1. **Model Learning (doesn’t exist in production):**  
   LLMs are trained, then deployed and frozen.  
   `The best interaction teaches the model nothing. The worst interaction teaches it nothing.`  

2. **System Learning (the promise of RAG and fine-tuning):**  
   - **RAG (Retrieval Augmented Generation):** Adds documents, but not true understanding.  
   - **Fine-tuning:** Expensive, risky, and frozen in time.  
   - **Prompt Engineering:** Drifts, and no single “perfect” prompt exists.  

3. **Organizational Learning:**  
   If the AI doesn’t learn and the system barely adapts, then it is the humans and organizations around the AI that must learn.  

---

## The Agentic AI Paradox

Now companies are betting on **Agentic AI** — the AI that can take actions, not only generate text. But if we can’t explain why the text output was wrong, how will we explain why the *action* was wrong, let alone fix it the next time?  

For example, if an agent books the wrong flight, will the next attempt be correct? Or will we just depend on probability and hope?  

---

## The Questions This Raises

- If learning doesn’t happen in the model, where should it happen?  
- Can you have “intelligent” systems that never actually learn?  
- When everyone uses the same frozen LLM, where lies the competitive advantage?  
- How do you improve something that can’t improve itself?  

Maybe the problem is more philosophical than technical. We’re trying to implement “learning machines” in organizations that themselves don’t have mechanisms to learn from implementation.  

`What would it mean to build learning around AI, rather than expecting learning from AI?`

---

## The Learning We Actually Build

The successful 5% are not failing. They’re generating real ROI. So what are they actually doing?  

---

### A Typical Implementation Journey

From the outside, **RAG** or **Agentic AI** sounds like a self-learning architecture.  
In reality, they are carefully designed, sophisticated solutions — configured and maintained by humans at every step.  

It starts with curating knowledge bases, PDFs, support tickets, screenshots, even tribal knowledge. None of it is plug-and-play. Everything must be cleaned, scaffolded, and labeled before being embedded into a vector database. And every use case may require different curation.  

`RAG does not learn documents. Humans prepare them.`  

Next comes the **knowledge map**, where domain concepts are clearly defined with synonyms and relationships. Without this, LLMs happily create new relationships that don’t exist and hallucinate.  

`LLMs do not know your domain. Humans encode domain anchors.`  

Then comes **retrieval**, tuned after understanding user intent. Queries must be mapped to anchors, documents fetched, and results re-ranked so new content outranks old, duplicates are removed, and shallow entries don’t bury detailed ones.  

`RAG retrieval does not self-correct. Every adjustment is a human choice.`  

On top sits **prompt engineering**. The model must be told exactly how to behave, when to escalate to tools, how to consume outputs. When prompts fail, they must be rewritten.  

`LLMs do not adapt their own behavior. Humans rewrite prompts when they break.`  

**Agentic AI** adds orchestration, chaining reasoning steps, calling APIs, or executing actions. But if an agent fails, the next attempt starts from scratch. The only improvement comes when humans redesign the logic.  

`Agentic AI does not learn workflows. Humans hard-code them.`  

---

### Invisible Labor

What looks like intelligence is in fact invisible labor:  

- Cleaning messy documents into structured data  
- Writing domain concepts into knowledge maps  
- Tuning retrieval and re-ranking after bad outputs  
- Rewriting prompts after contradictions  
- Adding guardrails and validation checks  

The model remains frozen. The scaffolding evolves only because people push it forward.  

---

## The Philosophical Question

When organizations build elaborate processes around frozen AI, where does the intelligence reside? In the model, or in the humans and systems that guide it?  

The successful 5% do not have “learning AI.” They have **learning organizations** that figured out the real manual work behind frozen intelligence.  

And maybe that’s enough. Or maybe it’s something else entirely — a new kind of “learning” or “intelligence” we haven’t yet defined.  

---

## Conclusion

The $238 billion question isn’t whether AI can learn — it clearly can’t.  

`The 'intelligence' in our AI systems is actually human intelligence, carefully maintained through invisible labor.`  

The successful 5% haven’t built learning machines. They’ve built machines that require constant human learning to function.  

Maybe that’s enough.  
Or maybe we’re building something we haven’t yet identified — intelligence that exists not in the model, not in the system, but in the gap between human and machine.  
