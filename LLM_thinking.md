---
title: "The Day \"Just Ask ChatGPT\" Became the Only Answer"
description: "We've replaced thinking with prompting, understanding with copy-pasting, and learning with asking ChatGPT — and we're calling it productivity."
date: "2025-09-03"
author: "Rohit Harsh"
tags: ["LLM", "Thinking", "Apple", "PromptEngineering"]
icon: "🔄"
gradient: "from-blue-100 to-cyan-100"
patternGradient: "from-blue-200/50 to-cyan-200/50"
---

# The Day "Just Ask ChatGPT" Became the Only Answer

Recently, I needed to write a query to pull the data in BigQuery.

A couple of years back, I would have gone to Google, searched the error, read the schema guide or maybe pinged a teammate for help. 

This time? I copied the error, pasted it into ChatGPT, got a solution, copied it back. It worked. I moved on.

I never understood why it failed. I never learned what fixed it. All I cared was the solution. 

And this made me realize that somewhere along the way, I stopped thinking through the problem and I think many of us did. 

---

## The Truth

The LLMs do not think, but what is more worrisome is that **we might start doing the same**. 

Earlier, when we got a problem, we would pull the logs, trace the event sequence line by line, and compare the working and non-working scenarios. Once we understood the flow, we matched it against the code to identify the logic that caused the issue. We often added verbose logging to trace every step, explore deeper, and understand exactly how the system worked. And the verbose logging was not only the debugging tool, but often the way we learned how the system _really_ worked. 

Today we go straight to ChatGPT, not for help to think through the issue, but to avoid thinking entirely. We want the quick answer, not the understanding of the concepts.  We copy the error and then the code, and ChatGPT diagnoses everything and tell where lies the problem and its all done. 

And all of this feels so efficient, so smart, and the illusion that we are getting more done than ever.

The reality: We are just becoming very efficient in not understanding our own work. 

---

## The Cognitive Decline

Like muscles, our cognitive skills weaken when we don't use them. Relying on AI for every task, question, or problem can quietly erode our ability to reason, think creatively, and solve things ourselves.

