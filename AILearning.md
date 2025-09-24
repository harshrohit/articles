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

Last year companies spent around $250 billion on AI ([Gartner forecast](https://www.gartner.com/en/newsroom/press-releases/2025-03-31-gartner-forecasts-worldwide-genai-spending-to-reach-644-billion-in-2025)). Yet an [MIT study](https://mlq.ai/media/quarterly_decks/v0.1_State_of_AI_in_Business_2025_Report.pdf) found that only 5% were able to deliver ROI. That leaves $238 billion in failed implementations - more than the entire GDP of New Zealand or Greece. An amount of money that could run Portugal's entire economy for most of a year, essentially vanished with nothing to show for it.

The statistics are shocking, but misleading if taken at face value. If 95% of the projects failed, the first instinct is to blame the technology. However, the same study shows that 5% of the projects succeeded, which means the technology does work, but many organizations cannot explain how to harness this new technology. They launch pilots without explaining what success looks like, try to replicate the demo into their own messy environment, they measure outputs without explaining their business impact, and they abandon projects without explaining what went wrong.

It isn't AI that needs rescuing but the explanations around it.

## The Study

MIT study revealed four patterns that define the GenAI Divide:

- **Limited Disruption**: Only 2 of 8 major sectors show meaningful structural change.
- **Enterprise Paradox**: Big firms lead in pilot volume but lag in scale-up
- **Investment Bias**: Budgets favor visible, top-line functions over high-ROI back office
- **Implementation advantage**: External partnerships see twice the success rate of internal builds.

And the core barrier to scaling is not infrastructure, regulation, or talent. **It is learning.** Most GenAI systems do not retain feedback, adapt to context, or improve over time.

And this raises the fundamental question.

## What is Learning

When we say "AI learns", what exactly is learning? The model itself is frozen - GPT-5, Claude does not update from your prompts, one interaction does not make the next interaction smarter. Every interaction starts from the scratch. So where exactly is learning?

### Three Types of "Learning" (that mostly don't happen)

1. **Model Learning (doesn't exist in production)**: LLMs are trained, then deployed and frozen. They didn't learn from the interactions by themselves. The best interaction with the customer does not make LLM learn anything, and so does the worst interaction.

2. **System Learning (The promise of RAG/fine tuning)**: Companies try to make learning through:
   - **RAG (Retrieval Augmented Generation)** - but this just add the documents, and not the understanding or learning.
   - **Fine-Tuning** - Expensive, risky and frozen in time.
   - **Prompt Engineering**: the prompts drift and there is no guarantee which one is the perfect.

3. **Organizational Learning**: If the AI doesn't learn and the system barely adapts, who is supposed to be learning

## The Agentic AI Paradox

Now companies are betting on "Agentic AI", the AI that can take actions, not only generate text. But if we can't explain why the text output was wrong, then how we will explain where the agent went wrong and more importantly fix the next interaction? For example, an agent booking the wrong flight, will the next interaction will be of the right booking or we will just hope and depends on the probability of the Agentic AI.

### Questions this raises:

- If learning doesn't happen in the model, where should it happen?
- Can you have "intelligent" systems that never actually learn?
- When everyone uses the same frozen LLM, where lies the competitive advantage?
- How will you improve something that can't improve itself?

Maybe the problem is more philosophical than technical. We're trying to implement "learning machines" in organizations that themselves don't have mechanisms to learn from implementation.

**What would it mean to build learning around AI rather than expecting learning from AI?**

## The Learning We Actually Build

The successful 5% are not failing, but they're generating real ROI. So what are they actually doing?

### A Typical Implementation Journey

"RAG" or "Agentic AI" are carefully designed, sophisticated solutions, configured and maintained by humans at every step.

It starts with curating knowledge base, PDFs, support tickets, screenshots, tribal knowledge and so on. Once all is collected, they are not plug and play for the LLM, they need cleaning, scaffolding, and labeling the content so that it can be embedded into a vector database. And every use case may require different kind of curation.

Next, comes the knowledge map, each domain concept is written in a way where the definitions, synonyms, and relationships are clearly defined. Without this, LLM can happily create new relationships which may not even exist and hallucinate.

Next, is the retrieval which needs to be tuned after understanding the user's intent. Once the user asks the query, the knowledge base has to be retrieved based on the knowledge anchors identified in the user's query. Based on the knowledge anchors, the detailed knowledge base is fetched. Once the documents are fetched, it needs to be re-ranked so recent documents outrank old ones, duplicates are removed, and shallow entries don't drown out detailed ones. This tuning is manual, trial-and-error, and continuous.

On top of this sits the Prompt Engineering. The model exactly needs to be told how it should behave, how to identify the knowledge is not sufficient and when to trigger the tools, along with the definition of the tools and the input and how the output should be consumed. And when the prompts failed, they need to be re-written. Nothing about the model adapts on its own.

Agentic AI adds another complexity which makes the system capable to execute actions. Each "agent" is a set of scripts written to orchestrate queries, call APIs, or chain reasoning steps. If it fails, the next attempt starts again from scratch. The only improvement comes if humans redesign the agent logic.

The model remains frozen. The scaffolding around it evolves and only because people push it forward.

## The Philosophical Question

When organization build elaborate processes around frozen AI, where does the intelligence reside. In the AI or in the human systems that guides it?

The successful 5% do not have "learning AI" but "learning organizations" that have figured out the real manual work behind the frozen intelligence. And may be that's enough, or may be its something entirely different what we call as "Learning" or "Intelligence" in general.

## Conclusion

The $238 billion question isn't whether AI can learn - it clearly can't. It's whether we are willing to acknowledge that the 'intelligence' in our AI systems is actually human intelligence, carefully maintained through invisible labor. The successful 5% haven't built learning machines. They've built machines that require constant human learning to function.

Maybe that's enough. Or maybe we are building something we have not yet identified, intelligence that exists not in the model, not in the system, but in the gap between human and machine.
