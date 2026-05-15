# Horizon Daily - 2026-05-15

> From 25 items, 13 important content pieces were selected

---

1. [First public macOS kernel memory corruption exploit on Apple M5](#item-1) ⭐️ 8.0/10
2. [New Nginx-Rift Exploit Bypasses ASLR Protection](#item-2) ⭐️ 8.0/10
3. [New arXiv policy: 1-year ban for hallucinated references](#item-3) ⭐️ 8.0/10
4. [Ontario auditors find doctors' AI note takers routinely blow basic facts](#item-4) ⭐️ 8.0/10
5. [Bun JavaScript runtime rewritten in Rust](#item-5) ⭐️ 8.0/10
6. [DS4 DeepSeek Announced with DwarfStar4 Inference Runtime](#item-6) ⭐️ 7.0/10
7. [RTX 5090 eGPU Tested on M4 MacBook Air Gaming](#item-7) ⭐️ 7.0/10
8. [CSP Allow-list Experiment Demonstrates Novel Bypass Technique](#item-8) ⭐️ 7.0/10
9. [Codex is now in the ChatGPT mobile app](#item-9) ⭐️ 6.0/10
10. [HDD Firmware Hacking Techniques Explored](#item-10) ⭐️ 6.0/10
11. [Technology choices become more flexible with React Native](#item-11) ⭐️ 6.0/10
12. [Mitchell Hashimoto on Programming Language Fungibility](#item-12) ⭐️ 6.0/10
13. [Boris Mann Questions Meaningfulness of 'AI Agents' Concept](#item-13) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [First public macOS kernel memory corruption exploit on Apple M5](https://blog.calif.io/p/first-public-kernel-memory-corruption) ⭐️ 8.0/10

The first public kernel memory corruption exploit targeting Apple M5 silicon has been released, marking a significant security milestone for Apple's latest hardware architecture. Researchers shared their vulnerability research report with Apple during a meeting at Apple Park. This represents a critical security achievement as Apple M5 silicon was designed with advanced security features like Memory Tagging Extension (MTE) specifically to prevent memory corruption exploits. The successful bypass of these protections indicates potential vulnerabilities in Apple's newest security architecture. The exploit reportedly survives Memory Integrity Engine (MIE), which was introduced as the marquee security feature for Apple M5 and A19 chips, specifically designed to stop memory corruption exploits. The vulnerability class affects many sophisticated compromises on iOS and macOS platforms.

hackernews · quadrige · May 14, 18:25 · [Discussion](https://news.ycombinator.com/item?id=48139219)

**Background**: Apple M5 silicon represents Apple's latest generation of custom-designed chips for Mac computers, featuring enhanced security architecture including Memory Tagging Extension (MTE) technology. Kernel memory corruption exploits target vulnerabilities in the operating system's core, potentially allowing attackers to gain elevated privileges and system control. These types of vulnerabilities are particularly concerning as they can bypass user-space security measures.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.calif.io/p/first-public-kernel-memory-corruption">First public macOS kernel memory corruption exploit on Apple M 5</a></li>
<li><a href="https://malware.news/t/first-public-macos-kernel-memory-corruption-exploit-on-apple-m5/107008">First public macOS kernel memory corruption exploit on Apple M5 - Malware Analysis - Malware Analysis, News and Indicators</a></li>
<li><a href="https://www.apple.com/newsroom/2025/10/apple-unleashes-m5-the-next-big-leap-in-ai-performance-for-apple-silicon/">Apple unleashes M 5 , the next big leap in AI performance for... - Apple</a></li>

</ul>
</details>

**Discussion**: The security community shows mixed reactions with some expressing curiosity about how the bug survived MTE protection, while others discuss potential bounty values ranging from $100,000 to $1.5 million depending on packaging and demonstration approach. Some commenters express skepticism about the claims, and there are discussions about the future impact of LLMs on security research and vulnerability discovery.

**Tags**: `#security`, `#exploit`, `#macOS`, `#kernel`, `#apple-m5`

---

<a id="item-2"></a>
## [New Nginx-Rift Exploit Bypasses ASLR Protection](https://github.com/DepthFirstDisclosures/Nginx-Rift) ⭐️ 8.0/10

A critical heap buffer overflow vulnerability called 'Nginx-Rift' (CVE-2026-42945) has been disclosed that affects Nginx versions from 0.6.27 (2008) to 1.30.0, potentially allowing unauthenticated remote code execution through rewrite directives with regex capture groups. This vulnerability is significant because Nginx is one of the most widely deployed web servers globally, and the exploit potentially enables remote code execution that could compromise entire server infrastructures. The fact that it has existed for 18 years undetected makes it particularly concerning for organizations running older Nginx versions. The vulnerability requires specific conditions including a 'rewrite' directive with a question mark in the replacement string and a subsequent 'set' directive referencing regex capture groups (e.g., $1, $2). While the published proof-of-concept disables ASLR, security experts believe ASLR bypass techniques likely exist. Mitigation involves using named captures instead of unnamed captures in rewrite definitions.

hackernews · hetsaraiya · May 14, 17:17 · [Discussion](https://news.ycombinator.com/item?id=48138268)

**Background**: ASLR (Address Space Layout Randomization) is a security technique that randomly arranges address spaces to prevent exploitation of memory corruption vulnerabilities. Nginx is a popular web server software that handles HTTP requests using configuration directives like 'rewrite' which can include regular expression patterns. The vulnerability exists in the script engine's two-pass process where buffer size calculation and data copying occur separately.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Aws7/nginx-rift">GitHub - Aws7/ nginx - rift : exploit for CVE-2026-42945 · GitHub</a></li>
<li><a href="https://www.picussecurity.com/resource/blog/nginx-rift-cve-2026-42945-critical-heap-buffer-overflow-vulnerability-explained">NGINX Rift : CVE-2026-42945 Critical Heap Buffer Overflow...</a></li>
<li><a href="https://devops-daily.com/posts/nginx-rift-cve-2026-42945-rewrite-rce">NGINX Rift (CVE-2026-42945): The 18-Year-Old Rewrite Bug That...</a></li>

</ul>
</details>

**Discussion**: Security experts emphasize that the published exploit disabling ASLR doesn't mean ASLR bypass isn't possible - the original research suggests reliable ASLR bypass methods exist. Community members note that mitigation involves replacing unnamed captures ($1, $2) with named captures in rewrite directives, and discuss alternative web servers like Caddy and Jetty written in memory-safe languages.

**Tags**: `#security`, `#exploit`, `#nginx`, `#vulnerability`, `#aslr`

---

<a id="item-3"></a>
## [New arXiv policy: 1-year ban for hallucinated references](https://twitter.com/tdietterich/status/2055000956144935055) ⭐️ 8.0/10

arXiv announces a new policy imposing 1-year bans on authors who submit papers with hallucinated references, requiring subsequent submissions to first be accepted at peer-reviewed venues. This policy addresses the growing problem of AI hallucination in academic publishing, where language models generate fake citations that undermine scientific integrity and waste researchers' time tracking down non-existent papers. The penalty includes a 1-year ban from arXiv followed by the requirement that future submissions must first be accepted at reputable peer-reviewed venues, though the exact detection methods for identifying hallucinated references remain unclear.

hackernews · gjuggler · May 14, 20:39 · [Discussion](https://news.ycombinator.com/item?id=48140922)

**Background**: arXiv is a free distribution service and open-access archive hosting nearly 2.4 million scholarly articles in physics, mathematics, computer science, and other fields. AI hallucination occurs when language models generate plausible-sounding but false information, including fake citations that don't correspond to real papers. Peer review involves independent assessment of research papers by experts in the same field to evaluate quality and suitability for publication.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ArXiv">arXiv - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Hallucination_(artificial_intelligence)">Hallucination (artificial intelligence) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Peer_review">Peer review - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community response is largely positive, with users supporting the policy as beneficial for scientific integrity. However, concerns were raised about detection methods at scale, with questions about whether manual spot checks or automated DOI verification would be used. Some users noted the policy might not be live yet as it wasn't clearly visible on arXiv's official policies page.

**Tags**: `#academic-publishing`, `#AI-hallucination`, `#research-integrity`, `#arXiv`, `#peer-review`

---

<a id="item-4"></a>
## [Ontario auditors find doctors' AI note takers routinely blow basic facts](https://www.theregister.com/ai-ml/2026/05/14/ontario-auditors-find-doctors-ai-note-takers-routinely-blow-basic-facts/5240771) ⭐️ 8.0/10

Ontario auditors discovered that AI-powered medical note-taking systems are routinely generating factually incorrect information, with 9 out of 20 systems found to fabricate information and make suggestions to patients' treatment plans. This represents serious safety concerns in healthcare settings where AI hallucinations could lead to incorrect diagnoses, inappropriate treatments, and compromised patient care, highlighting the critical need for human oversight in medical AI applications. The audit revealed that AI systems were making up common symptoms that didn't exist or claiming diagnoses that fit some details but not others, with error rates and sample sizes remaining unclear from the initial report.

hackernews · sohkamyung · May 14, 22:37 · [Discussion](https://news.ycombinator.com/item?id=48142188)

**Background**: AI medical note-taking systems use advanced speech recognition and natural language processing to convert doctor-patient conversations into structured clinical notes, with companies like Abridge serving major healthcare systems. However, AI hallucinations in healthcare represent a particularly dangerous risk since inaccurate medical information can directly impact patient safety, unlike other fields where hallucinations might merely produce confusing answers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bluelineinsights.com/insights/ai-hallucinations-in-healthcare-what-nurses-need-to-understand">AI Hallucinations in Healthcare : What Nurses... | Blueline Insights</a></li>
<li><a href="https://www.memrizz.com/blogs/ai-vs-human-scribes-who-wins-the-battle-for-medical-note-taking">AI vs. Human Scribes: Who Wins the Battle for Medical Note - Taking ?</a></li>
<li><a href="https://www.linkedin.com/pulse/ai-hallucinations-healthcare-when-confidence-becomes-parameswaran-1uhge">AI Hallucinations in Healthcare : When Confidence Becomes the Risk</a></li>

</ul>
</details>

**Discussion**: Users shared personal experiences of AI transcription failures, including misdiagnosing runner's knee as osteoporosis with fabricated symptoms, and business meetings where AI note-takers created false vendor promises. Commenters emphasized the critical need to check transcripts and questioned the adoption of systems with potentially high error rates despite the lack of quantitative data in the report.

**Tags**: `#AI-hallucination`, `#healthcare-AI`, `#medical-technology`, `#LLM-reliability`, `#patient-safety`

---

<a id="item-5"></a>
## [Bun JavaScript runtime rewritten in Rust](https://github.com/oven-sh/bun/pull/30412) ⭐️ 8.0/10

Bun has completed its rewrite from Zig to Rust with over 1 million lines of Rust code now in the codebase, representing a major architectural shift for the JavaScript runtime. This rewrite promises improved memory safety, performance, and security benefits due to Rust's compile-time safety guarantees, potentially making Bun more robust against common memory-related bugs like use-after-free and double-free errors. The Rust conversion addresses critical memory safety issues that plagued the Zig version, with over 10,000 unsafe blocks identified in the codebase, though the transition required significant preparation including detailed mapping of Zig to Rust idioms.

hackernews · Chaoses · May 14, 08:15 · [Discussion](https://news.ycombinator.com/item?id=48132488)

**Background**: Bun is a JavaScript runtime designed as a drop-in replacement for Node.js, using Safari's JavaScriptCore engine instead of V8. Originally written in Zig, a systems programming language focused on simplicity and performance, Bun aimed to provide faster JavaScript execution with built-in bundling and package management. Rust is a systems programming language emphasizing memory safety without garbage collection through its borrow checker.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bun_(software)">Bun (software) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Rust_(programming_language)">Rust (programming language)</a></li>

</ul>
</details>

**Discussion**: Community discussion highlights the extensive preparation involved in the rewrite, with detailed documentation mapping Zig to Rust idioms, and notes that the codebase already had internal smart pointer types that mapped directly to Rust equivalents. Developers noted that over 10,000 unsafe blocks remain in the Rust codebase, indicating ongoing complexity challenges.

**Tags**: `#rust`, `#javascript`, `#bun`, `#systems-programming`, `#performance`

---

<a id="item-6"></a>
## [DS4 DeepSeek Announced with DwarfStar4 Inference Runtime](https://antirez.com/news/165) ⭐️ 7.0/10

Antirez announced DS4 (DeepSeek 4) and its dedicated inference runtime called DwarfStar4, which currently requires 96GB of VRAM to run DeepSeek V4 Flash efficiently. The runtime supports multiple backends including Metal for MacBooks, NVIDIA CUDA, and AMD ROCm. This represents a significant advancement in local LLM capabilities, potentially challenging cloud-based AI services as local models approach the intelligence level of proprietary systems like Claude. The development signals growing competition in the AI industry and the democratization of powerful language models. DwarfStar4 is specifically designed for DeepSeek V4 Flash rather than being a generic GGUF runner, and it leverages Metal as its primary target backend starting from MacBooks with 96GB of RAM. The project builds upon llama.cpp and GGML foundations while focusing on narrow, specialized functionality.

hackernews · caust1c · May 14, 22:29 · [Discussion](https://news.ycombinator.com/item?id=48142108)

**Background**: DeepSeek V4 Flash is an efficiency-optimized Mixture-of-Experts model with 284B total parameters but only 13B activated parameters, supporting a 1M-token context window. Local LLM inference has been constrained primarily by memory capacity, with high-end models requiring substantial VRAM to operate effectively. The trend toward more capable local models challenges traditional cloud-based AI service models.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/unsloth/DeepSeek-V4-Flash">unsloth/ DeepSeek -V4-Flash · Hugging Face</a></li>
<li><a href="https://github.com/antirez/ds4">GitHub - antirez/ds4: DeepSeek 4 Flash local inference engine for...</a></li>
<li><a href="https://www.sitepoint.com/local-llm-hardware-requirements-mac-vs-pc-2026/">Local LLM Hardware Requirements: Mac vs PC 2026 | SitePoint</a></li>

</ul>
</details>

**Discussion**: Community discussions highlight the impressive capabilities of local models approaching those of commercial systems like Claude, though running much slower. Users express curiosity about the saturation point for 'enough' intelligence for coding tasks and whether local models could disrupt existing business models of companies like Anthropic. There's speculation about future hardware requirements potentially dropping to 16GB RAM within a few years.

**Tags**: `#llm`, `#inference`, `#deepseek`, `#local-ai`, `#hardware`

---

<a id="item-7"></a>
## [RTX 5090 eGPU Tested on M4 MacBook Air Gaming](https://scottjg.com/posts/2026-05-05-egpu-mac-gaming/) ⭐️ 7.0/10

Technical analysis demonstrates using an external RTX 5090 GPU with M4 MacBook Air for gaming, including detailed benchmarks comparing performance limitations and practical gaming scenarios. This represents a significant achievement in Apple Silicon gaming since eGPUs were officially unsupported on Apple Silicon Macs, opening new possibilities for Mac users seeking high-end gaming performance. The setup faces Thunderbolt bandwidth limitations and latency issues, with performance drops of 10-20% compared to direct PCIe connections, while also revealing Apple Silicon's slow prompt processing speeds for LLM workloads.

hackernews · allenleee · May 14, 15:47 · [Discussion](https://news.ycombinator.com/item?id=48137145)

**Background**: eGPUs (external GPUs) traditionally connect via Thunderbolt to enhance graphics performance on laptops, though Apple officially discontinued support for eGPUs on Apple Silicon Macs. Apple Silicon refers to custom ARM-based processors designed by Apple for Mac computers, starting with the M1 chip in 2020. Thunderbolt connections inherently introduce bandwidth bottlenecks and latency compared to direct PCIe connections inside a computer chassis.

<details><summary>References</summary>
<ul>
<li><a href="https://www.xda-developers.com/egpus-over-thunderbolt-sound-great-but-be-aware-limitations/">eGPUs over Thunderbolt sound great, but be aware of these limitations</a></li>
<li><a href="https://egpu.io/forums/mac-setup/pcie-slot-dgpu-vs-thunderbolt-3-egpu-internal-display-test/">eGPU Performance Loss – PCI Express vs. Thunderbolt | Thunderbolt macOS eGPU</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_silicon">Apple silicon - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community members expressed excitement about VM GPU passthrough possibilities and noted that Apple officially states eGPUs require Intel processors, making this achievement particularly noteworthy. Commenters highlighted the practical value for LLM performance improvements and discussed technical challenges with OpenGL support and Vulkan compatibility.

**Tags**: `#apple-silicon`, `#egpu`, `#gaming`, `#benchmarks`, `#macos`

---

<a id="item-8"></a>
## [CSP Allow-list Experiment Demonstrates Novel Bypass Technique](https://simonwillison.net/2026/May/13/csp-allow/#atom-everything) ⭐️ 7.0/10

Simon Willison created a tool that demonstrates how sandboxed iframes can intercept CSP errors and pass them to the parent window, allowing users to dynamically add domains to an allow-list. The experiment shows a custom fetch() implementation that catches CSP violations and prompts users to approve blocked domains. This experiment reveals a novel approach to bypassing Content Security Policy protections, highlighting potential security weaknesses in current CSP implementations. It demonstrates how legitimate security features can be leveraged as attack vectors, which is crucial for security professionals to understand. The tool uses sandboxed iframes with custom fetch() implementations that intercept CSP errors and communicate them to the parent window for user approval. Built with GPT-5.5 xhigh in the Codex desktop app, it demonstrates how the sandbox escape mechanism works through error interception and dynamic allow-list creation.

rss · Simon Willison · May 13, 04:50

**Background**: Content Security Policy (CSP) is a security standard designed to prevent cross-site scripting (XSS), clickjacking and other code injection attacks by specifying which domains can load resources. Sandboxed iframes apply additional restrictions to content within an iframe, limiting its capabilities to reduce security risks from third-party content. The combination of these security measures is meant to provide defense-in-depth against malicious code execution.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Content_Security_Policy">Content Security Policy - Wikipedia</a></li>
<li><a href="https://web.dev/articles/sandboxed-iframes">Play safely in sandboxed IFrames | Articles | web.dev</a></li>

</ul>
</details>

**Tags**: `#security`, `#web-development`, `#csp`, `#sandbox`, `#javascript`

---

<a id="item-9"></a>
## [Codex is now in the ChatGPT mobile app](https://openai.com/index/work-with-codex-from-anywhere/) ⭐️ 6.0/10

OpenAI has integrated Codex, its AI code generation model, into the ChatGPT mobile application, making code generation capabilities freely accessible to mobile users through their ChatGPT accounts. This represents a significant accessibility improvement, allowing developers to access AI-powered code generation on mobile devices without additional payment, expanding coding capabilities beyond traditional desktop environments. Codex is now included in the free ChatGPT plan and accessible via mobile app, though users note that mobile interfaces present challenges for effective coding workflows compared to traditional keyboards and larger screens.

hackernews · mikeevans · May 14, 20:06 · [Discussion](https://news.ycombinator.com/item?id=48140529)

**Background**: OpenAI Codex is a large language model specifically designed for translating natural language prompts into source code. It serves as an AI coding partner that can assist with various programming tasks and has previously been available primarily through desktop applications or command-line interfaces. The integration brings these capabilities to mobile platforms for increased accessibility.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex_(language_model)">OpenAI Codex (language model ) - Wikipedia</a></li>
<li><a href="https://openai.com/codex/">Codex | AI Coding Partner from OpenAI | OpenAI</a></li>
<li><a href="https://www.ibm.com/think/topics/ai-code-generation">What is AI code-generation? | IBM</a></li>

</ul>
</details>

**Discussion**: Users express mixed reactions, with some appreciating free access and portability while others note limitations with mobile coding interfaces. Community members report that smaller screens and lack of physical keyboards reduce effectiveness compared to desktop coding, and there are concerns about data privacy since interactions contribute to training datasets.

**Tags**: `#AI`, `#Code Generation`, `#Mobile Development`, `#OpenAI`, `#ChatGPT`

---

<a id="item-10"></a>
## [HDD Firmware Hacking Techniques Explored](https://icode4.coffee/?p=1465) ⭐️ 6.0/10

A technical exploration reveals how hard drive firmware can be reverse engineered and how vendors use trivial obfuscation methods that are easily bypassed by security researchers. This highlights significant security vulnerabilities in storage device firmware protection, showing that vendor obfuscation methods offer minimal security against determined attackers and could expose users to firmware-level attacks. Researchers demonstrated that some vendor firmware update utilities decrypt firmware to disk before uploading, making it possible to capture decrypted versions through system call interception techniques like seccomp.

hackernews · jsploit · May 14, 16:19 · [Discussion](https://news.ycombinator.com/item?id=48137553)

**Background**: Hard drive firmware is low-level software embedded in storage devices that controls basic operations like sector translation, head positioning, and error correction. Unlike BIOS firmware on motherboards, hard drive firmware is typically stored partially in controller chips and partially on reserved areas of the disk platters, making it less accessible to users but still vulnerable to sophisticated attacks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Firmware">Firmware - Wikipedia</a></li>
<li><a href="https://www.datalab247.com/articles/article6.html">How Hard Drive works: Firmware on Disk Platter and PCB</a></li>
<li><a href="https://smarthdd.com/firmware.htm">Hard drive firmware</a></li>

</ul>
</details>

**Discussion**: The community discussion reveals that vendor obfuscation methods are considered trivial by security researchers, with practical examples shared of how Linux SSD firmware update utilities can be exploited to extract decrypted firmware through syscall monitoring. Commenters noted that Samsung began encrypting their SSD firmware after earlier versions were successfully reverse-engineered and published.

**Tags**: `#firmware`, `#security`, `#reverse-engineering`, `#storage`, `#hdd`

---

<a id="item-11"></a>
## [Technology choices become more flexible with React Native](https://simonwillison.net/2026/May/14/not-so-locked-in/#atom-everything) ⭐️ 6.0/10

A medium-sized technology company completed a coding-agent-driven rewrite of their legacy iPhone and Android apps to React Native, feeling confident they could switch back to native development if needed. This reflects a broader trend where technology lock-in is decreasing as frameworks have matured. This shift represents a fundamental change in how companies approach technology decisions, moving from permanent commitments to more flexible strategies. It demonstrates that modern cross-platform frameworks like React Native have matured enough to be viable alternatives to native development without the fear of being locked in. The company felt React Native had improved significantly over recent years to cover all their app requirements. The availability of coding agents reduced the perceived cost advantage of maintaining separate native codebases, yet they still chose React Native for its flexibility.

rss · Simon Willison · May 14, 22:53

**Background**: React Native is an open-source UI framework developed by Meta that allows building native mobile applications for iOS and Android using React and JavaScript. It enables 'learn once, write anywhere' development by leveraging native platform capabilities while using familiar web development paradigms. Coding agents refer to AI-powered tools that can assist with or automate software development tasks, including full application rewrites.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/React_Native">React Native</a></li>
<li><a href="https://timdeschryver.dev/blog/keep-agentic-ai-simple-a-practical-workflow-for-software-development">Keep Agentic AI Simple: A Practical Workflow for Software Development</a></li>
<li><a href="https://thecodersblog.com/bun-runtime-migration-from-zig-to-rust-2026/">Bun's Rust Pivot: What the Zig - to - Rust Migration Means for...</a></li>

</ul>
</details>

**Tags**: `#mobile-development`, `#react-native`, `#technology-decisions`, `#software-architecture`

---

<a id="item-12"></a>
## [Mitchell Hashimoto on Programming Language Fungibility](https://simonwillison.net/2026/May/14/mitchell-hashimoto/#atom-everything) ⭐️ 6.0/10

Mitchell Hashimoto observed that programming languages are becoming more fungible, citing Bun's ability to switch from Zig to Rust quickly as evidence that languages are no longer permanent commitments but rather interchangeable tools. This represents a fundamental shift in software engineering where language choice becomes more tactical rather than strategic, potentially reducing vendor lock-in and increasing flexibility for development teams to adapt to changing requirements. Hashimoto notes that Bun demonstrated the ability to switch languages 'in roughly a week or two,' suggesting that modern tooling and abstractions have reduced the friction traditionally associated with language migrations.

rss · Simon Willison · May 14, 22:31

**Background**: Bun is a JavaScript runtime that initially used Zig as its implementation language before switching to Rust, demonstrating rapid language migration capabilities. Zig and Rust are both modern systems programming languages focused on performance and safety, with Zig emphasizing simplicity and Rust emphasizing memory safety without garbage collection. Mitchell Hashimoto is the creator of popular infrastructure tools like Terraform and Vagrant through HashiCorp.

<details><summary>References</summary>
<ul>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Rust_(programming_language)">Rust (programming language)</a></li>

</ul>
</details>

**Tags**: `#programming-languages`, `#rust`, `#zig`, `#bun`, `#software-engineering`

---

<a id="item-13"></a>
## [Boris Mann Questions Meaningfulness of 'AI Agents' Concept](https://simonwillison.net/2026/May/13/boris-mann/#atom-everything) ⭐️ 6.0/10

Boris Mann quoted that saying '11 AI agents' is meaningless, comparing it to equally meaningless phrases like '11 spreadsheets' or '11 browser tabs' to highlight the semantic confusion around AI agents. This critique highlights the need for better definitions in the AI agent space and challenges the current hype around AI agents by pointing out that simply having multiple agents doesn't indicate meaningful functionality or value. The quote emphasizes that the number of AI agents alone is not a meaningful metric, similar to how counting spreadsheets or browser tabs doesn't indicate productivity or capability.

rss · Simon Willison · May 13, 16:15

**Background**: An AI agent is typically defined as a software system that uses artificial intelligence to pursue goals and complete tasks on behalf of users with varying degrees of autonomy. However, there's ongoing debate about what constitutes a true AI agent versus simple automated tools or scripts. The term has become increasingly popular in generative AI discussions, sometimes leading to semantic confusion about capabilities and definitions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Intelligent_agent">Intelligent agent - Wikipedia</a></li>
<li><a href="https://cloud.google.com/discover/what-are-ai-agents">What are AI agents? Definition, examples, and types | Google Cloud</a></li>

</ul>
</details>

**Tags**: `#ai-agents`, `#ai`, `#agent-definitions`, `#criticism`, `#semantic-analysis`

---

