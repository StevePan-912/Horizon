---
layout: default
title: "Horizon Summary: 2026-05-24 (EN)"
date: 2026-05-24
lang: en
---

> From 23 items, 6 important content pieces were selected

---

1. [Memory shortage causes consumer electronics repricing](#item-1) ⭐️ 8.0/10
2. [SpaceX launches Starship v3 rocket](#item-2) ⭐️ 7.0/10
3. [.NET (C#) finally gets union types](#item-3) ⭐️ 7.0/10
4. [80386 microcode disassembled](#item-4) ⭐️ 7.0/10
5. [FTC fines companies $1M for fake AI 'active listening' ads](#item-5) ⭐️ 7.0/10
6. [HTML <dl> Element Usage and Accessibility Discussion](#item-6) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [Memory shortage causes consumer electronics repricing](https://simonwillison.net/2026/May/22/memory-shortage/#atom-everything) ⭐️ 8.0/10

AI data center growth is driving HBM memory demand from 2% to 20% of wafer capacity by 2026, causing shortages and price increases for consumer electronics that rely on DDR and LPDDR memory. A single gigabyte of HBM consumes more than three times the wafer capacity that a gigabyte of DDR or LPDDR does. This represents a fundamental shift in semiconductor economics where AI's appetite for high-margin HBM memory is constraining production of consumer-device RAM, making electronics more expensive globally. The shortage particularly affects sub-$100 smartphones critical to emerging markets like Africa and South Asia. Memory manufacturers have fixed wafer processing capacity that they allocate between DDR (desktops/servers), LPDDR (mobile devices), and HBM (GPUs). Only three major memory companies remain, and they prioritize HBM production due to higher profit margins and strong demand.

rss · Simon Willison · May 22, 22:01

**Background**: HBM (High Bandwidth Memory) is a specialized memory interface for 3D-stacked SDRAM used in high-performance graphics, AI and datacenter devices, offering much higher bandwidth than traditional DDR memory. DDR (Double Data Rate) and LPDDR (Low Power Double Data Rate) are standard memory types used in general-purpose computing and mobile devices respectively, balancing performance, power efficiency, and cost differently than HBM.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/HBM_memory_shortage">HBM memory shortage</a></li>
<li><a href="https://en.wikipedia.org/wiki/2024–present_global_memory_supply_shortage">2024–present global memory supply shortage - Wikipedia</a></li>
<li><a href="https://semiwiki.com/wikis/semiconductor-ip-wikis/ddr-vs-lpddr-vs-hbm-wiki/">DDR vs. LPDDR vs. HBM Wiki - SemiWiki</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#memory`, `#AI-hardware`, `#supply-chain`, `#consumer-electronics`

---

<a id="item-2"></a>
## [SpaceX launches Starship v3 rocket](https://www.space.com/space-exploration/launches-spacecraft/spacex-starship-v3-megarocket-first-test-flight) ⭐️ 7.0/10

SpaceX successfully launched their Starship v3 prototype rocket, achieving partial mission objectives despite experiencing engine failures and booster landing issues during the test flight. This represents a significant milestone in reusable rocket technology development, demonstrating SpaceX's rapid iteration approach toward creating a fully reusable super heavy-lift launch vehicle for future Mars missions and lunar exploration. The Starship v3 features upgraded Raptor 3 engines and improved heat shield technology, with the vehicle standing taller and more capable than previous versions, designed for 100-ton LEO payload capacity using methalox (methane-oxygen) propulsion.

hackernews · busymom0 · May 22, 23:41 · [Discussion](https://news.ycombinator.com/item?id=48242959)

**Background**: Starship is a two-stage, fully reusable, super heavy-lift launch vehicle under development by SpaceX, intended as the successor to Falcon 9 and Falcon Heavy rockets. The Raptor engines use a methalox (liquid methane and liquid oxygen) propellant combination with full-flow staged combustion technology, representing a significant advancement in rocket propulsion systems. The heat shield system has been iteratively improved across flight tests to handle extreme reentry temperatures.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/SpaceX_Starship">SpaceX Starship - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/SpaceX_Raptor">SpaceX Raptor - Wikipedia</a></li>
<li><a href="https://spacexstock.com/starship-heat-shield-how-it-handles-extreme-temperatures/">Starship Heat Shield: How It Handles Extreme Temperatures</a></li>

</ul>
</details>

**Discussion**: The community praised SpaceX's rapid iteration approach, viewing failures as valuable learning experiences rather than setbacks. Commentators noted improvements in heat shield performance during reentry compared to previous flights, and highlighted the impressive guidance system software that allowed Starship to land on target despite multiple engine failures.

**Tags**: `#spaceflight`, `#rocketry`, `#spacex`, `#engineering`, `#aerospace`

---

<a id="item-3"></a>
## [.NET (C#) finally gets union types](https://andrewlock.net/exploring-the-dotnet-11-preview-2-dotnet-gets-union-types/) ⭐️ 7.0/10

C# is introducing union types in .NET 11 preview, providing developers with a more idiomatic way to handle sum types that have been requested for years. This feature represents a significant addition to C# 15 that allows representing values that can be one of several distinct types. This addresses a long-standing developer need for better type safety and more expressive type systems in C#, allowing cleaner handling of scenarios where values can be one of multiple distinct types. It brings C# closer to functional programming paradigms while maintaining its object-oriented roots. Union types provide a more type-safe alternative to using enums for representing mutually exclusive states, addressing classic problems like the 'FileNotFound' boolean issue. The feature has been in development for over a decade and represents careful design considerations by the C# team.

hackernews · ingve · May 22, 12:28 · [Discussion](https://news.ycombinator.com/item?id=48234954)

**Background**: Union types (also known as sum types or tagged unions) allow a variable to hold values of different types at different times, but with compile-time safety ensuring only valid types are used. They're commonly found in functional programming languages and provide a more robust alternative to traditional approaches like using enums with special values or complex inheritance hierarchies. F# has had union types for decades, and their introduction to C# represents a major evolution in the language's type system.

<details><summary>References</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/dotnet/core/whats-new/dotnet-11/overview">What's new in .NET 11 | Microsoft Learn</a></li>
<li><a href="https://medium.com/turbo-net/whats-new-in-net-11-features-improvements-and-what-actually-matters-7125b6f71497">What’s New in .NET 11 Preview for Developers | Turbo .NET</a></li>
<li><a href="https://dosibridge.com/blog/net-11-preview-top-10-features-developers-should-know">.NET 11 Preview: Top 10 Features Developers Should Know</a></li>

</ul>
</details>

**Discussion**: The community shows significant excitement about the feature, with many developers expressing they've waited years for union types in C#. Some commenters note that F# has had this functionality for decades and C# is gradually catching up with functional programming features. There's appreciation for Microsoft's approach of adding performance-oriented features while maintaining ease of use for non-performance-critical scenarios.

**Tags**: `#c#`, `#dotnet`, `#union-types`, `#programming-languages`, `#software-engineering`

---

<a id="item-4"></a>
## [80386 microcode disassembled](https://www.reenigne.org/blog/80386-microcode-disassembled/) ⭐️ 7.0/10

Researchers have successfully extracted and disassembled the microcode from Intel's 80386 processor using high-resolution die images, creating a detailed text-based disassembly of the processor's microcode instructions. This achievement provides unprecedented insight into the internal workings of a historically important processor, enabling better understanding of x86 architecture evolution and supporting reverse engineering research for preservation and security analysis. The disassembly reveals that unlike the 8086, the 80386 always executes μ-ops with microcode for every instruction, and the output is essentially a static assembly language dialect that required inventing new terminology for previously undocumented components.

hackernews · nand2mario · May 23, 12:11 · [Discussion](https://news.ycombinator.com/item?id=48247004)

**Background**: Microcode is low-level software embedded in processors that translates machine instructions into sequences of elementary operations called micro-operations (μ-ops). The 80386 was Intel's first 32-bit processor released in 1985, and its microcode has been largely inaccessible until now. Die shot analysis involves photographing the actual silicon chip at high resolution and tracing the physical connections to reconstruct the underlying logic.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reenigne.org/blog/80386-microcode-disassembled/">80386 microcode disassembled « Reenigne blog</a></li>
<li><a href="https://www.altusintel.com/public-yyr4pw/?tt=1779562264">I386 Microcode Disassembly Results Published | Altus Intel</a></li>
<li><a href="https://news.ycombinator.com/item?id=48247004">80386 microcode disassembled | Hacker News</a></li>

</ul>
</details>

**Discussion**: The community shows strong interest in the technical methodology, with users asking detailed questions about how high-resolution die images can be converted to functional microcode, whether the process involves identifying individual transistors, and what format the output takes. There's also discussion about ensuring the correct chip revision is analyzed given the 386's long 22-year production run.

**Tags**: `#microcode`, `#reverse-engineering`, `#computer-architecture`, `#hardware`, `#80386`

---

<a id="item-5"></a>
## [FTC fines companies $1M for fake AI 'active listening' ads](https://simonwillison.net/2026/May/22/ftc-active-listening/#atom-everything) ⭐️ 7.0/10

The FTC requires Cox Media Group and two other firms to pay nearly $1 million to settle charges that they falsely claimed their 'Active Listening' AI-powered marketing service could capture real-time consumer intent from smart device conversations. The companies actually resold email lists from data brokers while misleading customers about voice data collection. This represents significant regulatory enforcement against deceptive AI marketing claims and highlights major privacy concerns around 'active listening' technology. The case sets precedent for how AI capabilities claims will be regulated and demonstrates the FTC's commitment to protecting consumer privacy. The companies claimed to use voice data from smart devices for ad targeting but actually provided no such service, instead reselling email lists at significant markup. The FTC clarified that hiding opt-in consent for voice data collection in terms of service does not constitute adequate consent under the law.

rss · Simon Willison · May 22, 04:48

**Background**: The 'Active Listening' service was pitched in 2024 as an AI-powered advertising platform that could listen to consumers' conversations through smart devices in real time to deliver targeted ads. This technology concept raised significant privacy concerns as it suggested companies were secretly eavesdropping on private conversations. The FTC Act prohibits deceptive practices in advertising and requires genuine consent for collecting sensitive personal data like voice recordings from inside consumers' homes.

<details><summary>References</summary>
<ul>
<li><a href="https://thecyberexpress.com/ftc-ai-powered-active-listening-case/">AI-Powered Marketing Service “Active Listening” Deceived ...</a></li>
<li><a href="https://captaincompliance.com/education/ftc-cox-media-group-active-listening-ai-fine/">The FTC's $930,000 Active Listening Smackdown: What the Cox ...</a></li>
<li><a href="https://www.editorandpublisher.com/stories/ftc-cox-media-group-2-others-to-pay-nearly-1m-over-deceptive-active-listening-ai-claims,261772">FTC: Cox Media Group and 2 others to pay nearly $1M over ...</a></li>

</ul>
</details>

**Tags**: `#AI ethics`, `#privacy`, `#regulation`, `#surveillance`, `#marketing`

---

<a id="item-6"></a>
## [HTML <dl> Element Usage and Accessibility Discussion](https://benmyers.dev/blog/on-the-dl/) ⭐️ 6.0/10

A blog post examines the proper usage of the HTML <dl> (description list) element and its accessibility considerations, with community discussion revealing technical debates about ARIA compliance and semantic HTML limitations. This discussion highlights critical accessibility issues in web development, showing how improper use of semantic HTML elements like <dl> can create barriers for users relying on assistive technologies, affecting web inclusivity standards. The <dl> element has no implicit ARIA role and requires explicit role assignment when using aria-label, with strict compatibility rules between ARIA attributes and element roles that many developers find restrictive for complex layouts.

hackernews · ravenical · May 23, 13:03 · [Discussion](https://news.ycombinator.com/item?id=48247325)

**Background**: The HTML <dl> element represents a description list containing terms (<dt>) and their descriptions (<dd>), originally designed for glossaries but now used for various key-value pair presentations. Semantic HTML uses markup to reinforce the meaning of content rather than just presentation, improving accessibility and SEO. ARIA (Accessible Rich Internet Applications) provides accessibility information to assistive technologies through attributes that define roles, states, and properties.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/dl">HTML description list element - HTML | MDN - MDN Web...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Semantic_HTML">Semantic HTML - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/HTML_element">HTML element</a></li>

</ul>
</details>

**Discussion**: Community feedback reveals significant confusion about ARIA compliance rules, with some developers expressing frustration that semantic HTML elements like <dl> lack sufficient flexibility for modern design needs. Historical context shows <dl>, <dt>, and <dd> elements date back to 1985 IBM GML documentation, predating the web itself.

**Tags**: `#html`, `#accessibility`, `#web-development`, `#aria`, `#semantic-markup`

---