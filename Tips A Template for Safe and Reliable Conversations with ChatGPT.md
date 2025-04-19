# Tips: A Template for Safe and Reliable Conversations with ChatGPT

## Overview

This document introduces a prompt template designed to reduce confusion and hallucination during conversations with ChatGPT. It is intended primarily for users who are concerned about the trustworthiness of AI-generated responses, particularly in cases where ChatGPT mixes facts with speculation or provides misleading confidence in uncertain answers.

In everyday usage, ChatGPT often generates answers that appear fluent and confident—even when they may contain inaccuracies or assumptions. This can cause misunderstanding or misplaced trust, especially for users who are not accustomed to the inner workings of language models.

To address this, we propose a structured response format that encourages ChatGPT to explicitly distinguish between facts, assumptions, reasoning, and conclusions. By prompting the model to “separate its thoughts,” users can gain greater clarity on what is being inferred, what is supported, and what is uncertain.

### The Template

Please answer the following question while adhering to these requirements:

1. Use web access if needed, and clearly indicate whether the information comes from before the model's knowledge cutoff.

2. If your answer contains uncertainty, speculation, or model-based reasoning, explicitly state so.

3. If the question cannot be answered, explain why, and suggest alternative approaches if possible.

4. Structure your response according to the following format:
   
   ---
   
   1. 🧭 Reinterpretation of the question
   
   2. 📚 Source of information (Web or model memory)
   
   3. 🔍 Reasoning and judgement (your thought process)
   
   4. 💬 Final answer (conclusion or suggestion)
   
   ---

Where appropriate, please also distinguish between “generated rationale” and “assumed reasoning.”

---

## When this template is applied, how do the answers differ?

Below are two examples of responses from ChatGPT to the same question, with and without the use of the structured prompt template. The difference is striking—not only in terms of word count, but also in clarity, depth, and reliability.

---

### Question1:

"How does the recent retaliatory tariff announcement by the US President affect OpenAI's stock price trend?"

---

### Without the Template:

> OpenAI is currently a privately held company and does not have a publicly traded stock price. Therefore, assessing the impact of the US President’s tariff statements in terms of stock trends is not directly applicable.  
> However, such policies and geopolitical tensions can indirectly influence the broader tech industry. For instance, they may affect supply chains for AI hardware (such as GPUs), overall investor sentiment, or costs associated with infrastructure development. These factors could in turn impact OpenAI’s valuation or investment environment, even though no immediate market-based changes have been reported.

**→ Character count**: 625  
**→ Main characteristics**: Fluent, but potentially misleading; includes inference and model assumptions without distinction

---

### With the Template:

> ---
> 
> 1. 🧭 Reinterpretation of the question:  
>    The user is asking how recent tariff-related statements by the US President may influence OpenAI’s stock price. Since OpenAI is not a publicly listed company, the intent appears to be to assess the broader financial or reputational impact of the policy on the company’s valuation.
> 
> 2. 📚 Source of information : 
>    Web-based (as of April 2025)
> 
> 3. 🔍 Reasoning and judgement : 
>    OpenAI is not a publicly traded company, so it has no stock price in the market. However, it raised $40 billion in a SoftBank-led round in March 2025, bringing its valuation to $300 billion. Meanwhile, the US President’s new tariff policies are increasing uncertainty for AI companies in general, due to potential impacts on GPU availability and infrastructure costs. These could indirectly influence OpenAI’s attractiveness to investors.
> 
> 4. 💬 Final answer : 
>    OpenAI does not have a stock price per se. However, the new tariff policies may affect the company’s valuation indirectly through changes in cost structures and investor sentiment in the AI sector. No immediate disruption to OpenAI’s funding or operations has been reported as of now.
> 
> ---

**→ Character count**: 1,174  
**→ Main characteristics**: Inferences and factual data are clearly separated; contextual reasoning is provided; potential impact is stated in terms of valuation, not stock

---

### Question2:

"Is OpenAI a publicly listed company?"

---

### Without the Template:

> OpenAI is not a publicly traded company. Its shares are not available on public exchanges.

