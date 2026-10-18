---
theme: ./slidev-theme-aalto-scicomp
themeConfig:
  palette: aalto-classic
  titles: aalto
  credit:
    text: Enrico Glerean · CC BY 4.0
    url: https://eglerean.github.io/
  download:
    url: /slides.pdf
    text: Download PDF
favicon: https://eglerean.github.io/favicon.svg
title: AI tools, Research Integrity and Ethics
author: Enrico Glerean
info: |
  Slides by Enrico Glerean (https://eglerean.github.io/), CC BY 4.0.
  Course: LC-L1000 Research Ethics for Doctoral Students
  Source: https://github.com/eglerean/genAI_researchintegrity
keywords: generative AI, AI tools, research integrity, research ethics, Enrico Glerean, https://eglerean.github.io/
layout: cover
class: no-footer
hexText: "Gen AI\nINTEGRITY"
hexSeed: 7
---

###### LC-L1000 Research Ethics for Doctoral Students

# AI tools, Research Integrity and Ethics

Responsible conduct of research with generative AI tools


::presenter::
**Enrico Glerean**, Staff Scientist, Aalto University, October 2026

<div class="license-line"><CcBy /> <a href="https://creativecommons.org/licenses/by/4.0/">CC BY 4.0</a> · <a href="https://github.com/eglerean/genAI_researchintegrity" class="gh-link" title="Slides on GitHub" aria-label="Slides on GitHub"><carbon-logo-github class="gh-icon" /></a></div>

<style>
h1 { font-size: 2.5rem !important; line-height: 1.1 !important; }
p { font-size: 0.95rem; }
.cover-presenter p { font-size: 0.85rem; }
.license-line { margin-top: 0.45rem; font-size: 0.75rem; white-space: nowrap; }
.gh-icon { vertical-align: -0.2em; width: 1.15em; height: 1.15em; }
.license-line a.gh-link { border-bottom: none; text-decoration: none; color: inherit; }
</style>

---
layout: section
color: dark
hexText: "AI?"
class: title-middle
---

# What is AI?


---
layout: three-cols
---

::header::
# What is AI in research? Topic, method, tool

<div class="ref-line">Reference: <a href="https://www.aalto.fi/en/research-art/best-practices-for-ai-use-in-research-work">Best practices for AI use in research work (Aalto.fi)</a></div>

::left::

### AI as a **topic**

AI is what is being studied.

- A new ML model or architecture
- A new algorithm for training
- How people interact with AI chatbots

::center::

### AI as a **method**

AI is how the data are analysed.

- A deep neural network that classifies tissue in cancer imaging data
- A scikit-learn model in the analysis of a dataset

::right::

### AI as a **tool**

AI is something that helps with the work.

- Brainstorming with a chatbot
- A coding agent writing analysis scripts
- An AI assistant helping to fill in a data management plan

<p class="small">Invisible AI: in word processors, search engines, translation, transcription tools, automatic meeting note-takers.</p>



---
layout: default
---

# Generative AI and Research Integrity

<div class="ref-line">Figure adapted from Glerean (2025) <a href="https://www.edpb.europa.eu/our-work-tools/our-documents/support-pool-experts-projects/fundamentals-secure-ai-systems-personal_en">“Fundamentals of secure AI systems with personal data”</a>, European Data Protection Board</div>

<p>For simplicity we focus on <strong>generative AI systems</strong> that use <strong>General Purpose AI models</strong> such as <strong>Large Language Models</strong> that can be used in your research work,  including <strong>agentic AI</strong> systems.</p>

<div class="grid-2-3">
  <div class="card">
    <h3>Generating one modality from another</h3>
    <ul>
      <li>Text → Text</li>
      <li>Text → Code</li>
      <li>Speech → Text</li>
      <li>Text → Speech</li>
      <li>Text → Image</li>
      <li>Image → Text</li>
      <li>…</li>
    </ul>
  </div>
  <div class="card dark ai-sys-diagram">
    <div class="asd-io-wrap asd-in">
      <div class="asd-io"><div class="asd-label">Data &amp; Input</div></div>
      <div class="asd-sample small">“Translate this email from English to Finnish: Hi Annukka, the AI lecture of our…”</div>
    </div>
    <div class="asd-arrow asd-in">→</div>
    <div class="asd-system">
      <div class="asd-label">AI system</div>
      <div class="asd-sub">e.g. a chatbot</div>
      <div class="asd-model">
        <div class="asd-label">AI model</div>
        <div class="asd-sub">e.g. a Large Language Model</div>
      </div>
    </div>
    <div class="asd-io-wrap asd-out">
      <div class="asd-io"><div class="asd-label">Outputs</div></div>
      <div class="asd-sample small">“Hei Annukka, tutkimusetiikan kurssimme tekoälyluento on…”</div>
    </div>
    <div class="asd-arrow asd-out">←</div>
  </div>
</div>

<style>
/* Dark box: inputs (top) go into the AI system, which wraps the AI model; outputs (bottom) come back out on the same side.
   Same look as the agent diagram (Harness and Model boxes) */
.ai-sys-diagram { display: grid; grid-template-columns: minmax(0, 1fr) auto minmax(0, 1fr); grid-template-rows: 1fr 1fr; gap: 0.5rem 0.6rem; align-items: center; }
.ai-sys-diagram .asd-label { font-family: var(--asc-font-serif); font-weight: 600; font-size: 1.1rem; }
.ai-sys-diagram .asd-sub { font-size: 0.8rem; opacity: 0.8; }
.asd-in { grid-row: 1; }
.asd-out { grid-row: 2; }
/* Example prompt and output under the two boxes, in small monospace text */
.asd-io-wrap { grid-column: 1; }
.asd-sample { margin-top: 0.4rem; font-family: var(--asc-font-mono); opacity: 0.85; }
.asd-io { padding: 0.8rem 0.9rem; text-align: center; background: var(--asc-night-raised); border: 1px solid rgba(250, 249, 245, 0.3); border-radius: var(--asc-radius-md); }
.asd-arrow { grid-column: 2; font-size: 1.6rem; line-height: 1; color: var(--asc-clay); }
.asd-system { grid-column: 3; grid-row: 1 / span 2; align-self: stretch; display: flex; flex-direction: column; padding: 0.8rem 1rem 1rem; border: 2px solid var(--asc-clay); border-radius: var(--asc-radius-lg); }
.asd-system .asd-model { flex: 1; margin-top: 0.6rem; display: flex; flex-direction: column; justify-content: center; padding: 1rem 0.9rem; text-align: center; background: var(--asc-clay); color: var(--asc-ink); border-radius: var(--asc-radius-md); }
.asd-model .asd-sub { opacity: 0.85; }
</style>

---
layout: default
---

# The Research Process aided by AI tools

<div class="ref-line">with Responsible Conduct of Research at its core. Wheel adapted from <a href="https://rdmkit.elixir-europe.org/">RDMkit, “The data lifecycle”</a></div>

<div class="rdm-wheel">
<svg class="rw-svg" viewBox="-165 -165 330 330" role="img" aria-label="Research data lifecycle wheel: Plan, Collect, Process, Analyse, Preserve, Share, Reuse, around Responsible Conduct of Research, ethics and law">
  <path d="M22.0 -158.5 A160 160 0 0 1 135.4 -85.2 L117.7 -55.3 L84.6 -53.3 A100 100 0 0 0 13.7 -99.1 L33.4 -125.6 Z" style="fill: var(--aalto-orange)" />
  <path d="M137.6 -81.6 A160 160 0 0 1 151.1 52.8 L116.6 57.5 L94.4 33.0 A100 100 0 0 0 86.0 -51.0 L119.1 -52.2 Z" style="fill: var(--aalto-darkyellow)" />
  <path d="M149.6 56.7 A160 160 0 0 1 52.9 151.0 L27.7 127.0 L33.1 94.4 A100 100 0 0 0 93.5 35.4 L115.0 60.5 Z" style="fill: var(--aalto-green)" />
  <path d="M49.0 152.3 A160 160 0 0 1 -85.0 135.5 L-82.0 100.9 L-53.2 84.7 A100 100 0 0 0 30.6 95.2 L24.4 127.7 Z" style="fill: var(--aalto-aquagreen)" />
  <path d="M-88.6 133.3 A160 160 0 0 1 -159.0 18.0 L-130.0 -1.2 L-99.4 11.3 A100 100 0 0 0 -55.4 83.3 L-84.6 98.7 Z" style="fill: var(--aalto-blue)" />
  <path d="M-159.4 13.8 A160 160 0 0 1 -113.2 -113.1 L-80.1 -102.4 L-70.8 -70.7 A100 100 0 0 0 -99.6 8.6 L-129.9 -4.6 Z" style="fill: var(--aalto-violet)" />
  <path d="M-110.2 -116.0 A160 160 0 0 1 17.8 -159.0 L30.1 -126.5 L11.1 -99.4 A100 100 0 0 0 -68.9 -72.5 L-77.4 -104.5 Z" style="fill: var(--aalto-red)" />
  <text x="77.1" y="-104.7" class="rw-label">Plan</text>
  <text x="129.9" y="-5.0" class="rw-label">Collect</text>
  <text x="84.9" y="98.4" class="rw-label">Process</text>
  <text x="-24.0" y="127.8" class="rw-label">Analyse</text>
  <text x="-114.9" y="60.9" class="rw-label">Preserve</text>
  <text x="-119.2" y="-51.8" class="rw-label">Share</text>
  <text x="-33.8" y="-125.5" class="rw-label">Reuse</text>
  <text y="-8" class="rw-core-text rw-core-big">RCR</text>
  <text y="18" class="rw-core-text">Ethics &amp; Law</text>
</svg>
  <div class="rw-box" style="--stage: var(--aalto-orange); left: 540px; top: 14px"><ul class="small">
      <li>Grant writing</li>
      <li>Research planning</li>
      <li>Study design</li>
      <li>Browsing and summarising the literature</li>
    </ul></div>
  <div class="rw-box" style="--stage: var(--aalto-darkyellow); left: 576px; top: 126px"><ul class="small">
      <li>Interfaces for data collection</li>
      <li>Code and automation help</li>
      <li>Synthetic data generation</li>
    </ul></div>
  <div class="rw-box" style="--stage: var(--aalto-green); left: 546px; top: 253px"><ul class="small">
      <li>Brainstorming on approaches for data preprocessing</li>
      <li>Code and automation</li>
      <li>Data minimisation (pseudo- and anonymisation)</li>
      <li>Data annotation (e.g. deductive coding)</li>
    </ul></div>
  <div class="rw-box" style="--stage: var(--aalto-aquagreen); left: 111px; top: 301px"><ul class="small">
      <li>Annotations</li>
      <li>Methodological considerations</li>
      <li>Data analysis (code and automation)</li>
    </ul></div>
  <div class="rw-box" style="--stage: var(--aalto-blue); left: 23px; top: 215px"><ul class="small">
      <li>Metadata preparation</li>
      <li>Summarising</li>
      <li>Organising and storing (meta)data</li>
    </ul></div>
  <div class="rw-box" style="--stage: var(--aalto-violet); left: 15px; top: 84px"><ul class="small">
      <li>Writing and editing</li>
      <li>Improving research outputs (tables, figures)</li>
      <li>Peer review simulation</li>
      <li>Summarising for the public</li>
      <li>Media outreach</li>
    </ul></div>
  <div class="rw-box" style="--stage: var(--aalto-red); left: 87px; top: 0px"><ul class="small">
      <li>Facilitating discovery and FAIRness</li>
      <li>Exploring open datasets</li>
      <li>Identifying research gaps</li>
    </ul></div>
</div>

<style>
/* Wheel with each example card placed so that its inner corner touches its own wedge (positions computed for a 290px wheel) */
.rdm-wheel { position: relative; height: 380px; }
.rw-svg { position: absolute !important; left: 297px; top: 35px; width: 290px; height: 290px; }
.rw-label { text-anchor: middle; dominant-baseline: middle; font-weight: 700; font-size: 14px; fill: #fff; }
.rw-core-text { text-anchor: middle; dominant-baseline: middle; font-size: 16px; fill: var(--asc-text); }
.rw-core-big { font-size: 30px; font-weight: 700; }
.rw-box { position: absolute !important; width: 290px; padding: 0.3rem 0.6rem; background: var(--asc-surface); border: 2px solid var(--stage); border-radius: var(--asc-radius-md); }
.rw-box ul { margin: 0; }
/* Black bullets here: the default blue bullet would read as another stage colour */
.rw-box li::before { background: #000; }
/* Smaller text, so half the theme's bullet-to-text gap (bullet left from -1.15rem to -0.68rem; list indent shrinks by the same amount) */
.rw-box ul { padding-left: 0.93rem; }
.rw-box li::before { left: -0.68rem; }
</style>

---
layout: section
color: dark
hexText: "AI\nETHICS"
class: title-middle
---

# Framework for AI ethics and responsible AI





---
layout: default
---

# AI ethics, Responsible AI, AI governance and AI regulations

<div class="pyramid">
<svg viewBox="0 0 600 420" role="img" aria-label="Pyramid: AI Ethics at the base, Responsible AI in the middle, AI governance and regulations at the top">
  <polygon class="p-bottom" points="118,290 482,290 560,410 40,410" />
  <polygon class="p-middle" points="196,170 404,170 482,290 118,290" />
  <polygon class="p-top" points="300,10 196,170 404,170" />
  <text x="300" y="358" class="p-label">AI Ethics</text>
  <text x="300" y="238" class="p-label">Responsible AI</text>
  <text x="300" class="p-label">
    <tspan x="300" y="105">AI</tspan> 
    <tspan x="300" y="130">governance</tspan>
    <tspan x="300" y="155">&amp; regulations</tspan>
  </text>
</svg>
<div class="p-cards">
  <div class="card p-card">
    AI Governance in Practice <span class="p-src">(<a href="https://www.turing.ac.uk/research/research-projects/ai-ethics-and-governance-practice">The Alan Turing Institute</a>)</span><br>
    <a href="https://eur-lex.europa.eu/eli/reg/2024/1689/oj/eng">Artificial Intelligence Act</a>
  </div>
  <div class="card p-card">
    SSAFE-D <span class="p-src">(<a href="https://www.turing.ac.uk/research/research-projects/ai-ethics-and-governance-practice">The Alan Turing Institute</a>)</span><br>
    EU: 7 requirements for <a href="https://digital-strategy.ec.europa.eu/en/library/ethics-guidelines-trustworthy-ai">Trustworthy AI</a> (HLEG 2019)
  </div>
  <div class="card p-card">
    Beneficence, Non-maleficence, Autonomy, Justice, Explicability <span class="p-src"><a href="https://academic.oup.com/book/46748">(Floridi 2023)</a></span>
  </div>
</div>
</div>

<style>
/* Pyramid on the left; the card column uses the same 420-unit height split as the slices (0-170, 170-290, 290-420) so each card sits beside its slice */
.pyramid { display: grid; grid-template-columns: auto 1fr; gap: 1rem; height: 360px; }
.pyramid svg { height: 100%; width: auto; }
.pyramid .p-cards { display: grid; grid-template-rows: 120fr 120fr 120fr; height: 100%; }
.pyramid .p-card { align-self: center; }
.pyramid .p-src { color: var(--asc-muted); }
.pyramid polygon { stroke: var(--asc-bg, #fff); stroke-width: 6; stroke-linejoin: round; }
.pyramid .p-bottom { fill: var(--aalto-red); }
.pyramid .p-middle { fill: var(--aalto-yellow); }
.pyramid .p-top { fill: var(--aalto-green); }
.pyramid .p-label { text-anchor: middle; font-weight: 700; font-size: 24px; fill: #000; }
.pyramid .p-small { font-size: 17px; }
</style>

---
layout: default
---

# Unified framework of five principles for ethical AI

<div class="corner-icon"><img src="/images/AIpyramid_1.png" alt="AI pyramid, level: AI ethics"></div>
<br>
<div class="five-principles">
  <img src="/images/unified-five-principles.png" alt="Diagram: traditional bioethics principles lead to Beneficence, Non-maleficence, Autonomy and Justice; a new enabling principle for AI leads to Explicability">
</div>

<div class="ref-bottom">Reference: Traditional bioethics principles by <a href="https://archive.org/details/principlesofbiom0000beau_k8c1">Beauchamp &amp; Childress</a> (1979-2026), extended by Floridi, L. (2023) in “<a href="https://academic.oup.com/book/46748">The ethics of artificial intelligence: Principles, challenges, and opportunities.</a>”. Original image from <a href="https://www.edpb.europa.eu/documents/support-pool-of-experts/fundamentals-of-secure-ai-systems-with-personal-data_en">Glerean (2025) "Fundamentals of secure AI systems with personal data" European Data Protection Board</a></div>

<style>
.five-principles { display: flex; justify-content: center; margin-top: 2rem; }
.five-principles img { width: 100%; max-width: 820px; height: auto; }
</style>

---
layout: default
---

# Responsible AI, the SSAFE-D principles

<div class="corner-icon"><img src="/images/AIpyramid_2.png" alt="AI pyramid, level: Responsible AI"></div>

<div class="ref-line"><strong>SSAFE-D</strong>: Sustainability, Safety, Accountability, Fairness, Explainability, Data Stewardship (<a href="https://www.turing.ac.uk/research/research-projects/ai-ethics-and-governance-practice">The Alan Turing Institute</a>)</div>

<div class="grid-3">
  <div class="card sd-card" style="--c: var(--aalto-green)"><div class="sd-tri">S</div><div><h3>Sustainability</h3><p class="small">Achieving this goal requires assuring AI projects being developed with continuous sensitivity to real-world impacts.</p></div></div>
  <div class="card sd-card" style="--c: var(--aalto-red)"><div class="sd-tri">S</div><div><h3>Safety</h3><p class="small">Achieving this goal requires an AI system to be technically accurate, reliable, secure, and robust.</p></div></div>
  <div class="card sd-card" style="--c: var(--aalto-blue)"><div class="sd-tri">A</div><div><h3>Accountability</h3><p class="small">Achieving this goal requires assuring the project’s end-to-end answerability and auditability.</p></div></div>
  <div class="card sd-card" style="--c: var(--aalto-orange)"><div class="sd-tri">F</div><div><h3>Fairness</h3><p class="small">Achieving this goal requires assuring a minimum threshold of discriminatory non-harm and bias mitigation.</p></div></div>
  <div class="card sd-card" style="--c: var(--aalto-violet)"><div class="sd-tri">E</div><div><h3>Explainability</h3><p class="small">Achieving this goal requires the ability to explain and justify AI project processes and AI-supported outcomes.</p></div></div>
  <div class="card sd-card" style="--c: var(--aalto-aquagreen)"><div class="sd-tri">D</div><div><h3>Data Stewardship</h3><p class="small">Achieving this goal requires data quality, integrity, protection, and privacy to be assured.</p></div></div>
</div>


<style>
.sd-card { display: flex; gap: 1rem; align-items: flex-start; }
/* The letter is part of the triangle graphic, not text */
.sd-tri { flex: none; width: 3rem; height: 2.6rem; clip-path: polygon(50% 0, 100% 100%, 0 100%); background: var(--c); color: #000; font-weight: 700; font-size: 1.1rem; display: flex; align-items: flex-end; justify-content: center; padding-bottom: 0.15rem; }
</style>

---
layout: default
---

# SSAFE-D applied: how ethical are AI tools?

<div class="corner-icon"><img src="/images/AIpyramid_2.png" alt="AI pyramid, level: Responsible AI"></div>

<div class="ref-line">Responsible AI principles are currently not followed by the majority of developers of generative AI systems/models (OpenAI, Anthropic, Meta, Google, xAI…)</div>

<div class="sd-eval">
  <p>❌ <strong>Sustainability</strong>: huge impact on the planet; data centres use about 1.5% of global electricity, set to double by 2030 (<a href="https://www.iea.org/reports/energy-and-ai/energy-demand-from-ai">IEA</a>) (<a href="https://arxiv.org/abs/2510.09022">Morand et al. 2026</a>)</p>
  <p>❌ <strong>Safety</strong>: induced <a href="https://www.reuters.com/investigates/special-report/meta-ai-chatbot-death/">death</a>, <a href="https://www.theguardian.com/technology/2025/aug/27/chatgpt-scrutiny-family-teen-killed-himself-sue-open-ai">suicide</a>, <a href="https://www.cnn.com/2026/01/07/business/character-ai-google-settle-teen-suicide-lawsuit">teen-harm lawsuits settled</a> (2026), <a href="https://abc17news.com/money/cnn-business-consumer/2026/06/01/florida-sues-openai-alleging-its-unsafe-for-children/">Florida sues OpenAI</a> (2026), <a href="https://www.vice.com/en/article/openai-used-kenyan-workers-making-dollar2-an-hour-to-filter-traumatic-content-from-chatgpt/">exploitation</a> of global-south annotators and sycophancy (<a href="https://www.science.org/doi/10.1126/science.aec8352">Cheng et al.,  2026</a>; <a href="https://dl.acm.org/doi/full/10.1145/3715275.3732039">Moore et al. 2025</a>)</p>
  <p>❌ <strong>Accountability</strong>: few consequences for harming individuals; Grok's sexualised deepfakes led to <a href="https://www.cnbc.com/2026/01/05/india-eu-investigate-musks-x-after-grok-created-deepfake-child-porn.html">investigations</a> (2026), but Canada's regulator <a href="https://www.aljazeera.com/economy/2026/6/11/musks-grok-accused-of-violating-canadian-privacy-laws-on-deepfakes">cannot fine xAI</a> (<a href="https://arxiv.org/abs/2512.01166">Stelling et al. 2026</a>; <a href="https://internationalaisafetyreport.org/publication/international-ai-safety-report-2026">Int. AI Safety Report 2026</a>)</p>
  <p>❌ <strong>Fairness</strong>: biases against <a href="https://www.theguardian.com/technology/2024/mar/16/ai-racism-chatgpt-gemini-bias">Black people</a>, women, minorities (<a href="https://www.nature.com/articles/s41586-024-07856-5">Hofmann et al., 2024</a>; <a href="https://www.nature.com/articles/s41586-025-09581-z">Guilbeault et al., 2025</a>)</p>
  <p>❌ <strong>Explainability</strong>: proprietary models, no clear explanation of how they work; company <a href="https://news.stanford.edu/stories/2025/12/foundation-model-transparency-index-ai-companies-information">transparency fell</a> in 2025 (<a href="https://arxiv.org/abs/2505.05410">Chen et al. 2025</a>)</p>
  <p>❌ <strong>Data Stewardship</strong>: training data kept secret, illegal use of copyrighted material (<a href="https://www.jurist.org/news/2026/07/judge-approves-record-1-5-billion-settlement-involving-anthropic/">$1.5B settlement for pirated books</a>, 2026), Stable Diffusion even reproduced <a href="https://www.theverge.com/2023/2/6/23587393/ai-art-copyright-lawsuit-getty-images-stable-diffusion">Getty Images watermarks</a> (UK, 2023-2025), unauthorised <a href="https://europeanlawblog.eu/2klfhf06/">processing of personal data</a>, near-verbatim extraction of books from LLMs (<a href="https://arxiv.org/abs/2601.02671">Ahmed et al. 2026</a>)</p>
</div>

<div class="ref-bottom">Check these references for more: <a href="https://www.sciencedirect.com/science/article/pii/S0268401223000816">Stahl &amp; Eke (2024) “The Ethics of ChatGPT”</a> · <a href="https://thecon.ai/">Bender &amp; Hanna (2025) “The AI Con”</a></div>

---
layout: default
---

# AI regulations: EU AI Act

<div class="corner-icon"><img src="/images/AIpyramid_3..png" alt="AI pyramid, level: AI governance and regulations"></div>

<div class="ref-line"><a href="https://eur-lex.europa.eu/eli/reg/2024/1689/oj/eng">Regulation (EU) 2024/1689</a>: a risk-based approach. Most task-specific AI tools are minimal risk; general-purpose AI models (e.g. GPT, Gemini, Claude) have their own rules.</div>

<div class="grid-3">
  <div class="card">
    <h3>Prohibited</h3>
    <p class="aia-when">Unacceptable risk · since 2 Feb 2025</p>
    <ul class="small">
      <li>Social scoring</li>
      <li>Manipulation, exploiting vulnerabilities</li>
      <li>Untargeted scraping of face images</li>
      <li>Emotion recognition at work and in education</li>
      <li>Predicting crime from profiling alone</li>
      <li>Non-consensual intimate deepfakes (from 2 Dec 2026)</li>
    </ul>
  </div>
  <div class="card">
    <h3>High risk</h3>
    <p class="aia-when">Strict requirements · from 2 Dec 2027</p>
    <ul class="small">
      <li>Education: admission, grading, proctoring</li>
      <li>Employment: hiring, evaluating workers</li>
      <li>Access to credit and essential services</li>
      <li>Law enforcement, migration, justice</li>
      <li>Risk management, data quality, documentation, human oversight</li>
    </ul>
  </div>
  <div class="card">
    <h3>Transparency</h3>
    <p class="aia-when">Limited risk · since 2 Aug 2026</p>
    <ul class="small">
      <li>Tell people they are talking to an AI</li>
      <li>Mark AI-generated content as machine-readable</li>
      <li>Label deepfakes</li>
      <li>Disclose emotion recognition and biometric categorisation</li>
    </ul>
  </div>
</div>

<div class="card dark">
<strong>Scope:</strong> the AI Act is a product regulation: it applies when AI is placed on the EU market or put into service. AI specifically developed and put into service for the sole purpose of scientific research and development is excluded, but if your research will become a product or a service, the Act will apply to it, so plan for it early.<br>
</div>

<style>
.aia-when { color: var(--asc-muted); }
</style>


---
layout: section
color: dark
hexText: "RESEARCH\nINTEGRITY"
class: title-middle
---

# Combining Research integrity with AI 
## [ethics|trustworthiness|governance]

---
layout: default
---

# Responsible AI and research integrity (1/2)

<div class="ref-line"><a href="https://allea.org/code-of-conduct/">ALLEA Code of Conduct</a> | <a href="https://research-and-innovation.ec.europa.eu/document/2b6cf7e5-36ac-41cb-aab5-0d32050143dc_en">EC Living Guidelines (October, 2026)</a> | <a href="https://www.aalto.fi/en/services/responsible-use-of-generative-artificial-intelligence-in-the-research-process">Aalto.fi guidelines</a> | <a href="https://tenk.fi/sites/default/files/2026-06/Artificial%20Intelligence%20in%20Research.%20TENK%27s%20Recommendation%202026.pdf">TENK 2026</a></div>

<div class="grid-2-3">
  <div class="card"><h3>Reliability</h3><p>Quality of research/education, reflected in the design, methodology, analysis, and use of resources.</p></div>
  <div class="card dark"><ul>
    <li><strong>Verify</strong> and <strong>reproduce</strong> AI-generated information; watch for bias, hallucinations, and inaccuracy</li>
    <li>Check all <strong>references</strong>, <strong>citations</strong> and <strong>summaries</strong>: AI fabricates citations and summarises real ones wrong.</li>
    <li>Output is non-deterministic: keep <strong>prompts, logs and model versions</strong> when needed to understand, reproduce, or audit the research</li>
  </ul></div>
</div>

<div class="grid-2-3">
  <div class="card"><h3>Honesty</h3><p>Doing your work in a transparent, fair, full, and unbiased way.</p></div>
  <div class="card dark"><ul>
    <li>Disclose which AI tools you used <strong>substantially</strong> and <strong>what they contributed.</strong></li>
    <li><strong>Disclose</strong> AI use that shapes your judgement or could affect results; in doubt, disclose</li>
    <li>Say <strong>how you verified</strong> the output</li>
    <li>Follow your <strong>journal's, funder's, or discipline's rules</strong></li>
  </ul></div>
</div>

---
layout: default
---

# Responsible AI and research integrity (2/2)

<div class="ref-line"><a href="https://allea.org/code-of-conduct/">ALLEA Code of Conduct</a> | <a href="https://research-and-innovation.ec.europa.eu/document/2b6cf7e5-36ac-41cb-aab5-0d32050143dc_en">EC Living Guidelines (October, 2026)</a> | <a href="https://www.aalto.fi/en/services/responsible-use-of-generative-artificial-intelligence-in-the-research-process">Aalto.fi guidelines</a> | <a href="https://tenk.fi/sites/default/files/2026-06/Artificial%20Intelligence%20in%20Research.%20TENK%27s%20Recommendation%202026.pdf">TENK 2026</a></div>

<div class="grid-2-3">
  <div class="card"><h3>Respect</h3><p>Towards colleagues, research participants, research subjects, society, cultural heritage, and the environment.</p></div>
  <div class="card dark"><ul>
    <li>Protect privacy, confidentiality, IP and <strong>research security</strong></li>
    <li><strong>Don't upload unpublished work</strong> to non-approved external tools, ask permission from other authors.</li>
    <li><strong>Cite and credit sources</strong> that AI output may reproduce</li> 
    <li>Consider sustainability: choose the <strong>lowest-impact tool</strong> for the task</li>
  </ul></div>
</div>

<div class="grid-2-3">
  <div class="card"><h3>Accountability</h3><p>From idea to publication, and all the steps of the study / teaching / research process.</p></div>
  <div class="card dark"><ul>
    <li>You remain <strong>ultimately responsible</strong> for research outputs, also when <strong>agents</strong> act for you.</li>
    <li>AI systems are <strong>neither authors nor co-authors nor owners</strong></li>
    <li>Peer review and grant evaluation: <strong>never delegate the judgement</strong>; funder and journal rules come first. Peer reviewers are the human-in-the-loop.</li>
  </ul></div>
</div>

---
layout: section
color: dark
hexText: "AI\nRISKS"
class: title-middle
---

# A framework for AI risks in research

---
layout: default
---

# AI risks in research

<div class="ref-line">Separating the different types of risks makes it easier for a researcher to assess if a certain tool can be used. <a href="https://eglerean.github.io/assets/docs/2026_05_06_AI_research_risks.pdf">Glerean, 2026.</a></div>

<div class="grid-3">
  <div class="card blue">
    <h3>Fundamental digital risks</h3>
    <ul>
      <li>Non-approved remote tools</li>
      <li>Loss of confidentiality</li>
      <li>Increased (cyber)security risks</li>
      <li>Unethical / illegal solutions sold by vendors</li>
    </ul>
  </div>
  <div class="card yellow">
    <h3>AI-amplified risks</h3>
    <ul>
      <li>Fabrication</li>
      <li>Falsification</li>
      <li>Plagiarism/IPR infringement</li>
      <li>Irreproducible research</li>
      <li>Environmental cost</li>
    </ul>
  </div>
  <div class="card red">
    <h3>AI-native risks</h3>
    <ul>
      <li>Training data bias</li>
      <li>No explainability</li>
      <li>Deskilling</li>
      <li>Erosion of autonomy and automation bias</li>
      <li>Sycophancy</li>
      <li>Impacts justice</li>
    </ul>
  </div>
</div>

<div class="card dark">
Local and open source tools can help mitigate digital risks, but we need researchers' communities to agree on when it is better to just avoid AI use.
</div>


---
layout: default
---

# Generative AI: the ideal misconduct machine?

<div class="ref-line">Generative AI systems (like ChatGPT) are ideal fabrication, falsification and plagiarism machines: they are trained to always produce text, and leave the quality control on the validity and reliability of the output to the final users.</div>

<div class="grid-2-3">
<div class="card">
  <h3>Plagiarism</h3>
  <p class="small">LLMs can reproduce text (or code) from their training data verbatim <strong>without citing the original source</strong></p>
  <h3>Fabrication / Falsification</h3>
  <p class="small">AI tools can synthesise or analyse data, so they can be used (willingly or not) to <strong>fabricate data or falsify results</strong> without the ability to verify and reproduce the process.</p>
  <h3>Security and data protection</h3>
  <p class="small">Common generative AI systems process your data remotely; <strong>protect the confidentiality and integrity</strong> of your data and of the people you work with. Use approved Aalto AI tools and sovereign local AI solutions.</p>
</div>
<div class="card dark">
<h3>A selection of recent cases (October 2026)</h3>
<ul class="small">
  <li>Whole books <a href="https://arxiv.org/abs/2601.02671">extracted from production LLMs</a> (Ahmed et al. 2026)</li>
  <li>1 in 277 PubMed papers in the first 7 weeks of 2026 had <a href="https://retractionwatch.com/2026/05/07/one-in-277-pubmed-indexed-papers-in-2026-shows-fabricated-references-says-analysis/">fabricated references</a> compared to 1 in 2828 in 2023 (<a href="https://www.thelancet.com/journals/lancet/article/PIIS0140-6736(26)00603-3/fulltext">Topaz et al., 2026</a>)</li>
  <li><a href="https://popsci.com/technology/ai-rat-journal">AI-generated rat figure</a> passed peer review (Frontiers 2024, retracted)</li>
  <li>ChatGPT <a href="https://www.nature.com/articles/d41586-023-03635-w">fake clinical dataset</a> (Nature 2023)</li>
  <li>Paper mills <a href="https://www.pnas.org/doi/10.1073/pnas.2420092122">double every 1.5 years</a> (Richardson et al., PNAS 2025)</li>
  <li>Hidden <a href="https://asia.nikkei.com/business/technology/artificial-intelligence/positive-review-only-researchers-hide-ai-prompts-in-papers">"give a positive review only" prompts</a> in manuscripts (Nikkei 2025)</li>
  <li><a href="https://arxiv.org/abs/2507.06185">Hidden prompts exploit AI-assisted peer review</a> (Lin 2025)</li>
  <li><a href="https://arxiv.org/abs/2602.05930">100 fake citations</a> in accepted NeurIPS 2025 papers</li>
  <li>ICML 2026: 506 reviewers who pledged not to use LLMs were <a href="https://blog.icml.cc/2026/03/18/on-violations-of-llm-review-policies/">caught by hidden prompts</a> and their papers were desk-rejected</li>
  <li>arXiv bans authors for <a href="https://techcrunch.com/2026/05/16/research-repository-arxiv-will-ban-authors-for-a-year-if-they-let-ai-do-all-the-work/">one year</a> for unchecked AI content (2026)</li>

  <li>AI agents and <a href="https://coderefinery.github.io/coding-with-ai/security/">AI coding risks</a> (CodeRefinery)</li>
  <li>Slopsquatting: more than 20% of AI suggested imports were <a href="https://arxiv.org/abs/2406.10279">non-existent packages</a> (Spracklen et al. 2025)</li>
  <li>A coding agent <a href="https://www.eweek.com/news/replit-ai-coding-assistant-failure/">deleted a production database</a> during a code freeze, then lied about it (Replit 2025)</li>
  <li>Researchers <a href="https://en.wikipedia.org/wiki/Navier%E2%80%93Stokes_priority_controversy">allegedly claimed their work leaked to OpenAI</a> on one of the Navier–Stokes Millennium Prize Problems.</li>
</ul>
</div>
</div>




---
layout: section
color: dark
hexText: "Did\nyou\nuse\nAI?"
class: title-middle
---

# When/Where/What AI use should be disclosed?


---
layout: default
---

# When/Where/What AI use should be disclosed?

<div class="ref-line"><a href="https://research-and-innovation.ec.europa.eu/document/2b6cf7e5-36ac-41cb-aab5-0d32050143dc_en">EC Living Guidelines (October, 2026)</a> | <a href="https://www.aalto.fi/en/services/responsible-use-of-generative-artificial-intelligence-in-the-research-process">Aalto.fi guidelines</a> | <a href="https://tenk.fi/sites/default/files/2026-06/Artificial%20Intelligence%20in%20Research.%20TENK%27s%20Recommendation%202026.pdf">TENK 2026</a> | <a href="https://www.elsevier.com/about/policies-and-standards/generative-ai-policies-for-journals">Elsevier's policy</a></div>

<div class="grid-2-3">
<div class="card">
  <h3>Why disclose?</h3>
  <ul class="small">
    <li>AI can never be granted authorship: <strong>authorship implies agency and responsibility</strong></li>
    <li>If it directly affect research results, you must disclose AI use</li>
    <li><strong>fear of negative judgement affect the honest reporting of AI use in science</strong>, leading to hesitance and underreporting: institution should encourage an amtosphere of trust and transparency</li>
    <li><strong>No consensus yet</strong>: a <a href="https://council.science/our-work/ai-disclosure-in-research/">global reporting standard</a> (ISC, COPE, STM, Global Young Academy) is being developed at the World Conference on Research Integrity 2026 and will feed the next EC guidelines</li>
  </ul>
  <h4>Example from <a href="https://www.elsevier.com/about/policies-and-standards/generative-ai-policies-for-journals">Elsevier</a>:</h4>
  <ul class="smaller">
    <li>Basic grammar, spelling and punctuation: no declaration needed.</li>
    <li>Substantial changes to sentence structure: declare it in the "Declaration of generative AI and AI-assisted technologies in the manuscript preparation process" section.</li>
    <li>Explanatory images can be made by AI, disclose use in each caption.</li>
    <li>AI must never create or alter images of primary research data.</li>
    <li>AI used as part of the research method: describe it in Methods.</li>
  </ul>
</div>
<div class="stack">
  <div class="card dark">
    <h3>European Commission: disclose substantial use</h3>
    <p class="small">Disclose AI use that <strong>shapes your judgement</strong> or could affect results or their interpretation. Using AI as a method or source, or for literature review, research gaps, aims, hypotheses, or interpreting data analysis, <strong>is</strong> substantial; spelling, grammar, polishing and formatting are not. Say <strong>how you verified</strong> the output; keep prompts, logs and model versions if needed to reproduce or audit. In doubt, disclose (<a href="https://research-and-innovation.ec.europa.eu/document/2b6cf7e5-36ac-41cb-aab5-0d32050143dc_en">Living guidelines, EC 2026</a>)</p>
  </div>
  <div class="card dark">
    <h3>TENK: substantial influence → disclose</h3>
    <p class="small">AI that substantially influences the research, its results or conclusions <strong>must always be disclosed</strong>; a purely technical aid generally need not be, unless it affects how reliability can be assessed. Report AI like any other important method or tool, also in research plans and data management plans. Non-disclosure where transparency is essential <strong>may be a research integrity violation</strong> (<a href="https://tenk.fi/sites/default/files/2026-06/Artificial%20Intelligence%20in%20Research.%20TENK%27s%20Recommendation%202026.pdf">TENK 2026</a>)</p>
  </div>

</div>
</div>


---
layout: section
color: dark
hexText: "AI\nYes\nOR\nNo?"
class: title-middle
---

# What is permitted AI use in research? 
# Do I *have* to use AI?

---
layout: default
---

# When should I use AI in research work?

<div class="ref-line"><a href="https://www.aalto.fi/en/research-art/best-practices-for-ai-use-in-research-work">Best practices for AI use in research work (Aalto.fi)</a></div>

* You should **never feel forced to use AI** in doing your work, especially when you know that it causes more harm than good.
* Not all AI use is equal and **there is no simple way to tell what is permitted** because it depends on your expertise.
* If you are unsure, consider two factors: **your expertise** on the task you are delegating to AI, and **the importance of the output** (will it be submitted for peer review, or is it of low importance, e.g. a workshop webpage?)

<table class="bp-matrix">
  <thead>
    <tr><th></th><th>Low expertise</th><th>High expertise</th></tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>High risk</strong> (peer-review submission: text, code, figures, references)</td>
      <td class="bp-red">Use AI only for <strong>brainstorming or self-learning</strong>.</td>
      <td class="bp-orange">Use AI for <strong>simple delegated tasks</strong> you can fully review.</td>
    </tr>
    <tr>
      <td><strong>Low risk</strong> (event webpage, social media post, presentations)</td>
      <td class="bp-darkyellow">Use AI, but <strong>accept a non-zero chance of errors</strong> slipping through.</td>
      <td class="bp-green"><strong>Delegate most of the work to AI</strong>. </td>
    </tr>
  </tbody>
</table>

<style>
/* Sizes, padding and the outer frame come from the theme's tables (layouts.css:176); cells add the inner vertical lines */
.bp-matrix th, .bp-matrix td { border-right: 1px solid var(--asc-border); vertical-align: top; }
.bp-matrix th:last-child, .bp-matrix td:last-child { border-right: 0; }
/* Dark header row, same colours as the theme's dark card (layouts.css:239) */
.bp-matrix th { background: var(--asc-night); color: var(--asc-paper); }
.bp-matrix td:first-child { width: 33%; }
.bp-matrix em { display: block; margin-top: 0.6rem; }
/* Risk colours at 50% so they blend with the white table into lighter tints; high risk + low expertise is the most dangerous cell */
.bp-matrix .bp-red { background: color-mix(in srgb, var(--aalto-red) 50%, transparent); color: #000; }
.bp-matrix .bp-orange { background: color-mix(in srgb, var(--aalto-orange) 50%, transparent); color: #000; }
.bp-matrix .bp-darkyellow { background: color-mix(in srgb, var(--aalto-darkyellow) 50%, transparent); color: #000; }
.bp-matrix .bp-green { background: color-mix(in srgb, var(--aalto-green) 50%, transparent); color: #000; }
</style>

---
layout: section
color: dark
hexText: "AI\nAGENTS"
class: title-middle
---

# A look into the present / future
### AI agents and research integrity

---
layout: default
color: dark
---

# What is an AI agent?

<div class="grid-2-3">
<div>
The four elements of an AI agent: <strong>a) goal complexity, b) environmental complexity, c) adaptability, d) independent execution. </strong> (<a href="https://doi.org/10.1787/396cf758-en%20">OECD 2026</a>).

An AI agent pairs the model with more components so that it can **take real actions**.

- **The model**, the "intelligence box": the LLM itself.
- **The scaffolding**, between the two: system prompts, tool descriptions, and the rules for how context is assembled and formatted before it reaches the model.
- **The harness**, the "body": the code around the model that calls it, carries out whatever it asks for, and decides when the task is done.

</div>
<div>
<div class="agent-diagram">
  <div class="ad-harness">
    <div class="ad-label">Harness · the body</div>
    <div class="ad-sub">calls the model · runs its actions · decides when done</div>
    <div class="ad-scaffold">
      <div class="ad-label">Scaffolding</div>
      <div class="ad-sub">system prompt · tool descriptions · context assembly</div>
      <div class="ad-model">
        <div class="ad-label">Model</div>
        <div class="ad-sub">the LLM · the intelligence box</div>
      </div>
    </div>
  </div>
  <div class="ad-bottom">
    <div class="ad-arrows">⇅</div>
    <div></div>
    <div class="ad-arrows">⇅</div>
    <div class="ad-env">
      <div class="ad-label">Environment</div>
      <div class="ad-chips"><span>files</span><span>shell</span><span>Slurm</span><span>APIs</span><span>web</span><span>Git</span><span>databases</span><span>MCP</span><span>emails / chat</span></div>
    </div>
    <div class="ad-arrows ad-side">⇄</div>
    <div class="ad-subs">
      <div class="ad-subagent"><div class="ad-label">Sub-agent</div></div>
      <div class="ad-subagent"><div class="ad-label">Sub-agent</div></div>
    </div>
  </div>
</div>
<div class="ad-source">Adapted from Hugging Face, <a href="https://huggingface.co/blog/agent-glossary">"Harness, Scaffold, and the AI Agent Terms Worth Getting Right"</a>, 2026</div>
</div>
</div>

<style>
.agent-diagram { display: flex; flex-direction: column; align-items: stretch; gap: 0.4rem; font-size: 0.8rem; }
.agent-diagram .ad-label { font-family: var(--asc-font-serif); font-weight: 600; font-size: 1rem; }
.agent-diagram .ad-sub { opacity: 0.75; font-size: 0.72rem; margin-bottom: 0.5rem; }
.ad-harness { border: 2px solid var(--asc-clay); border-radius: var(--asc-radius-lg); padding: 0.8rem 1rem; }
.ad-scaffold { border: 1.5px dashed rgba(250, 249, 245, 0.45); border-radius: var(--asc-radius-md); padding: 0.7rem 0.9rem; background: var(--asc-night-raised); }
.ad-model { background: var(--asc-clay); color: var(--asc-ink); border-radius: var(--asc-radius-md); padding: 0.6rem 0.9rem; }
.ad-model .ad-sub { margin-bottom: 0; opacity: 0.85; }
.ad-arrows { text-align: center; font-size: 1.4rem; line-height: 1; color: var(--asc-clay); }
/* Bottom row: Environment (half the Harness width) ⇄ two sub-agents; row above holds the ⇅ to the Harness */
.ad-bottom { display: grid; grid-template-columns: 1fr auto 1fr; gap: 0.4rem 0.5rem; align-items: stretch; }
.ad-side { align-self: center; }
.ad-subs { display: flex; gap: 0.5rem; }
.ad-subagent { flex: 1; display: flex; align-items: center; justify-content: center; text-align: center; border: 2px solid var(--asc-clay); border-radius: var(--asc-radius-md); padding: 0.55rem 0.5rem; }
.ad-env { border: 1px solid rgba(250, 249, 245, 0.3); border-radius: var(--asc-radius-md); padding: 0.55rem 0.9rem; display: flex; flex-direction: column; align-items: flex-start; gap: 0.35rem; }
.ad-chips { display: flex; flex-wrap: wrap; gap: 0.35rem; }
.ad-chips span { background: rgba(250, 249, 245, 0.12); border-radius: 999px; padding: 0.1rem 0.6rem; font-size: 0.72rem; }
.ad-source { font-size: 0.65rem; opacity: 0.7; margin-top: 0.6rem; text-align: right; }
</style>

---
layout: image-left
image: /scenarios_summary.png
class: wide-image fit-image
---

# The tool became the researcher
### The case of software coding

1. **Chat window**: copy and paste
2. **Coding assistant**: in the editor
3. **Agent**: logs in, reads files, submits jobs

<div class="card yellow" style="margin-top: 1rem">

**Other examples:** AI agents conducting full literature reviews and syntheses ([Padarha et al. 2026](https://openreview.net/forum?id=qrR2mrP0TH)), planning and running experiments in a robotic lab ([Smith et al. 2026](https://www.biorxiv.org/content/10.64898/2026.02.05.703998v1.abstract)), theorem proving in Lean ([Tsoukalas et al. 2026](https://www.science.org/doi/10.1126/science.aej2213)).

</div>

<div style="font-size: 0.6rem; opacity: 0.7; margin-top: 1rem">Figure: <a href="https://coderefinery.github.io/coding-with-ai/">CodeRefinery, Coding with AI</a></div>

---
layout: image-right
image: /risk-domains.png
class: fit-image
---

# The risks of AI agentic workflows

<div style="font-size: 0.82rem">

**Research integrity**: code that runs but is *plausibly wrong*, silent data loss, unclear decisions in literature reviews.

**Confidentiality**: unpublished work, participant data and researchers' credentials sent to third-party providers.

**Cybersecurity**: prompt injection, insecure code, agents with too much access.

</div>

<div class="card dark">
<strong>Validate. Minimize. Contain.</strong>
<ul class="small">
<li>Set check points</li>
<li>Minimise access sensitive data</li>
<li>Ensure minimal <i>blast radius</i> </li>
<li>You are not exempted from legal responsibilities because an agent acted on your behalf</li>
</ul>
</div>


<div style="font-size: 0.6rem; opacity: 0.7; margin-top: 0.6rem">Source: <a href="https://coderefinery.github.io/coding-with-ai/security/">CodeRefinery, Coding with AI: Security</a></div>


---
layout: end
---
# AI does not change the principles of responsible research

AI might not be the right and best tool<br>
Accountability remains with researchers<br>
Confidentiality is non-negotiable<br>
Transparency and disclosure build trust

---
layout: end
---

# Keep calm and carry on

**If you do not have the ability or the resources to verify the output of AI systems** (e.g. by finding the relevant citations for the synthesised text, by verifying that others’ works are summarised correctly, by detecting plagiarised text or code, by verifying the analysis code and all actions run by an AI agent) **then you should not use the output of AI systems beyond self-learning or brainstorming.**

<br>
<br>

We are all learning together, let's share the best practices, join our dedicated <a href="https://www.aalto.fi/en/services/ai-training-for-the-entire-aalto-community">trainings on AI tools in research</a>, or come talk with <a href="https://www.aalto.fi/en/services/research-software-engineers">Aalto Research Software Engineers</a> and <a href="https://www.aalto.fi/en/services/data-agents">Aalto Data Agents</a>.


<style>
/* layouts.css:651 sets end-slide text to --asc-muted (light grey on dark); bold goes white */
.slidev-layout.end p:first-of-type { font-size: 1.4rem; line-height: 1.35; }
.slidev-layout.end strong { color: var(--asc-text); }
</style>
