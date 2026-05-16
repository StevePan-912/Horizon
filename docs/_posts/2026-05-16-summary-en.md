---
layout: default
title: "Horizon Summary: 2026-05-16 (EN)"
date: 2026-05-16
lang: en
---

> From 26 items, 9 important content pieces were selected

---

1. [A 0-click exploit chain for the Pixel 10](#item-1) ⭐️ 8.0/10
2. [Companies suffer from 'AI psychosis' by over-relying on AI](#item-2) ⭐️ 7.0/10
3. [Erlang/OTP 29.0 Released](#item-3) ⭐️ 7.0/10
4. [The sigmoids won't save you](#item-4) ⭐️ 7.0/10
5. [Zulip transitions to nonprofit foundation amid team changes](#item-5) ⭐️ 7.0/10
6. [NPM supply chain security vulnerabilities under scrutiny](#item-6) ⭐️ 7.0/10
7. [Image-blaster creates 3D environments from single images](#item-7) ⭐️ 7.0/10
8. [Company chooses React Native with coding agents](#item-8) ⭐️ 6.0/10
9. [Mitchell Hashimoto on Programming Language Fungibility](#item-9) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [A 0-click exploit chain for the Pixel 10](https://projectzero.google/2026/05/pixel-10-exploit.html) ⭐️ 8.0/10

Google Project Zero researchers discovered a 0-click exploit chain affecting Pixel 10 devices, exploiting vulnerabilities in AI-powered message processing features that decode media before user interaction. This represents a high-severity security vulnerability with potential widespread impact, highlighting critical security risks introduced by AI-powered features that process message media automatically before user interaction occurs. The exploit chain takes advantage of AI-powered message processing features that decode incoming media before users open messages, creating an expanded 0-click attack surface that increases security risks.

hackernews · happyhardcore · May 15, 13:39 · [Discussion](https://news.ycombinator.com/item?id=48148460)

**Background**: Google Project Zero is a team of security analysts employed by Google tasked with finding zero-day vulnerabilities, announced on July 15, 2014. A 0-click exploit is a cybersecurity attack that executes malicious code on a target system without requiring any user interaction. AI-powered message processing features have been added to mobile phones to enable better search and understanding of messages, but this creates increased security risks as message media must be decoded before the message is opened by the user.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Google_Project_Zero">Google Project Zero</a></li>
<li><a href="https://github.com/VivekMangale4/Zero-Click-Exploit">GitHub - VivekMangale4/Zero- Click - Exploit : A zero- click exploit is...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zero-day_vulnerability">Zero-day vulnerability - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community discussions highlight concerns about the security trade-offs of AI-powered features, with users questioning whether lessons have been learned about processing SMS messages without user consent. There's also discussion about Google's relatively fast 90-day patch response time compared to the rest of the Android ecosystem, and observations about the increasing frequency of published exploits potentially related to AI security focus.

**Tags**: `#security`, `#exploit`, `#android`, `#pixel`, `#ai-security`

---

<a id="item-2"></a>
## [Companies suffer from 'AI psychosis' by over-relying on AI](https://twitter.com/mitchellh/status/2055380239711457578) ⭐️ 7.0/10

Technology expert Mitchell Hashimoto highlights how companies are experiencing 'AI psychosis' by outsourcing critical decision-making to AI systems rather than using AI as a tool to augment human intelligence. This phenomenon involves companies relying on AI outputs without proper human oversight or verification. This trend represents a significant risk to business operations, potentially leading to poor strategic decisions, security vulnerabilities, and systems that become too complex for humans to understand or maintain. The over-reliance on AI for critical thinking could create systemic failures across industries. The concern specifically relates to companies that accept AI outputs without verification rather than using AI as a productivity enhancement tool. This includes situations where businesses treat AI-generated content as final decisions without human review, particularly in areas requiring critical judgment.

hackernews · reasonableklout · May 15, 20:26 · [Discussion](https://news.ycombinator.com/item?id=48153379)

**Background**: The term 'AI psychosis' in this context refers to organizational behavior rather than individual mental health issues. It describes companies that have become overly dependent on AI for decision-making processes, similar to how the original clinical term referred to individuals developing delusions through chatbot interactions. Human-in-the-loop AI systems are designed to maintain human oversight in AI decision-making processes to prevent such over-reliance.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_psychosis">AI psychosis</a></li>
<li><a href="https://altexsoft.medium.com/human-in-the-loop-in-ai-systems-825a34e61826?source=user_profile_page---------1-------------fb641da4b895----------------------">Human in the Loop in AI Systems . “People mistakenly... | Medium</a></li>

</ul>
</details>

**Discussion**: Community discussion reveals widespread agreement that companies are indeed outsourcing critical thinking to AI, with examples of financial professionals posting ChatGPT screenshots as their analysis. Commenters predict the emergence of 'AI rescue consulting' as a new service sector to fix AI-created problems, and express concerns about the potential for completely AI-written systems to become too complex for human understanding.

**Tags**: `#artificial-intelligence`, `#software-engineering`, `#business-strategy`, `#technology-adoption`, `#human-computer-interaction`

---

<a id="item-3"></a>
## [Erlang/OTP 29.0 Released](https://www.erlang.org/news/188) ⭐️ 7.0/10

Erlang/OTP 29.0 has been released with security improvements including disabling SSH/SFTP by default, new CLI capabilities through the io_ansi module, and various standard library enhancements. This release addresses critical security concerns by disabling potentially vulnerable services by default while enhancing Erlang's capabilities for building CLI applications, which expands its utility beyond traditional distributed systems. The release includes the new io_ansi module for CLI applications with seamless cross-node fwrite functionality, and adds support for -unsafe attributes, while prioritizing security by disabling SSH daemon and SFTP by default.

hackernews · pyinstallwoes · May 15, 23:33 · [Discussion](https://news.ycombinator.com/item?id=48155297)

**Background**: Erlang/OTP (Open Telecom Platform) is a set of libraries and design principles that standardize the creation of highly reliable, fault-tolerant applications originally developed for telecommunications. The platform runs on the BEAM virtual machine and is known for features like hot code swapping, distributed computing, and soft real-time capabilities. Erlang was originally developed by Ericsson in 1986 and became open source in 1998.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Erlang/OTP">Erlang/OTP</a></li>

</ul>
</details>

**Discussion**: Community members praised the security improvements of disabling SSH/SFTP by default and highlighted the new io_ansi module as a significant enhancement for CLI application development. Discussion included explanations of OTP's purpose for newcomers and interest in how record handling will evolve in the ecosystem.

**Tags**: `#erlang`, `#release`, `#security`, `#cli`, `#distributed-systems`

---

<a id="item-4"></a>
## [The sigmoids won't save you](https://www.astralcodexten.com/p/the-sigmoids-wont-save-you) ⭐️ 7.0/10

An analysis argues that AI progress may face fundamental physical and computational limits similar to other technologies that plateau after reaching their constraints, challenging assumptions about continued exponential growth in artificial intelligence capabilities. This analysis provides a contrarian perspective on AI development expectations, suggesting that current trends may not continue indefinitely and that technological progress often faces inherent limitations that lead to plateaus rather than sustained exponential growth. The analysis draws parallels between AI development and historical technology progressions like aircraft speed improvements, applying Lindy's Law to suggest that trends typically continue for about as long as they have already existed, with confidence intervals showing 90% probability of continuing between 1/19th to 19 times longer than current duration.

hackernews · Tomte · May 15, 10:51 · [Discussion](https://news.ycombinator.com/item?id=48147021)

**Background**: In neural networks, sigmoid functions are traditional activation functions that map inputs to values between 0 and 1, creating the characteristic S-shaped curve. Physical limits to computation refer to fundamental constraints imposed by physics on how much computation can be performed with given amounts of mass, volume, or energy. Lindy's Law suggests that the future life expectancy of something is proportional to its current age.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sigmoid_function">Sigmoid function - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Physical_limits_to_computation">Physical limits to computation</a></li>

</ul>
</details>

**Discussion**: Commenters noted that the article's premise about technology replacement cycles is valid but ignored its own answer about technologies being replaced when reaching limits. Some emphasized the impossibility of predicting AI development with certainty, while others highlighted Lindy's Law as a useful framework. There were also observations about the author's personal stake in maintaining trend continuation predictions.

**Tags**: `#AI`, `#technology-progress`, `#forecasting`, `#limits-of-computation`, `#historical-analysis`

---

<a id="item-5"></a>
## [Zulip transitions to nonprofit foundation amid team changes](https://blog.zulip.com/2026/05/15/announcing-zulip-foundation/) ⭐️ 7.0/10

Zulip is transitioning to a nonprofit foundation while founder Tim Abbott and three senior team members move to Anthropic, with the company being donated to the newly created Zulip Foundation to address trust and sustainability concerns. This transition addresses growing concerns about commercial pressures on open source projects and aims to ensure Zulip remains trustworthy and sustainable as a community-driven platform, separate from profit motives. The move comes as users increasingly worry about companies selling data or adding ads to open source products, and the foundation structure is designed to serve the public good rather than private interests.

hackernews · boramalper · May 15, 18:37 · [Discussion](https://news.ycombinator.com/item?id=48152168)

**Background**: Zulip is an open source chat and collaboration platform originally created in 2012 by Jeff Arnold, Waseem Daher, Jessica McKellar, and Tim Abbott. It has been used by various communities including the Rust programming language team for development discussions. Anthropic is an AI safety and research company known for developing the Claude AI system.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zulip">Zulip - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/company">Company \ Anthropic</a></li>

</ul>
</details>

**Discussion**: Community responses are mixed, with supporters appreciating the trustworthiness benefits of the nonprofit structure, while others express sadness about core team departures and skepticism about the timing of the announcement. Some users praise Zulip's superior interface compared to alternatives like Discord.

**Tags**: `#open-source`, `#governance`, `#nonprofit`, `#zulip`, `#community`

---

<a id="item-6"></a>
## [NPM supply chain security vulnerabilities under scrutiny](https://kevinpatel.xyz/posts/no-way-to-prevent-this/) ⭐️ 7.0/10

Analysis reveals ongoing security issues with npm package manager where supply chain attacks regularly occur, with community discussing mitigation strategies including cooldown periods and safer default configurations. This highlights critical security vulnerabilities in the JavaScript ecosystem that affect millions of developers and projects relying on npm, which has over 100 million weekly downloads. The discussion around cooldowns and safer configurations addresses real-world corporate security challenges. Cooldown mechanisms can prevent recent supply chain attacks like axios compromises by ignoring packages released within the last N days, since most compromised packages are taken down within hours. Postinstall scripts are identified as a major security risk requiring restriction.

hackernews · alligatorplum · May 16, 00:36 · [Discussion](https://news.ycombinator.com/item?id=48155690)

**Background**: npm (originally 'Node Package Manager', now a recursive backronym for 'npm is not an acronym') is the default package manager for Node.js and the largest software registry in the world. Supply chain attacks occur when malicious actors compromise trusted packages to distribute malware through dependencies. Recent high-profile attacks include the 'Shai-Hulud' incident and the axios compromise that affected the JavaScript ecosystem significantly.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Npm">npm - Wikipedia</a></li>
<li><a href="https://workos.com/blog/axios-npm-supply-chain-attack">The Axios npm supply chain attack : What every... — WorkOS</a></li>
<li><a href="https://www.reflectiz.com/blog/npm-supply-chain-attack/">The "Shai-Hulud" npm Supply Chain Attack : What We Know – Reflectiz</a></li>
<li><a href="https://www.stepsecurity.io/blog/introducing-the-npm-package-cooldown-check">Introducing the NPM Package Cooldown Check - StepSecurity</a></li>

</ul>
</details>

**Discussion**: Community members emphasize that cooldowns would have prevented major attacks like axios and tanstack compromises, noting that large companies often already have cooldowns via Artifactory/Nexus. There's frustration about the difficulty of maintaining safe global npm configurations across developer machines, and calls for the npm team to restrict postinstall scripts by default.

**Tags**: `#npm`, `#supply-chain-security`, `#package-management`, `#javascript`, `#cybersecurity`

---

<a id="item-7"></a>
## [Image-blaster creates 3D environments from single images](https://github.com/neilsonnn/image-blaster) ⭐️ 7.0/10

A new GitHub repository called Image-blaster uses AI-powered generation techniques to create 3D environments, sound effects, and meshes from a single image input. The tool represents advancement in computer vision and 3D reconstruction capabilities. This technology significantly lowers the barrier for 3D content creation, allowing users to generate complex 3D environments from simple 2D images. It represents a major leap from previous multi-image requirements like Microsoft's PhotoSynth, making 3D reconstruction more accessible for gaming, VR, and design applications. The project leverages AI-powered generation techniques and appears to integrate with platforms like WorldLabs for enhanced capabilities. Unlike traditional methods requiring multiple images, this approach works with just a single input image for 3D reconstruction.

hackernews · MattRogish · May 15, 15:42 · [Discussion](https://news.ycombinator.com/item?id=48150069)

**Background**: 3D reconstruction from single images has been a challenging area in computer vision, with previous solutions like Microsoft's PhotoSynth requiring multiple photos of the same scene. Recent advances in AI and neural networks have enabled more sophisticated understanding of depth, texture, and spatial relationships from 2D images, leading to tools like TripoSR, SAM 3D, and Any3D that can generate 3D models from single inputs. These technologies typically use deep learning models trained on large datasets to infer missing 3D information from 2D visual cues.

<details><summary>References</summary>
<ul>
<li><a href="https://www.triposrai.com/">TripoSR AI - Open-Source 3 D Reconstruction from Single Images</a></li>
<li><a href="https://dev.sam3d.org/">SAM 3 D : High Quality Image to 3 D Online</a></li>
<li><a href="https://any3d.art/">Any 3 D | Transform 2D Images into 3 D Models</a></li>

</ul>
</details>

**Discussion**: Users express excitement about the advancement, comparing it favorably to Microsoft's old PhotoSynth technology which required multiple images. Community members discuss related platforms like WorldLabs and Meshy.ai, noting that while impressive, some current tools still suffer from hallucination issues where generated content doesn't make logical sense. Some users explore applications for isometric sprite generation and compare it to similar projects like TRELLIS.

**Tags**: `#3D-reconstruction`, `#AI-computer-vision`, `#image-processing`, `#generative-ai`, `#mesh-generation`

---

<a id="item-8"></a>
## [Company chooses React Native with coding agents](https://simonwillison.net/2026/May/14/not-so-locked-in/#atom-everything) ⭐️ 6.0/10

A medium-sized technology company completed a coding-agent-driven rewrite of their legacy iPhone and Android apps to React Native, citing improved tooling quality and the ability to migrate back to native if needed. This demonstrates how improved development tooling and AI coding agents are reducing the risk of technology lock-in, allowing companies to make more flexible platform decisions based on current capabilities rather than long-term commitment fears. The company's decision was enabled by React Native's improved maturity over recent years and the availability of coding agents that reduce maintenance costs, making the 'port back to native' option feasible in the future.

rss · Simon Willison · May 14, 22:53

**Background**: React Native is a framework that allows developers to build mobile applications using JavaScript and React, sharing code between iOS and Android platforms. Coding agents are AI-powered tools that can assist with or automate programming tasks, potentially reducing development time and costs. Technology lock-in refers to the difficulty of switching from one technology platform to another due to compatibility issues, learning curves, and migration costs.

<details><summary>References</summary>
<ul>
<li><a href="https://apidog.com/blog/ai-coding-agents/">Top AI Coding Agents Shaping Modern Software Development</a></li>
<li><a href="https://zencoder.ai/blog/best-free-ai-agents-for-coding">8 Best Free AI Agents for Coding To Try in 2026</a></li>

</ul>
</details>

**Tags**: `#react-native`, `#mobile-development`, `#technology-decisions`, `#coding-agents`, `#software-architecture`

---

<a id="item-9"></a>
## [Mitchell Hashimoto on Programming Language Fungibility](https://simonwillison.net/2026/May/14/mitchell-hashimoto/#atom-everything) ⭐️ 6.0/10

Mitchell Hashimoto observed that programming languages are becoming more fungible, citing Bun's ability to switch from Zig to Rust quickly as evidence that languages are increasingly interchangeable rather than permanent commitments. This perspective challenges the traditional view of programming language lock-in, suggesting that modern development practices and tooling make it easier to migrate between languages based on changing requirements rather than being permanently tied to initial technology choices. Hashimoto noted that Bun demonstrated they could potentially switch to 'probably any language they want in roughly a week or two,' indicating that Rust is 'expendable' and can be replaced when no longer useful.

rss · Simon Willison · May 14, 22:31

**Background**: Zig is a systems programming language designed as a general-purpose improvement to C, emphasizing robustness and optimization, created by Andrew Kelley and first announced in 2016. Rust is a systems programming language emphasizing performance, type safety, and memory safety without a garbage collector, created by Graydon Hoare at Mozilla and first released in 2015. Bun is a JavaScript runtime that initially used Zig but later switched to Rust for performance reasons.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Rust_(programming_language)">Rust (programming language)</a></li>

</ul>
</details>

**Tags**: `#programming-languages`, `#rust`, `#zig`, `#bun`, `#software-architecture`

---