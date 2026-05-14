---
layout: default
title: "Horizon Summary: 2026-05-14 (EN)"
date: 2026-05-14
lang: en
---

> From 24 items, 8 important content pieces were selected

---

1. [Needle: 26M Parameter Model for Tool Calling](#item-1) ⭐️ 8.0/10
2. [The Emacsification of Software](#item-2) ⭐️ 7.0/10
3. [Twin brothers wipe 96 government databases minutes after being fired](#item-3) ⭐️ 7.0/10
4. [CSP Allow-list Experiment Demonstrates Novel Bypass Technique](#item-4) ⭐️ 7.0/10
5. [S-100 Virtual Workbench Simulates Classic 1970s Computer Systems](#item-5) ⭐️ 6.0/10
6. [Boris Mann Questions AI Agent Count Meaningfulness](#item-6) ⭐️ 6.0/10
7. [Hashimoto: Enterprise Tech Decisions Driven by Job Security](#item-7) ⭐️ 6.0/10
8. [LLM CLI tool adds reasoning token support](#item-8) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Needle: 26M Parameter Model for Tool Calling](https://github.com/cactus-compute/needle) ⭐️ 8.0/10

Cactus team open-sourced Needle, a 26 million parameter model distilled from Gemini that specializes in function calling and tool use, achieving 6000 tokens/s prefill and 1200 tokens/s decode on consumer devices. The model uses Simple Attention Networks architecture with no MLPs, relying instead on attention and gating mechanisms. This represents a major breakthrough in AI efficiency by demonstrating that complex tool-calling capabilities can be distilled into a tiny model that runs on budget phones and consumer devices, making agentic AI accessible on edge hardware. The approach challenges conventional wisdom about needing large models for sophisticated AI functions. The model achieved 200B token pretraining on 16 TPU v6e chips in 27 hours, followed by 2B token post-training on synthetic function-calling data in 45 minutes. It outperforms larger models like FunctionGemma-270M and Qwen-0.6B on single-shot function calling tasks while being significantly smaller.

hackernews · HenryNdubuaku · May 12, 18:03 · [Discussion](https://news.ycombinator.com/item?id=48111896)

**Background**: Function calling (or tool calling) enables AI models to interface with external systems and access real-time data beyond their training data. Traditional approaches use large models with MLP (Multi-Layer Perceptron) components, but Needle demonstrates that for tool-calling tasks, cross-attention mechanisms are sufficient without the computational overhead of MLPs. Simple Attention Networks eliminate MLP blocks entirely, using only attention and gating operations.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/cactus-compute/needle/blob/main/docs/simple_attention_networks.md">needle/docs/simple_attention_networks.md at main · cactus-compute/needle</a></li>
<li><a href="https://developers.openai.com/api/docs/guides/function-calling">Function calling | OpenAI API</a></li>
<li><a href="https://www.promptingguide.ai/applications/function_calling">Function Calling with LLMs | Prompt Engineering Guide</a></li>

</ul>
</details>

**Discussion**: Community discussions focused on the model's discriminatory power for tool selection, concerns about Google's potential response to distillation efforts, and comparisons with existing approaches. Some users noted that removing MLPs aligns with other recent research showing similar findings for models with external knowledge sources.

**Tags**: `#AI`, `#model-distillation`, `#function-calling`, `#on-device-AI`, `#efficiency`

---

<a id="item-2"></a>
## [The Emacsification of Software](https://sockpuppet.org/blog/2026/05/12/emacsification/) ⭐️ 7.0/10

A new blog post argues that modern LLMs enable individuals to build highly customized personal software solutions rather than relying on generic applications, drawing parallels to Emacs's philosophy of extensive customization. The post suggests that AI tools make it easier to create personal software tailored to individual needs. This represents a potential shift from mass-market software consumption to personalized software creation, where individuals can build their own podcast apps, note-taking tools, and other utilities using LLMs. The trend could democratize software development and reduce dependency on commercial applications. The concept builds on Emacs's extensibility model where users create their own 'dot emacs' configuration files, now extended to entire personal software ecosystems. LLMs like Claude can produce replacement-grade software for common applications, though not necessarily the most competitive globally.

hackernews · rdslw · May 13, 07:06 · [Discussion](https://news.ycombinator.com/item?id=48118727)

**Background**: Emacs is a highly extensible and customizable text editor that has been around since the 1970s, known for its philosophy of allowing users to customize every aspect through Emacs Lisp programming. The term 'Emacsification' refers to the approach of creating highly personalized, customizable software environments. Large language models (LLMs) are AI systems capable of understanding and generating human-like text, which can now assist in coding and software development tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.masteringemacs.org/article/beginners-guide-to-emacs">An Emacs Tutorial: Beginner's Guide to Emacs - Mastering Emacs</a></li>
<li><a href="https://symflower.com/en/company/blog/2024/ai-tools-software-testing/">The best LLM tools for software development</a></li>
<li><a href="https://anythingllm.com/">AnythingLLM | The all-in-one AI application for everyone</a></li>

</ul>
</details>

**Discussion**: Commenters agree that LLMs enable personal software creation, citing examples like podcast apps, note-taking tools, and feed readers that can be built with AI assistance. However, some express concerns about the brittleness of customized solutions, noting that personal Emacs configurations can become difficult to maintain across different platforms. There's also historical context suggesting this returns to the original vision of personal computing where everyone would program their own solutions.

**Tags**: `#software-development`, `#customization`, `#LLM-tools`, `#personal-software`, `#Emacs`

---

<a id="item-3"></a>
## [Twin brothers wipe 96 government databases minutes after being fired](https://arstechnica.com/tech-policy/2026/05/drop-database-what-not-to-do-after-losing-an-it-job/) ⭐️ 7.0/10

Two recently-fired twin employees systematically destroyed 96 government databases including Department of Homeland Security systems, with one brother executing 'DROP DATABASE dhsproddb' command at 4:58 PM and asking AI tools how to clear system logs afterward. This incident highlights critical cybersecurity vulnerabilities in government IT systems and demonstrates major failures in access control protocols during employee termination, affecting sensitive national security infrastructure. The brothers retained database administrator privileges after termination and used DROP DATABASE commands to destroy systems, later attempting to cover their tracks by asking AI tools how to clear SQL server logs and event applications.

hackernews · jnord · May 12, 22:28 · [Discussion](https://news.ycombinator.com/item?id=48115438)

**Background**: Database security involves implementing access controls, authentication mechanisms, and privilege management to protect sensitive information from unauthorized access or destruction. Government systems typically require mandatory access control (MAC) protocols where users can only access data matching their security clearance level. Proper employee termination procedures should immediately revoke all system access upon job conclusion to prevent security breaches. The incident reveals failures in these fundamental security practices, allowing terminated employees to maintain administrative privileges to critical systems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Database_security">Database security - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Access_control">Access control - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mandatory_access_control">Mandatory access control - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community discussion focuses on the balance between security protocols and humane employment practices, with some noting that employees with excessive database privileges pose risks even when employed. Commenters questioned how non-Americans were granted access to sensitive government systems and expressed amusement at the incompetence of the perpetrators seeking AI help to cover their tracks.

**Tags**: `#cybersecurity`, `#database-security`, `#access-control`, `#incident-response`, `#government-security`

---

<a id="item-4"></a>
## [CSP Allow-list Experiment Demonstrates Novel Bypass Technique](https://simonwillison.net/2026/May/13/csp-allow/#atom-everything) ⭐️ 7.0/10

Simon Willison created a proof-of-concept tool that demonstrates how to work around Content Security Policy restrictions by loading apps in sandboxed iframes and intercepting blocked fetch requests, allowing users to dynamically update CSP allow-lists through a custom fetch implementation. This experiment highlights critical security implications for CSP implementations while demonstrating potential legitimate use cases for dynamic allow-list management in controlled environments, revealing fundamental limitations in current CSP protection mechanisms. The technique uses sandboxed iframes with custom fetch() implementations that intercept CSP errors and pass them to the parent window, which prompts users to add domains to the allow-list, built using GPT-5.5 xhigh in the Codex desktop app.

rss · Simon Willison · May 13, 04:50

**Background**: Content Security Policy (CSP) is a security standard designed to prevent cross-site scripting (XSS), clickjacking, and other code injection attacks by controlling which resources can be loaded on a web page. The sandbox directive creates a restricted environment for iframes, limiting their capabilities to prevent malicious behavior. The connect-src directive specifically controls where browsers can fetch data from, making it a key target for this bypass technique.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Content_Security_Policy">Content Security Policy - Wikipedia</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Reference/Headers/Content-Security-Policy/sandbox">Content - Security - Policy : sandbox directive - HTTP | MDN</a></li>
<li><a href="https://cheatsheetseries.owasp.org/cheatsheets/Content_Security_Policy_Cheat_Sheet.html">Content Security Policy - OWASP Cheat Sheet Series Content Security Policy Level 3 javascript - fetch () does not send request (CSP issue ... Fetch Standard CSP connect-src Explained - Content-Security-Policy Network Request Interception | Kaliiiiiiiiii-Vinyzu ...</a></li>

</ul>
</details>

**Tags**: `#csp`, `#security`, `#web-development`, `#sandbox`, `#content-security-policy`

---

<a id="item-5"></a>
## [S-100 Virtual Workbench Simulates Classic 1970s Computer Systems](https://grantmestrength.github.io/S100/) ⭐️ 6.0/10

A new virtual workbench has been created that simulates classic S-100 bus computer systems from the 1970s, including platforms like the IMSAI-8080, allowing users to experience vintage computing environments and run early software. This project preserves computing history by making vintage S-100 systems accessible to enthusiasts without requiring expensive physical hardware, connecting modern users to the foundational era of personal computing in the mid-1970s. The virtual workbench recreates the S-100 bus architecture that was the first industry standard bus for microcomputers, supporting systems that ran CP/M operating systems and early programming languages like BASIC and C.

hackernews · rbanffy · May 13, 15:52 · [Discussion](https://news.ycombinator.com/item?id=48123546)

**Background**: The S-100 bus was introduced with the MITS Altair 8800 in 1975 and became the standard for early personal computers. It was a 100-pin passive backplane system that allowed various CPU, memory, and I/O cards to be plugged in, forming complete computer systems. The IMSAI-8080 was a popular clone of the Altair 8800 released in late 1975, based on the Intel 8080 processor and S-100 bus architecture. These systems were foundational to the personal computer revolution and ran early operating systems like CP/M.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/S-100_bus">S-100 bus - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/IMSAI_8080">IMSAI 8080 - Wikipedia</a></li>
<li><a href="https://www.retrotechnology.com/herbs_stuff/s100bus.html">S-100 and IEEE-696 Bus List - retrotechnology.com S100 Computers - History Full text of "The S-100 and other micro buses" - Archive.org S-100 Computer (1) - Computer - Computing History The history of industrial I/O buses: S-100, ISA, PC104 ...</a></li>

</ul>
</details>

**Discussion**: The community response shows strong nostalgia among vintage computing enthusiasts, with users sharing personal memories of working with S-100 systems and early programming experiences. Commenters expressed excitement about running classic software like Microsoft Advanced Basic and playing games such as Star Trek on emulated systems.

**Tags**: `#retro-computing`, `#vintage-hardware`, `#emulation`, `#S-100-bus`, `#historical-computing`

---

<a id="item-6"></a>
## [Boris Mann Questions AI Agent Count Meaningfulness](https://simonwillison.net/2026/May/13/boris-mann/#atom-everything) ⭐️ 6.0/10

Boris Mann made a quote questioning the meaningfulness of counting AI agents by comparing '11 AI agents' to mundane tools like spreadsheets and browser tabs. The quote highlights that saying 'I have 11 AI agents' is semantically equivalent to saying 'I have 11 spreadsheets' or 'I have 11 browser tabs.' This perspective challenges the current AI agent hype cycle by pointing out that agent counts without context are meaningless metrics. It highlights the need for more substantive evaluation criteria rather than simple numerical counts when assessing AI agent capabilities. The quote emphasizes that the term 'AI agents' lacks specificity when used merely as a count, similar to how counting spreadsheets or browser tabs doesn't convey meaningful information about productivity or capability. The criticism targets the semantic emptiness of agent numbers without understanding their actual functions or sophistication levels.

rss · Simon Willison · May 13, 16:15

**Background**: AI agents are computational systems designed to act autonomously, receiving input from users and choosing appropriate actions to achieve established goals, unlike traditional software that simply follows predetermined commands. The distinction between AI agents and traditional software lies in autonomy, learning capabilities, and adaptive behavior, making simple counts potentially misleading when evaluating their actual utility.

<details><summary>References</summary>
<ul>
<li><a href="https://mahalakshmitechcampus.com/blogs/what-are-ai-agents-definition-how-they-work-real-world-examples/">What are AI Agents : Definition , How... - Mahalakshmi Tech Campus</a></li>
<li><a href="https://kritimyantra.com/blogs/understanding-ai-agents-the-simple-guide-youve-been-waiting-for">Understanding AI Agents : The Simple Guide... - Kritimyantra | Blog</a></li>

</ul>
</details>

**Tags**: `#ai-agents`, `#ai`, `#agent-definitions`, `#criticism`, `#productivity`

---

<a id="item-7"></a>
## [Hashimoto: Enterprise Tech Decisions Driven by Job Security](https://simonwillison.net/2026/May/12/mitchell-hashimoto/#atom-everything) ⭐️ 6.0/10

Mitchell Hashimoto observed that 90% of technical decision makers prioritize avoiding getting fired over innovation, following analyst-driven trends like Gartner and McKinsey recommendations rather than making bold technical choices. This insight reveals why enterprise software markets often favor established vendors over innovative solutions, explaining market dynamics where analyst reports drive purchasing decisions more than technical merit. Hashimoto distinguishes between technical decision makers who work 9-to-5 and weekend developers, noting that enterprise buyers choose 'defensible' products based on analyst reports rather than technical excellence.

rss · Simon Willison · May 12, 22:21

**Background**: Technical Decision Makers (TDMs) are professionals responsible for evaluating and selecting technology solutions within organizations. Research firms like Gartner and McKinsey publish influential reports that guide enterprise purchasing decisions, creating a market where analyst recommendations carry significant weight in corporate boardrooms.

<details><summary>References</summary>
<ul>
<li><a href="https://www.acronymfinder.com/Technical-Decision-Maker-(various-companies)-(TDM).html">TDM - Technical Decision Maker (various companies ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Gartner">Gartner - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/McKinsey_&_Company">McKinsey & Company - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#enterprise`, `#decision-making`, `#technical-leadership`, `#industry-insights`

---

<a id="item-8"></a>
## [LLM CLI tool adds reasoning token support](https://simonwillison.net/2026/May/12/llm/#atom-everything) ⭐️ 6.0/10

LLM CLI tool version 0.32a2 introduces support for viewing reasoning tokens from OpenAI's advanced models using the new /v1/responses endpoint, displaying them in different colors to distinguish from standard output. This enhancement provides transparency into how advanced AI models like GPT-5 class reason through problems, allowing developers to better understand model decision-making processes and debug complex interactions. The new /v1/responses endpoint replaces /v1/chat/completions for reasoning-capable models and enables interleaved reasoning across tool calls, with users able to hide reasoning tokens using the -R or --hide-reasoning flags.

rss · Simon Willison · May 12, 17:45

**Background**: Reasoning tokens are internal processing steps that advanced AI models use before producing final responses, helping them plan, use tools effectively, and solve complex multi-step tasks. The OpenAI /v1/responses endpoint was designed specifically for reasoning models like GPT-5 to provide better integration between chat and assistant capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.openai.com/api/docs/guides/reasoning">Reasoning models | OpenAI API</a></li>
<li><a href="https://platform.openai.com/docs/guides/migrate-to-responses">Migrate to the Responses API | OpenAI API</a></li>
<li><a href="https://developers.openai.com/blog/responses-api">Why we built the Responses API | OpenAI Developers</a></li>

</ul>
</details>

**Tags**: `#llm`, `#openai`, `#cli-tool`, `#reasoning-tokens`, `#gpt`

---