A recent [study](https://www.pnas.org/doi/abs/10.1073/pnas.2422633122?doi=10.1073%2Fpnas.2422633122&mod=ANLink) on students learning in math education, gives us an unsettling glimpse of this phenomenon. Students using ChatGPT performed **48%** better than their counterparts who did not have access to the AI. The same group of students performed **17%** lower when the AI access is taken away. However, the carefully designed safeguards, especially asking the AI tutor to provide teacher-designed hints instead of giving away answers, can mitigate these negative effects. 

But it’s not only about losing practice with problems, we are losing something more fundamental.  
Another [study](https://www.psychologicalscience.org/news/releases/want-to-solve-a-problem-dont-just-use-your-brains-but-your-bodies-too.html) reminds us that problem solving is not just the work of the brain but also our body. We use our hands, our posture, even our gestures to think, and, when we delegate to AI too quickly, we skip this process and lose the deeper engagement. Remember the scribbling on the paper, mapping the system on the white boards? Or just going out for a walk, and out of nowhere the solution just appears. That’s your brain and your body thinking together to get to the solution. Copy pasting from ChatGPT takes away all of that.  

---

## The Day Apple Said No (And Why It Matters)

While everyone rushed to build chatbots and put AI on everything, Apple published two papers essentially saying: "These things can't actually reason, and we can prove it."

They tested the latest "reasoning" models, the ones that supposedly "think step-by-step" and "show their work." The study shows that these models face complete accuracy collapse when problems get complex. Even worse: they *appear* to reason more with harder problems, but then suddenly give up, despite having plenty of tokens left to think.

On simple tasks, regular LLMs actually outperform these "reasoning" models. The entire step-by-step thinking process is an illusion.

Most notably, Apple observed LLM's limitations in performing exact computation; these models can make 100 correct moves in Tower of Hanoi, but couldn't get past 5 moves in the River Crossing puzzle. Even when given the exact algorithm, these models couldn't improve. They are pattern matching until they hit the wall. 

Read the studies yourself:
- [GSM-Symbolic: Understanding the Limitations of Mathematical Reasoning in Large Language Models](https://machinelearning.apple.com/research/gsm-symbolic)
- [The Illusion of Thinking](https://machinelearning.apple.com/research/illusion-of-thinking)

What makes this worse is that despite these fundamental limitations, every company is shipping half-baked AI features, for the problems which are far beyond AI reach. This is not a work of innovation but a fear of being seen as "behind." They're adding chatbots that don't work, AI assistants that nobody uses, all to tick a box that says "we have AI."

And unless you're OpenAI, Google, or Anthropic, unless you're spending billions on compute and training, you are not in the AI business. You are just another customer, another subscriber or just another monthly payment to use someone else's models.

The entire industry is racing to integrate technology they don't control, can't improve, and barely understand. All to avoid looking outdated in earnings calls. 

But in this mad rush, they're also losing their actual competitive advantages: engineers who understand their own code, teams that can debug without AI, and the ability to solve problems that don't have Stack Overflow answers.

---

## The Statistical Average

We assume AI helps us to be more creative and think differently. According to the [study](https://www.media.mit.edu/articles/a-i-is-homogenizing-our-thoughts/)  by MIT, researchers split more than 50 Boston-area university students into three groups: one using only their own thinking, one with Google access, and one with ChatGPT. All were given the topic “Must our achievements benefit others in order to make us truly happy” to write SAT-style essays.  

The text produced by the LLM users tended to converge on common words and ideas. SAT prompts are designed to trigger various narratives from the writers, however, the use of AI has a homogenizing effect. The output was very similar for the different people who were asked to talk about their writings on different days. 

For example, for the question related to philanthropy (“Should people who are more fortunate than others have more of a moral obligation to help those who are less fortunate?”), all the ChatGPT users said yes. No one with ChatGPT played a devil’s advocate, no one explored counter arguments.

But in the other group, people had more mixed opinions. Some even questioned the idea of philanthropy, raising concerns or offering critiques that didn’t come up in the AI-written answers. 

Hence, when you think you are getting an AI-based personal assistant, in reality you are getting homogenized thought, filtered through the same training data, the same RLHF, the same guardrails. Or in other words, you are getting the statistical average of the internet's opinions, packaged as personalized help. 

---

## What You Should Actually Do

**Swap roles with AI**: Tell the AI that “I am the assistant, and you are the human, Ask me questions”. When the AI asks you a question, force yourself to explain the concept. This may seem silly at first, but you will be amazed to realize how much you know or how much you don’t. It is one of the fastest ways to move from _reading answer_ to _truly learning_. 

**The Explanation Test**: Instead of saying, "Give me the answer", try saying "Guide me through the problem so I can solve this on my own". Request step-by-step explanations. Once the answer is there, close the chat window and try to explain it to test the retention. 

**Solve Problems Backwards**: When facing a unique issue or a question, start by assuming the AI's first suggestion is wrong. Work backwards to understand why. You'll often find it was right, but now you'll know WHY, and more importantly, you will spot when it is confidently wrong next time. 

---

## The Choice

We're at an inflection point. Not for AI but for us.

Either we maintain our ability to think and understand what these tools actually are. Brilliant pattern matchers that simulate understanding without possessing it. Or we atrophy into prompt engineers for systems we don't comprehend, solving problems we can't actually solve, knowing things we don't really know.

"Just ask ChatGPT" has become the default answer to everything. But what happens when ChatGPT doesn't know? What happens when it's confidently wrong? What happens when the problem needs actual understanding, not pattern matching?

More importantly: What happens when you can no longer tell the difference?

The machines aren't going to start thinking.

The question is: Will we stop?

---

*P.S.: If you used AI to read, summarize, or respond to this article, you've proven my point. Notice what just happened: You outsourced your engagement with an argument about not outsourcing your thinking. Sit with that discomfort. That feeling? That's what thinking feels like.*
