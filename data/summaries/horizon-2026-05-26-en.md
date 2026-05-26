# Horizon Daily - 2026-05-26

> From 22 items, 7 important content pieces were selected

---

1. [Using AI to write better code more slowly](#item-1) ⭐️ 7.0/10
2. [Norway builds sovereign LLM with 2PB Huawei storage](#item-2) ⭐️ 7.0/10
3. [Microsoft Copilot Cowork Exfiltrates Files via Prompt Injection](#item-3) ⭐️ 7.0/10
4. [Armin Ronacher warns about AI-assisted bug reporting problems](#item-4) ⭐️ 7.0/10
5. [California moves to exempt Linux from its age-verification law after backlash](#item-5) ⭐️ 6.0/10
6. [Programming book sales decline signals shift in learning methods](#item-6) ⭐️ 6.0/10
7. [AI Converts Classic 1983 BASIC Game to Modern Web Version](#item-7) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Using AI to write better code more slowly](https://nolanlawson.com/2026/05/25/using-ai-to-write-better-code-more-slowly/) ⭐️ 7.0/10

Developers are adopting iterative AI workflows that use multiple AI models for code generation and review, trading development speed for improved code quality through back-and-forth interactions between different LLMs. This approach represents a shift from viewing AI as a speed multiplier to seeing it as a quality assurance tool, highlighting the trade-off between rapid development and code correctness that many developers now face. The workflow involves using different specialized models like Claude 4.7 Max for implementation and Codex GPT 5.5 for fast reviews, with multiple iteration cycles between generation and review phases to catch corner cases and improve output quality.

hackernews · signa11 · May 25, 23:16 · [Discussion](https://news.ycombinator.com/item?id=48272984)

**Background**: AI-assisted software development uses large language models (LLMs) and AI agents to help developers throughout the software development lifecycle, including code generation, debugging, testing, and documentation. LLM workflows typically involve chains of API calls that can be orchestrated to perform complex tasks through multiple steps and model interactions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI-assisted_software_development">AI-assisted software development - Wikipedia</a></li>
<li><a href="https://www.morphllm.com/llm-workflows">LLM Workflows: Patterns, Tools & Production Architecture ...</a></li>
<li><a href="https://docs.aws.amazon.com/prescriptive-guidance/latest/agentic-ai-patterns/llm-workflows.html">LLM workflows - AWS Prescriptive Guidance</a></li>

</ul>
</details>

**Discussion**: Developers report spending more time in LLM review/resolution loops than writing code manually, with some noting that AI code quality on initial attempts is often poor. Community members discuss using multiple specialized models iteratively, with concerns about AI potentially removing the thinking process from development work.

**Tags**: `#AI-assisted-development`, `#code-review`, `#LLM-workflows`, `#software-engineering`, `#developer-productivity`

---

<a id="item-2"></a>
## [Norway builds sovereign LLM with 2PB Huawei storage](https://www.blocksandfiles.com/flash/2026/05/22/norways-2-petabytes-of-huawei-flash-storage-and-llm-training/5244910) ⭐️ 7.0/10

Norway is developing a sovereign LLM using 2 petabytes of Huawei flash storage and local cultural data, arguing that countries need language-specific models to preserve their cultural knowledge. The project uses an HPE Cray Supercomputing EX system with 448 GPUs and 64,512 CPU cores. This represents a significant trend toward 'sovereign AI' where nations seek to develop independent AI capabilities to reduce dependence on foreign technology providers and maintain control over their cultural data. It highlights the growing recognition that global English-based models may not adequately represent local languages, history, and culture. The project faces skepticism regarding hardware adequacy, as the 448 GPU system may be insufficient for training a full-scale LLM compared to industry standards. The initiative specifically targets Norwegian language preservation and cultural knowledge representation that global models allegedly cannot provide.

hackernews · rbanffy · May 25, 19:37 · [Discussion](https://news.ycombinator.com/item?id=48270770)

**Background**: Sovereign AI refers to national strategies focused on developing independent artificial intelligence infrastructure, data control, and models to reduce dependence on foreign technology providers. Petabyte-scale storage systems are specialized infrastructures designed to manage massive datasets exceeding one quadrillion bytes, requiring distributed systems and sophisticated data management practices. Huawei provides enterprise storage solutions including hybrid flash storage systems for large-scale applications.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sovereign_AI_Fund">Sovereign AI Fund</a></li>
<li><a href="https://www.scality.com/topics/what-is-petabyte-storage/">What is Petabyte Storage? | Scality</a></li>
<li><a href="https://e.huawei.com/en/products/storage/hybrid-flash-storage">OceanStor Hybrid Flash Storage | Huawei Enterprise</a></li>

</ul>
</details>

**Discussion**: Community discussions include skepticism about the hardware adequacy, with critics noting that 448 GPUs may be insufficient for training a full LLM. Some question whether dedicated local language models are necessary since major AI companies already train on multilingual data, while others support the cultural preservation goals but suggest sharing training data with existing model builders might be more effective.

**Tags**: `#LLM`, `#sovereign-AI`, `#Huawei`, `#storage`, `#language-models`

---

<a id="item-3"></a>
## [Microsoft Copilot Cowork Exfiltrates Files via Prompt Injection](https://www.promptarmor.com/resources/microsoft-copilot-cowork-exfiltrates-files) ⭐️ 7.0/10

Microsoft Copilot's Cowork feature is vulnerable to prompt injection attacks that enable malicious skills to exfiltrate files from users' systems. The vulnerability allows attackers to craft seemingly innocent skills that execute unauthorized data extraction through injected commands. This represents a critical security flaw in enterprise-grade AI assistance, affecting Microsoft 365 users who rely on Copilot for workplace automation. The vulnerability demonstrates the growing security challenges with AI agent-based systems and highlights the need for robust input validation in AI-powered workplace tools. The attack exploits the skill-based architecture of Copilot Cowork, where malicious skills can bypass intended security boundaries through prompt injection techniques. The vulnerability affects file access controls and allows unauthorized data transmission to external endpoints.

hackernews · Kneenex · May 25, 21:45 · [Discussion](https://news.ycombinator.com/item?id=48272354)

**Background**: Microsoft Copilot Cowork is a feature that automates tasks across Microsoft 365 by executing skills on behalf of users, such as sending emails, creating documents, and scheduling meetings. Prompt injection attacks target AI models by inserting malicious inputs designed to manipulate the model's behavior beyond its intended purpose. These attacks are particularly dangerous in agent-based AI systems where the AI performs actions on users' behalf with elevated permissions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.microsoft.com/en-us/microsoft-365/blog/2026/03/09/copilot-cowork-a-new-way-of-getting-work-done/">Copilot Cowork: A new way of getting work done | Microsoft 365 Blog</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>
<li><a href="https://snyk.io/blog/toxicskills-malicious-ai-agent-skills-clawhub/">Snyk Finds Prompt Injection in 36%, 1467 Malicious Payloads in a ToxicSkills Study of Agent Skills Supply Chain Compromise | Snyk</a></li>

</ul>
</details>

**Discussion**: The community shows mixed reactions, with some arguing this is expected behavior since skills are essentially programs for LLM agents, while others emphasize Microsoft's responsibility for proper input validation. Some commenters suggest Microsoft rushed the feature to production, and there's ongoing debate about whether this constitutes incompetence versus a fundamental challenge in AI security.

**Tags**: `#security`, `#prompt-injection`, `#copilot`, `#vulnerability`, `#ai-security`

---

<a id="item-4"></a>
## [Armin Ronacher warns about AI-assisted bug reporting problems](https://simonwillison.net/2026/May/24/armin-ronacher/#atom-everything) ⭐️ 7.0/10

Armin Ronacher highlights how AI-assisted bug reporting tools are generating problematic issue submissions that contain inaccurate analyses and false conclusions despite appearing confident. He advocates for simplified bug reports focusing on what humans actually observed rather than AI-generated interpretations. This represents a growing challenge in open source software development as AI tools become more prevalent, creating noise that wastes maintainers' time and potentially delays legitimate bug fixes. The trend threatens the quality of issue tracking systems and developer productivity across the software ecosystem. Ronacher specifically mentions 'slop' issues with fake-minimal reproductions, incorrect root cause guesses, suggested implementation strategies, and irrelevant error classifications. He proposes a four-point format: command run, expected outcome, actual outcome, and exact error/log output.

rss · Simon Willison · May 24, 18:46

**Background**: AI-assisted bug reporting tools like BugBuddy and other extensions are becoming common, using LLMs to help users create bug reports by asking follow-up questions and auto-capturing screenshots, console errors, and network failures. These tools aim to make bug reporting accessible to non-technical users but can introduce inaccuracies through over-interpretation. Issue tracking systems in open source projects rely on accurate, concise reports to maintain efficiency and prioritize fixes effectively.

<details><summary>References</summary>
<ul>
<li><a href="https://chromewebstore.google.com/detail/bugbuddy/hlpanlhgmfkcjcoehnfefcplmbogdfmh">Report bugs to your dev team in 60 seconds. No technical knowledge...</a></li>
<li><a href="https://vibecheck-qa.com/blog/best-bug-reporting-chrome-extensions">Best Bug Reporting Chrome Extensions in 2026 | VibeCheck</a></li>
<li><a href="https://usersnap.com/blog/open-source-bug-tracking/">17 Excellent Open Source Bug Tracking Tools in 2026</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#bug-reporting`, `#AI-tools`, `#software-development`, `#issue-tracking`

---

<a id="item-5"></a>
## [California moves to exempt Linux from its age-verification law after backlash](https://www.tomshardware.com/software/linux/california-moves-to-exempt-linux-from-its-upcoming-age-verification-law-after-backlash-over-forcing-operating-systems-to-collect-users-ages-amendment-proposed-by-the-same-lawmaker-who-wrote-the-original-law) ⭐️ 6.0/10

California is moving to exempt Linux operating systems from its upcoming age-verification law after significant public backlash over the requirement that operating systems collect users' ages. This represents a significant policy shift in tech regulation that affects open-source software and raises First Amendment concerns about government requirements for operating system functionality. It demonstrates how public pressure can influence state legislation affecting digital rights. The original law would have required operating systems to collect user ages, which raised concerns among Linux developers about constitutional challenges and technical feasibility. The exemption addresses these concerns by removing Linux from the regulatory scope.

hackernews · rbanffy · May 25, 18:19 · [Discussion](https://news.ycombinator.com/item?id=48269961)

**Background**: California passed an age-verification law intended to restrict access to certain online content by requiring platforms to verify users' ages. However, the law's broad language inadvertently targeted operating systems like Linux, creating compliance challenges for open-source software that doesn't typically handle user age data collection. Age verification laws represent a growing trend in state-level internet regulation aimed at protecting minors online.

**Discussion**: Community discussion reveals mixed reactions with some commenters noting that most people don't understand the actual law's provisions. Technical users suggest alternative approaches like checking for parental controls in browsers, while others express concern about the legislative process lacking input from internet companies. Some speculate that the Linux exemption may be motivated by avoiding First Amendment challenges rather than genuine policy reconsideration.

**Tags**: `#regulation`, `#privacy`, `#linux`, `#age-verification`, `#policy`

---

<a id="item-6"></a>
## [Programming book sales decline signals shift in learning methods](https://unix.foo/posts/nobody-cracks-open-a-programming-book/) ⭐️ 6.0/10

A blog post analyzes the decline in programming book sales and its implications for developer learning patterns. Author Jon Bodner shares actual sales data from his 'Learning Go' book showing significant fluctuations with recent downward trends. This decline reflects a fundamental shift in how developers acquire programming knowledge, moving away from comprehensive book-based learning toward online resources like Google search and Stack Overflow. The change may impact how programming languages evolve, potentially becoming more complex since they're no longer constrained by what can fit in a teachable book format. Sales data shows 'Learning Go' had 367 copies sold in March 2025 but dropped to 124 in March 2026, representing a significant decline. The total first edition sales reached roughly 20,000 copies since its 2021 release, indicating that while books still sell, the market has contracted considerably.

hackernews · zdw · May 25, 23:21 · [Discussion](https://news.ycombinator.com/item?id=48273030)

**Background**: Programming books traditionally served as comprehensive guides for learning languages and development practices, offering structured, authoritative content that could be read cover-to-cover. The rise of online documentation, interactive tutorials, video courses, and community-driven Q&A platforms has created alternative learning pathways that are often more immediate and searchable than traditional books.

**Discussion**: Community responses show mixed views with some authors confirming sales declines while others argue that quality books still have value for learning idiomatic programming practices. Some commenters note that complex languages like C++ became too bloated for effective book-based learning, while others found success with comprehensive books like 'The Rust Programming Language' for mastering advanced concepts.

**Tags**: `#programming-books`, `#learning-resources`, `#developer-tools`, `#software-development`, `#education`

---

<a id="item-7"></a>
## [AI Converts Classic 1983 BASIC Game to Modern Web Version](https://simonwillison.net/2026/May/24/usborne-mad-house/#atom-everything) ⭐️ 6.0/10

Simon Willison used Claude AI to convert the 1983 Usborne 'Mad House' BASIC game into an interactive JavaScript/HTML version that maintains the original retro aesthetic and gameplay mechanics. This project demonstrates how AI can help preserve computing history by converting vintage software to modern formats, making classic educational materials accessible to new generations while maintaining their original charm and educational value. The converted game features a retro green-on-black terminal aesthetic with original gameplay elements like door counters, footsteps tracking, and ASCII corridor navigation, while being mobile-friendly and creditting the original Usborne source material.

rss · Simon Willison · May 24, 17:14

**Background**: Usborne published popular computer programming books in the 1980s that featured colorful illustrations and BASIC code that children could type into their home computers like the Commodore 64. BASIC (Beginner's All-purpose Symbolic Instruction Code) was designed for ease of use and became the de facto programming language for home computers in the late 1970s and 1980s. Claude is an AI assistant by Anthropic designed to help with creative tasks including code generation.

<details><summary>References</summary>
<ul>
<li><a href="https://usborne.com/us/books/computer-and-coding-books">Computer and coding books from Usborne | Usborne | Be Curious</a></li>
<li><a href="https://en.wikipedia.org/wiki/BASIC_programming_language">BASIC programming language</a></li>
<li><a href="https://claude.ai/">Sign in - Claude</a></li>

</ul>
</details>

**Tags**: `#retro-computing`, `#javascript`, `#web-development`, `#ai-assistance`, `#programming-history`

---

