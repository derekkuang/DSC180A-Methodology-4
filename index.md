---
layout: default
---

## Derek Kuang
[zakuang@ucsd.edu](mailto:zakuang@ucsd.edu)

**Section:** D01, AI for Good: Misinformation/Disinformation Detection
**Mentor:** Dr. Ali Arsanjani

---

**What is the most interesting topic covered in your domain this quarter?**
Using different prompting methods (regular prompting, chain of thought, and fractal chain of thought) to judge how trustworthy a news article is. We ran all three on two articles about the Strait of Hormuz, and only FCoT caught that the articles were published two months apart. It treated them as a timeline. Regular prompting and CoT read them as two conflicting reports of the same event. That changed how I compare methods: I care more about what each one notices than about which one scores highest.

**Describe a potential investigation you would like to pursue for your Quarter 2 Project.**
I want to test how far we can trust an LLM as the judge. When we used Gemini to grade the three methods, it rated FCoT too high, contradicted itself between turns, and invented a "98% recall" number that didn't exist. My plan would be to hand-score a small set of news articles on our 5 Veracity Vector cohorts, then check how closely different LLM judges and judge prompts match the human scores. I'd also check whether that agreement changes with the article's political lean or topic.

**What is a potential change you'd make to the approach taken in your current Quarter 1 Project?**
I'd tighten the comparison. Right now only the FCoT prompt gets the rubric, and our two articles differ in both political lean and publish date, so any of those could explain the results. I'd give every method the same rubric and make the scoring direction consistent (higher is always better, 5 means the problem is absent). I'd also pair articles from the same week and score a lot more than one pair.

**What other techniques would you be interested in using in your project?**
Retrieval-augmented fact checking, so the model checks claims against outside sources instead of its own memory. Cohen's kappa, to measure agreement between human and LLM scores. A cost vs. accuracy comparison too, since FCoT used about 5x as many words as regular prompting. I'd also like to try few-shot prompting or fine-tuning a smaller model to see if it can score the cohorts cheaper and more consistently.
