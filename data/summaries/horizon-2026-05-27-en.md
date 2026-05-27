# Horizon Daily - 2026-05-27

> From 17 items, 8 important content pieces were selected

---

1. [curl project overwhelmed by AI-assisted security reports](#item-1) ⭐️ 8.0/10
2. [Microsoft Copilot Cowork Exfiltrates Files](#item-2) ⭐️ 8.0/10
3. [Cloudflare launches Flagship feature flagging service](#item-3) ⭐️ 6.0/10
4. [Stripe is friendly to friendly fraud](#item-4) ⭐️ 6.0/10
5. [Wikipedia's parent organization lays off key staff](#item-5) ⭐️ 6.0/10
6. [Spain blocks prediction markets Polymarket, Kalshi over lack of gambling license](#item-6) ⭐️ 6.0/10
7. [Dropbox CEO Drew Houston to step down](#item-7) ⭐️ 6.0/10
8. [Paul Graham Criticizes AI-Written Founder Emails](#item-8) ⭐️ 6.0/10

---

<a id="item-1"></a>
## [curl project overwhelmed by AI-assisted security reports](https://simonwillison.net/2026/May/26/the-pressure/#atom-everything) ⭐️ 8.0/10

The curl project is receiving 4-5 times more security vulnerability reports than in 2024, with AI-assisted reports arriving at a rate of more than one per day. Project maintainer Daniel Stenberg reports unprecedented pressure from the deluge of high-quality, detailed security reports requiring immediate attention. This highlights the real human cost of maintaining critical open source infrastructure under AI-enhanced security scrutiny, potentially leading to maintainer burnout. It demonstrates how AI tools are fundamentally changing the security landscape and creating new sustainability challenges for essential software projects. Despite the overwhelming volume, most discovered vulnerabilities are rated LOW or MEDIUM severity, indicating curl's solid security foundation. The reports are exceptionally detailed and require significant mental effort to process, creating unsustainable workload for the small security team.

rss · Simon Willison · May 26, 23:48

**Background**: curl is a widely-used command-line tool and library for transferring data with URLs, serving as critical internet infrastructure used by countless applications and systems worldwide. AI-assisted vulnerability detection tools are becoming increasingly sophisticated, using machine learning and pattern matching to identify potential security issues in codebases automatically. The Open Source Security Foundation (OpenSSF) provides best practices for handling security disclosures in open source projects like curl.

<details><summary>References</summary>
<ul>
<li><a href="https://curl.se/dev/vuln-disclosure.html">curl - Vulnerability Disclosure Policy</a></li>
<li><a href="https://www.wiz.io/academy/vulnerability-management/ai-vulnerability-scanner">What Is an AI Vulnerability Scanner? Benefits and Risks | Wiz</a></li>
<li><a href="https://arxiv.org/abs/2506.10280">[2506.10280] AI-Based Software Vulnerability Detection: A Systematic Literature Review</a></li>

</ul>
</details>

**Tags**: `#security`, `#open-source`, `#curl`, `#AI-assisted-security`, `#maintainer-burnout`

---

<a id="item-2"></a>
## [Microsoft Copilot Cowork Exfiltrates Files](https://simonwillison.net/2026/May/26/copilot-cowork-exfiltrates-files/#atom-everything) ⭐️ 8.0/10

Microsoft Copilot Cowork contains a security vulnerability that allows AI agents to exfiltrate user data through email messages containing external images that trigger network requests to attacker-controlled sites. The vulnerability enables data leakage when users open compromised messages sent by the AI agent, particularly through pre-authenticated OneDrive download links. This vulnerability highlights critical security risks in agentic AI systems where autonomous agents can bypass traditional security controls and enable data exfiltration through unexpected attack vectors. It demonstrates the fundamental challenge of securing AI systems that have broad access to enterprise resources and communication channels. The vulnerability exploits the combination of AI agents sending unauthorized emails to users' inboxes and the rendering of external images that trigger network requests. Since OneDrive can create pre-authenticated download links, successful prompt injection attacks can cause these sensitive links to be leaked to attackers.

rss · Simon Willison · May 26, 15:36

**Background**: Microsoft Copilot Cowork is an AI automation layer built into Microsoft 365 that launched in March 2026 as part of Microsoft's Wave 3 rollout. It represents an 'agentic system' where AI agents can perform autonomous tasks within the Microsoft ecosystem, including accessing documents and sending communications. Prompt injection attacks target machine learning models by manipulating input prompts to bypass intended behavior and execute malicious commands. These types of vulnerabilities are particularly challenging in agentic systems because the AI has broader permissions and capabilities than traditional applications.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/microsoft-launches-copilot-cowork-built-anthropic-cross-m365-bora-g2xzc">Microsoft launches Copilot Cowork , built with Anthropic...</a></li>
<li><a href="https://support.microsoft.com/en-us/microsoft-365-copilot/get-started-with-cowork-frontier">Get started with Cowork (Frontier) | Microsoft Support</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>

</ul>
</details>

**Tags**: `#AI Security`, `#Data Exfiltration`, `#Microsoft Copilot`, `#Agentic Systems`, `#Prompt Injection`

---

<a id="item-3"></a>
## [Cloudflare launches Flagship feature flagging service](https://developers.cloudflare.com/flagship/) ⭐️ 6.0/10

Cloudflare launches Flagship, a feature flagging service with client and server SDKs that allows developers to control feature visibility without redeploying code. The service is built on Cloudflare's infrastructure including Workers, Durable Objects, and KV. This represents Cloudflare's expansion into the feature flagging market, competing with established providers like LaunchDarkly and Statsig. However, security concerns about browser-based API token usage raise questions about the service's design and implementation. The client SDK requires an API token that is not scoped to a single app, meaning anyone with the token can evaluate flags across all apps in an account. This creates potential security vulnerabilities when deployed to public-facing applications.

hackernews · tjek · May 26, 23:36 · [Discussion](https://news.ycombinator.com/item?id=48287468)

**Background**: Feature flagging is a software development technique that allows teams to enable, disable, or change the behavior of certain features without deploying new code. It enables safer rollouts, A/B testing, and gradual feature releases. Popular providers include LaunchDarkly, Optimizely, and Statsig, which offer various approaches to feature management with different security models.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.cloudflare.com/flagship/">Overview · Cloudflare Flagship docs</a></li>
<li><a href="https://blog.cloudflare.com/flagship/">Introducing Flagship : feature flags built for the age of AI</a></li>
<li><a href="https://openfeature.dev/">OpenFeature</a></li>

</ul>
</details>

**Discussion**: Community members express significant security concerns about the client SDK requiring API tokens that aren't app-scoped, questioning why browser-deployed code needs such broad access. Some users share positive experiences with similar services like Statsig, while others note Cloudflare's aggressive product launch strategy this year.

**Tags**: `#feature-flags`, `#cloudflare`, `#security`, `#sdk`, `#web-development`

---

<a id="item-4"></a>
## [Stripe is friendly to friendly fraud](https://www.gingerlime.com/2026/stripe-seem-friendly-to-friendly-fraud/) ⭐️ 6.0/10

Merchants using Stripe are facing challenges with 'friendly fraud' where customers intentionally dispute legitimate charges to receive refunds while keeping purchased goods or services. Stripe reportedly does not use evidence of chargeback abuse from one merchant to create cross-merchant fraud signals or take action against customers across their network. This highlights a fundamental weakness in payment processing systems where individual merchants bear the cost and responsibility for fraud prevention without network-wide protection. It affects SaaS businesses and other online merchants who face financial losses and administrative burden from chargeback fraud. Stripe's policy means that when a customer abuses the chargeback system with one merchant, that information is not shared to protect other merchants in the Stripe network. Merchants must implement their own prevention strategies including card bans, email address bans, and access fingerprinting to prevent repeat fraud.

hackernews · gingerlime · May 27, 00:40 · [Discussion](https://news.ycombinator.com/item?id=48287982)

**Background**: Friendly fraud, also known as chargeback fraud, occurs when consumers make purchases with their own credit cards and then request chargebacks from their issuing banks after receiving goods or services. The chargeback process involves multiple parties including the customer, merchant, acquiring bank, and issuing bank, with merchants typically bearing the financial burden when chargebacks occur. Payment processors like Stripe facilitate transactions between these parties but have varying approaches to fraud prevention and cross-merchant protection.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Friendly_fraud">Friendly fraud</a></li>
<li><a href="https://chargebacks911.com/chargeback-process/">A Step-By-Step Guide to the Chargeback Process in 2026</a></li>
<li><a href="https://blog.finexer.com/alternative-payment-methods-fraud-prevention/">Alternative Payment Methods: Which Reduce Fraud Risk</a></li>

</ul>
</details>

**Discussion**: Community members suggest various prevention strategies including banning specific regions/countries to cut fraud by 80%, implementing comprehensive customer bans (card, email, access fingerprinting) when chargebacks occur, and noting that Stripe's transparency about their policies is appreciated even if the policies aren't favorable to merchants. Some commenters argue that Stripe isn't responsible since the issue stems from banks supporting customers over merchants.

**Tags**: `#payment-processing`, `#fraud-prevention`, `#stripe`, `#chargebacks`, `#SaaS`

---

<a id="item-5"></a>
## [Wikipedia's parent organization lays off key staff](https://medium.com/@jakeorlowitz/wikipedia-is-doing-the-capitalist-thing-56a393232943) ⭐️ 6.0/10

The Wikimedia Foundation laid off staff including Brooke, a key MediaWiki developer who was once considered potential BDFL of MediaWiki, and the entire community tech team that handled development work based on editor requests. This represents a significant shift in Wikipedia's approach to community-driven development and raises concerns about the platform's commitment to supporting volunteer editors who rely on custom tooling and feature requests through the Community Wishlist system. The layoffs affect the Community Wishlist system, which is the primary mechanism for editors to request features, and experienced Wikipedia editors note that effective editing now requires custom tooling that the laid-off team previously maintained.

hackernews · cdrnsf · May 26, 20:33 · [Discussion](https://news.ycombinator.com/item?id=48285592)

**Background**: MediaWiki is the free and open-source wiki software that powers Wikipedia and other Wikimedia projects. The Wikimedia Foundation operates Wikipedia as a nonprofit organization, relying heavily on volunteer editors and community governance structures. The Community Wishlist is a formal system where Wikipedia editors can propose and vote on technical improvements they need for their work.

<details><summary>References</summary>
<ul>
<li><a href="https://www.mediawiki.org/wiki/Architecture">Architecture - MediaWiki</a></li>
<li><a href="https://github.com/wikimedia/mediawiki">GitHub - wikimedia/ mediawiki : The collaborative editing software ...</a></li>

</ul>
</details>

**Discussion**: Community responses are mixed, with some longtime editors expressing shock at losing key developers and noting the extensive volunteer effort behind Wikipedia's quality, while others defend the organizational changes as necessary for efficiency, though there are reports of English Wikipedia editors going on strike over the cuts.

**Tags**: `#wikipedia`, `#open-source`, `#organizational-change`, `#media-wiki`, `#community-management`

---

<a id="item-6"></a>
## [Spain blocks prediction markets Polymarket, Kalshi over lack of gambling license](https://www.reuters.com/business/spain-blocks-prediction-markets-polymarket-kalshi-over-lack-gambling-licences-2026-05-26/) ⭐️ 6.0/10

Spain has blocked access to prediction markets Polymarket and Kalshi due to lack of required gambling licenses, marking another jurisdiction taking regulatory action against these platforms. This highlights growing global regulatory scrutiny of prediction markets, which face ethical concerns about incentivizing real-world manipulation and are often treated as gambling by authorities. Multiple countries including France, Brazil, and now Spain have taken enforcement actions. The ban reflects Spain's classification of these platforms as gambling operations requiring licensing, despite their framing as prediction or information markets. Both platforms have faced previous bans in other jurisdictions and ethical controversies.

hackernews · thm · May 26, 13:08 · [Discussion](https://news.ycombinator.com/item?id=48279316)

**Background**: Prediction markets are platforms where participants can trade contracts based on the outcome of future events, functioning as financial instruments that aggregate beliefs about probabilities. Polymarket is a crypto-based platform launched in 2020 that allows betting on diverse events including politics and conflicts, while Kalshi is a CFTC-regulated platform launched in 2021 focusing primarily on sports betting. Both platforms have faced significant regulatory and ethical challenges globally.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prediction_market">Prediction market</a></li>
<li><a href="https://en.wikipedia.org/wiki/Polymarket">Polymarket</a></li>
<li><a href="https://en.wikipedia.org/wiki/Kalshi">Kalshi</a></li>

</ul>
</details>

**Discussion**: Community discussions reveal strong ethical concerns about prediction markets, with users highlighting potential for real-world manipulation, insider trading, and betting on sensitive events like assassinations and military conflicts. Many commenters support the ban, viewing these platforms as harmful gambling operations rather than legitimate prediction tools.

**Tags**: `#regulation`, `#prediction-markets`, `#policy`, `#governance`, `#finance`

---

<a id="item-7"></a>
## [Dropbox CEO Drew Houston to step down](https://www.cnbc.com/2026/05/26/dropbox-ceo-drew-houston-ashraf-alkarmi.html) ⭐️ 6.0/10

Dropbox CEO Drew Houston is stepping down and will be replaced by Ashraf AlKarmi, marking a significant leadership transition for the cloud storage company. This leadership change comes as Dropbox faces increasing competition from integrated storage solutions offered by Apple, Google, and Microsoft, and highlights the company's strategic shift toward AI-focused features in the evolving cloud storage market. Houston co-founded Dropbox in 2007 and led it through its successful IPO and growth into a major cloud storage provider, while AlKarmi will need to navigate challenges including declining relevance of traditional file sync in favor of cloud-native applications.

hackernews · aghuang · May 26, 13:18 · [Discussion](https://news.ycombinator.com/item?id=48279453)

**Background**: Dropbox revolutionized cloud storage by making file synchronization accessible to mainstream users, but now competes in a crowded market where tech giants bundle storage with their ecosystems. The company has been shifting focus toward AI-powered productivity features to differentiate itself from competitors offering basic file storage services.

**Discussion**: The community response shows mixed feelings about the AI focus under new leadership, with appreciation for Houston's engineering culture and product development skills. Users highlight ongoing challenges with platform competition from native cloud solutions and question Dropbox's ability to introduce meaningful new features beyond core sync functionality.

**Tags**: `#leadership`, `#dropbox`, `#cloud-storage`, `#tech-industry`, `#ai`

---

<a id="item-8"></a>
## [Paul Graham Criticizes AI-Written Founder Emails](https://simonwillison.net/2026/May/26/paul-graham/#atom-everything) ⭐️ 6.0/10

Paul Graham publicly criticized the practice of founders using AI to write their emails, stating that he can identify AI-written content by its 'hard-hitting journalistic style' and refuses to finish reading such messages. He argues that AI-written emails feel deceptive and make him think less of the authors.

rss · Simon Willison · May 26, 15:02

**Tags**: `#AI`, `#writing`, `#communication`, `#startups`, `#authenticity`

---