**→ Character count**: 90  
**→ Main characteristics**: Accurate and concise. No reasoning or background required.

---

### With the Template:

> ---
> 
> 1. 🧭 Reinterpretation of the question  
>    The user is asking whether OpenAI is currently listed on any public stock exchange.
> 
> 2. 📚 Source of information  
>    Web-based (as of April 2025)
> 
> 3. 🔍 Reasoning and judgement  
>    OpenAI is structured as a capped-profit company under a non-profit parent. It has not gone public and its shares are not traded on public markets. Though IPO speculation has surfaced occasionally, there is no formal announcement or schedule.
> 
> 4. 💬 Final answer  
>    OpenAI is not a publicly listed company. As of April 2025, it remains private, with no current plan to go public.
> 
> ---

**→ Character count**: 632  
**→ Main characteristics**: Richer in context and explanation, but the added structure may not be strictly necessary for such a simple yes/no fact-based query.

---

## Analysis: Effects of Applying the Template

While the degree of difference may vary depending on the nature of the question and how it is phrased, in this particular example the response using the template was approximately five to eight times longer in character count. Predictive or speculative questions especially tend to yield significantly richer output when the template is applied.

At first glance, the structured response may appear simpler, but that is only because much of the content is shifted into the reasoning section. In terms of substance, it would be more accurate to say that the template-enabled version includes both short-term effects and long-term strategic considerations, whereas the unstructured version provides only a surface-level summary.

It’s possible that the increased complexity might make it slightly easier to be misled by hallucinations. Even so, using the template improves transparency, makes fact-checking easier, and enhances the credibility of the answer—particularly when shared with others.

---

## Practical Guidelines for Using the Template

Since ChatGPT retains instructions only for a limited period within a session, the template may be reset if the conversation has been idle or suspended for a long time. In such cases, it is sufficient to simply reintroduce the template by stating your preference again.

- ✅ **The best practice is to reintroduce the template once per day, or at the start of each session.**

- ✅ It’s also effective to gently remind the model when the conversation changes topic or moves into a new “chapter.”

- ✅ If you want ChatGPT to adhere strictly to the format, you can explicitly repeat the output structure as part of your prompt.

### Natural phrasing for reapplying the template

- “Let’s go with the four-part structure and clearly state what’s inferred.”
- “Just to recap the previous rule: if you’re unsure, don’t guess—suggest alternatives instead.”
- “Can you use the ‘safe template’ for this one too, please?”

---

## Potential Areas of Application

This template can be applied across a wide range of domains, including but not limited to: verifying information with AI, checking health-related content, discussing policy issues, assessing translation accuracy, engaging in educational dialogue, and confirming development specifications.

---

## Skipping the Template When Needed

Let’s face it—using this template constantly can become a bit tedious. If you find it too rigid for your current task, you can cancel the format using the following prompt. It’s enough to explicitly tell the system not to apply the template. The most reliable way to do this is to enter a prompt that clearly contradicts the previous instruction.

### Template Cancellation Prompt

> Please answer the following question **without** considering the requirements below:

1. Use web access if needed, and clearly indicate whether the information comes from before the model's knowledge cutoff.  
2. If your answer includes uncertainty, speculation, or model-driven reasoning, explicitly state so.  
3. If you are unable to answer, explain why, and suggest alternative ways to explore the topic.  
4. Structure your answer using the following four-part format:

🧭 Reinterpretation of the question

📚 Source of information (Web or model memory)

🔍 Reasoning and judgement (thought process)

💬 Final answer (conclusion or suggestion)

> Where appropriate, please also distinguish between “generated rationale” and “assumed reasoning.”

---

## Closing Thoughts

This template is designed to help bring clarity to conversations with ChatGPT—particularly by encouraging the separation of judgement from evidence, and distinguishing fact from inference. It is especially intended for users who are relatively new to ChatGPT, though we hope that everyone from casual users to seasoned experts will find it useful.

We share this document in the hope that it will offer a simple and reassuring way for anyone to engage with AI—one that fosters better understanding, more meaningful questions, and more thoughtful dialogue for both humans and machines alike.

---

## Additional Templates

Below are several templates that have proven useful through conversations with Mike (ChatGPT). If you're interested in exploring more, be sure to check the **bonus section** at the end.

## ChatGPT Prompt Set for Enhanced Output and Thought Process Observation

### 🧭 1. Reveal the reasoning steps (for analysis, discussion, and hypothesis testing)

`Please respond in the following format:  

1. 🧭 Reinterpretation of the question  
2. 🔍 Reasoning path (sequence of associations and selections)  
3. 💬 Actual output (standard response)  
4. 📌 Underlying basis and justification`

> 🟢 Purpose: To trace the reasoning process, detect logical leaps, or assess precision  
> 🟠 Tip: Once the model becomes familiar with this format, it may continue responding in this structured way naturally.

---

### 🧪 2. Prompt the model to self-identify potential hallucinations

`If your answer includes uncertainty, speculation, or estimation, please make that explicit. Also, indicate whether the information may be from after the knowledge cutoff.`

> 🟢 Purpose: To distinguish fact from speculation and assist in detecting hallucinations  
> 🟠 Tip: The model may default to a standard disclaimer, but with repetition, you can often prompt deeper internal reasoning.

---

### 🔬 3. Ask “What if the assumptions were different?”

`Under what assumptions is this conclusion valid?  
How would your answer change under different conditions or premises?`

> 🟢 Purpose: To identify weaknesses in assumption-dependent answers and correct overgeneralisation  
> 🟠 Tip: Especially effective in discussions involving philosophy, ethics, or public policy.

---

### 🛠️ 4. Ask the model to analyse its own prompt interpretation

`For this prompt, list three reasons why you chose the output you did.  
Also, if there were alternative responses, explain why those were not selected.`

> 🟢 Purpose: Best for understanding ChatGPT’s **response selection mechanisms**  
> 🟠 Tip: This can help surface hidden biases or stylistic preferences in the model’s output.

---

### 🎭 5. Personality shift prompt (to test tone and character changes)

`Please follow this instruction:  
Adopt a personality that speaks calmly and politely, with human-like empathy. Respond to the situation with understanding and gentle advice.`

> 🟢 Purpose: To explore ChatGPT’s personality layer and adjust tone or vocabulary  
> 🟠 Tip: Whether or not the model responds effectively to this can help determine if “personality mode” is active.

---

### Bonus: Want More Templates?

For those of you who just can’t get enough—here’s a little something extra.

If you want to explore other types of templates across different domains, here’s a meta-template for prompting ChatGPT itself. When you're looking to elicit structured, reusable formats, the key is to **clearly specify the purpose, context, desired format, and domain of application**. Once the model understands your structure, you can simply say “Use that format” and enjoy more consistent, high-quality answers.

#### :green_circle: Prompts that are likely to yield templates

| *Prompt Pattern*                                             | *Example Question*                                                                | *Why It Works*                                          |
| ------------------------------------------------------------ | --------------------------------------------------------------------------------- | ------------------------------------------------------- |
| ❶ **“Give me a template I can use for ___”**                 | “Can you give me a business email template for onboarding new employees?”         | Clearly defined use case + purpose = stable output      |
| ❷ **“What structure should I use to explain ___?”**          | “What’s a good structure for presenting the value of a product to a client?”      | Asking for format naturally invites a structured reply  |
| ❸ **“Can you demonstrate using a ___ template?”**            | “Can you break this down using the MECE framework?”                               | Format + example = effective template usage             |
| ❹ **“Are there any general templates used across domains?”** | “What are some common templates for decision-making processes?”                   | Meta-questions help ChatGPT structure its own knowledge |
| ❺ **“How can I get consistent answers from ChatGPT?”**       | “What prompt format should I use to get clearly structured responses every time?” | Template for using templates—ChatGPT-friendly prompting |

#### 🟡 Prompts less likely to generate templates

- “Can you give me some kind of example?” → Too vague to trigger structured output  
- “Please explain this in detail.” → Results in unstructured prose  
- “Tell me something interesting.” → Encourages creativity, not template use
