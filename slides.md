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
title: Generative AI, Research Integrity and Ethics
author: Enrico Glerean
info: |
  Slides by Enrico Glerean (https://eglerean.github.io/), CC BY 4.0.
  Course: LC-L1000 Research Ethics for Doctoral Students
  Source: https://github.com/eglerean/genAI_researchintegrity
keywords: generative AI, research integrity, research ethics, Enrico Glerean, https://eglerean.github.io/
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

<style>
.ref-line { font-size: 0.7rem; opacity: 0.75; margin: -0.6rem 0 0.8rem; }
.col li { line-height: 1.4; margin: 0.2rem 0; }
.hidden-ai { margin-top: 0.9rem; font-size: 0.72rem; line-height: 1.35; opacity: 0.8; }
</style>

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

<p class="hidden-ai">Invisible AI: in word processors, search engines, translation, and transcription tools.</p>

---
layout: default
---

# The Research Process aided by AI tools
### Examples of AI tools used in different part of the research project

<div class="rdm-grid">
  <div class="stage" style="--stage: var(--aalto-orange)">Plan</div>
  <div class="stage" style="--stage: var(--aalto-darkyellow)">Collect</div>
  <div class="stage" style="--stage: var(--aalto-green)">Process</div>
  <div class="stage" style="--stage: var(--aalto-aquagreen)">Analyse</div>
  <div class="stage" style="--stage: var(--aalto-blue)">Preserve</div>
  <div class="stage" style="--stage: var(--aalto-violet)">Share</div>
  <div class="stage" style="--stage: var(--aalto-red)">Reuse</div>

  <div class="cell">
  • Grant writing<br>
  • Research planning<br>
  • Study design<br>
  • Browsing and summarizing the literature
  </div>
  <div class="cell">
  • Interfaces for data collection<br>
  • Code and automation help
  </div>
  <div class="cell">
  • Brainstorming on approaches for data preprocessing<br>
  • Code and automation<br>
  • Data minimization (pseudo- and anonymization)<br>
  • Data annotation (e.g. deductive coding)
  </div>
  <div class="cell">
  • Annotations<br>
  • Methodological considerations<br>
  • Data analysis (Code and automation)
  </div>
  <div class="cell">
  • Metadata preparation<br>
  • Summarising<br>
  • Organise and store (meta)data
  </div>
  <div class="cell">
  • Write and editing<br>
  • Improve research outputs (tables, figures)<br>
  • Peer review simulation<br>
  • Summarizing for public<br>
  • Media reach out
  </div>
  <div class="cell">
  • Facilitate discovery and FAIR-ness<br>
  • Explore open datasets<br>
  • Identify research gaps
  </div>
</div>



<div class="card dark ow-bottom">

There are multiple uses of AI across the <a href="https://rdmkit.elixir-europe.org/">research lifecycle</a> and depending on the tool and the usage each stage can carry risks of misconduct: Fabrication, Falsification, Plagiarism.
</div>

<style>
.rdm-grid { display: grid; grid-template-columns: repeat(7, minmax(0, 1fr)); gap: 0.4rem; margin-top: 1rem; }
.rdm-grid .stage { white-space: nowrap; text-align: center; font-weight: 700; font-size: 0.85rem; padding: 0.4rem 0.2rem; border-radius: var(--asc-radius-lg); background: var(--stage); color: #fff; }
.rdm-grid .cell { padding: 0.5rem; font-size: 0.7rem; line-height: 1.3; background: var(--asc-surface); border: 1px solid var(--asc-border); border-radius: var(--asc-radius-lg); }
.ow-bottom { margin-top: 1rem; padding: 0.6rem 1.3rem; }
.ow-bottom p { font-family: var(--asc-font-serif); font-size: 1.02rem; line-height: 1.3; margin: 0; }
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
  <div class="p-card">
    AI Governance in Practice <span class="p-src">(<a href="https://www.turing.ac.uk/research/research-projects/ai-ethics-and-governance-practice">The Alan Turing Institute</a>)</span><br>
    <a href="https://eur-lex.europa.eu/eli/reg/2024/1689/oj/eng">Artificial Intelligence Act</a>
  </div>
  <div class="p-card">
    SSAFE-D: Sustainability, Safety, Accountability, Fairness, Explainability, Data Stewardship <span class="p-src">(<a href="https://www.turing.ac.uk/research/research-projects/ai-ethics-and-governance-practice">The Alan Turing Institute</a>)</span>
  </div>
  <div class="p-card">
    Beneficence, Non-maleficence, Autonomy, Justice, Explicability <span class="p-src"><a href="https://academic.oup.com/book/46748">(Floridi 2023)</a></span>
  </div>
</div>
</div>

<style>
/* Pyramid on the left; the card column uses the same 420-unit height split as the slices (0-170, 170-290, 290-420) so each card sits beside its slice */
.pyramid { display: grid; grid-template-columns: auto 1fr; gap: 1.5rem; height: 360px; margin-top: 0.5rem; }
.pyramid svg { height: 100%; width: auto; }
.pyramid .p-cards { display: grid; grid-template-rows: 170fr 120fr 130fr; height: 100%; }
.pyramid .p-card { align-self: center; padding: 0.5rem 0.75rem; font-size: 1.0rem; line-height: 1.35; background: var(--asc-surface); border: 1px solid var(--asc-border); border-radius: var(--asc-radius-lg); }
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
<br>
<div class="five-principles">
  <img src="/images/unified-five-principles.png" alt="Diagram: traditional bioethics principles lead to Beneficence, Non-maleficence, Autonomy and Justice; a new enabling principle for AI leads to Explicability">
</div>

<div class="ref-bottom">Reference: Traditional bioethics principles by <a href="https://archive.org/details/principlesofbiom0000beau_k8c1">Beauchamp &amp; Childress</a> (1979-2026), extended by Floridi, L. (2023) in “<a href="https://academic.oup.com/book/46748">The ethics of artificial intelligence: Principles, challenges, and opportunities.</a>”. Original image from <a href="https://www.edpb.europa.eu/documents/support-pool-of-experts/fundamentals-of-secure-ai-systems-with-personal-data_en">Glerean (2025) "Fundamentals of secure AI systems with personal data" European Data Protection Board</a></div>

<style>
.five-principles { display: flex; justify-content: center; margin-top: 2rem; }
.five-principles img { width: 100%; max-width: 820px; height: auto; }
/* !important: the theme sets position: relative on all slide content (layouts.css:352); bottom clears the 2.75rem footer */
.ref-bottom { position: absolute !important; left: 3.5rem; right: 3.5rem; bottom: 3rem; font-size: 0.7rem; opacity: 0.75; }
</style>

---
layout: default
---

# Responsible AI, the SSAFE-D principles

<div class="ref-line"><strong>SSAFE-D</strong>: Sustainability, Safety, Accountability, Fairness, Explainability, Data Stewardship (<a href="https://www.turing.ac.uk/research/research-projects/ai-ethics-and-governance-practice">The Alan Turing Institute</a>)</div>

<div class="ssafed">
  <div class="sd-card" style="--c: var(--aalto-green)"><div class="sd-tri">S</div><div><h3>Sustainability</h3><p>Achieving this goal requires assuring AI projects being developed with continuous sensitivity to real-world impacts.</p></div></div>
  <div class="sd-card" style="--c: var(--aalto-red)"><div class="sd-tri">S</div><div><h3>Safety</h3><p>Achieving this goal requires an AI system to be technically accurate, reliable, secure, and robust.</p></div></div>
  <div class="sd-card" style="--c: var(--aalto-blue)"><div class="sd-tri">A</div><div><h3>Accountability</h3><p>Achieving this goal requires assuring the project’s end-to-end answerability and auditability.</p></div></div>
  <div class="sd-card" style="--c: var(--aalto-orange)"><div class="sd-tri">F</div><div><h3>Fairness</h3><p>Achieving this goal requires assuring a minimum threshold of discriminatory non-harm and bias mitigation.</p></div></div>
  <div class="sd-card" style="--c: var(--aalto-violet)"><div class="sd-tri">E</div><div><h3>Explainability</h3><p>Achieving this goal requires the ability to explain and justify AI project processes and AI-supported outcomes.</p></div></div>
  <div class="sd-card" style="--c: var(--aalto-aquagreen)"><div class="sd-tri">D</div><div><h3>Data Stewardship</h3><p>Achieving this goal requires data quality, integrity, protection, and privacy to be assured.</p></div></div>
</div>

<div class="card dark sd-bottom">

The SSAFE-D principles come from <a href="https://www.turing.ac.uk/research/research-projects/ai-ethics-and-governance-practice">AI Ethics and Governance in Practice</a>, a programme of The Alan Turing Institute with workbooks for applying these principles across the whole AI project lifecycle.
</div>

<style>
.sd-bottom { margin-top: 0.75rem; padding: 0.6rem 1.3rem; }
.sd-bottom p { font-family: var(--asc-font-serif); font-size: 1.02rem; line-height: 1.3; margin: 0; }
.ref-line { font-size: 0.7rem; opacity: 0.75; margin: -0.6rem 0 0.8rem; }
.ssafed { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 0.75rem; }
.sd-card { display: flex; gap: 0.75rem; align-items: flex-start; padding: 0.75rem; background: var(--asc-surface); border: 1px solid var(--asc-border); border-radius: var(--asc-radius-lg); }
.sd-tri { flex: none; width: 3rem; height: 2.6rem; clip-path: polygon(50% 0, 100% 100%, 0 100%); background: var(--c); color: #000; font-weight: 700; font-size: 1.1rem; display: flex; align-items: flex-end; justify-content: center; padding-bottom: 0.15rem; }
.sd-card h3 { margin: 0 0 0.25rem; font-size: 0.95rem; }
.sd-card p { margin: 0; font-size: 0.75rem; line-height: 1.35; }
</style>

---
layout: default
---

# SSAFE-D applied: how ethical are current tools?

Responsible AI principles are currently not followed by the majority of developers of generative AI systems/models (OpenAI, Anthropic, Meta, Google, xAI…)

<div class="sd-eval">
  <div>❌ <strong>Sustainability</strong>: huge impact on the planet; data centres use about 1.5% of global electricity, set to double by 2030 (<a href="https://www.iea.org/reports/energy-and-ai/energy-demand-from-ai">IEA</a>) (<a href="https://arxiv.org/abs/2510.09022">Morand et al. 2026</a>)</div>
  <div>❌ <strong>Safety</strong>: induced <a href="https://www.reuters.com/investigates/special-report/meta-ai-chatbot-death/">psychosis</a>, <a href="https://www.theguardian.com/technology/2025/aug/27/chatgpt-scrutiny-family-teen-killed-himself-sue-open-ai">suicide</a>, <a href="https://www.cnn.com/2026/01/07/business/character-ai-google-settle-teen-suicide-lawsuit">teen-harm lawsuits settled</a> (2026), <a href="https://abc17news.com/money/cnn-business-consumer/2026/06/01/florida-sues-openai-alleging-its-unsafe-for-children/">Florida sues OpenAI</a> (2026), <a href="https://www.vice.com/en/article/openai-used-kenyan-workers-making-dollar2-an-hour-to-filter-traumatic-content-from-chatgpt/">exploitation</a> of global-south annotators (<a href="https://www.science.org/doi/10.1126/science.aec8352">Cheng et al., Science 2026</a>; <a href="https://dl.acm.org/doi/full/10.1145/3715275.3732039">Moore et al. 2025</a>)</div>
  <div>❌ <strong>Accountability</strong>: few consequences for harming individuals; Grok's sexualised deepfakes led to <a href="https://www.cnbc.com/2026/01/05/india-eu-investigate-musks-x-after-grok-created-deepfake-child-porn.html">investigations</a> (2026), but Canada's regulator <a href="https://www.aljazeera.com/economy/2026/6/11/musks-grok-accused-of-violating-canadian-privacy-laws-on-deepfakes">cannot fine xAI</a> (<a href="https://arxiv.org/abs/2512.01166">Stelling et al. 2026</a>; <a href="https://internationalaisafetyreport.org/publication/international-ai-safety-report-2026">Int. AI Safety Report 2026</a>)</div>
  <div>❌ <strong>Fairness</strong>: biases against <a href="https://www.theguardian.com/technology/2024/mar/16/ai-racism-chatgpt-gemini-bias">Black people</a>, women, minorities (<a href="https://www.nature.com/articles/s41586-024-07856-5">Hofmann et al., Nature 2024</a>; <a href="https://www.nature.com/articles/s41586-025-09581-z">Guilbeault et al., Nature 2025</a>)</div>
  <div>❌ <strong>Explainability</strong>: proprietary models, no clear explanation of how they work; company <a href="https://news.stanford.edu/stories/2025/12/foundation-model-transparency-index-ai-companies-information">transparency fell</a> from 58 to 41 out of 100 in 2025 (<a href="https://arxiv.org/abs/2505.05410">Chen et al. 2025</a>)</div>
  <div>❌ <strong>Data Stewardship</strong>: training data kept secret, illegal use of copyrighted material (<a href="https://www.jurist.org/news/2026/07/judge-approves-record-1-5-billion-settlement-involving-anthropic/">$1.5B settlement for pirated books</a>, 2026), Stable Diffusion even reproduced <a href="https://www.theverge.com/2023/2/6/23587393/ai-art-copyright-lawsuit-getty-images-stable-diffusion">Getty Images watermarks</a> (UK, 2023-2025), unauthorised <a href="https://europeanlawblog.eu/2klfhf06/">processing of personal data</a>, near-verbatim extraction of books from LLMs (<a href="https://arxiv.org/abs/2601.02671">Ahmed et al. 2026</a>)</div>
</div>

<div class="ref-bottom">Check the references for more: <a href="https://www.sciencedirect.com/science/article/pii/S0268401223000816">Stahl &amp; Eke (2024) “The Ethics of ChatGPT”</a> · <a href="https://thecon.ai/">Bender &amp; Hanna (2025) “The AI Con”</a></div>

<style>
.sd-eval { display: grid; gap: 0.4rem; margin-top: 0.75rem; font-size: 0.8rem; line-height: 1.3; }
/* !important: the theme sets position: relative on all slide content (layouts.css:352); bottom clears the 2.75rem footer */
.ref-bottom { position: absolute !important; left: 3.5rem; right: 3.5rem; bottom: 3rem; font-size: 0.7rem; opacity: 0.75; }
</style>

---
layout: default
---

# AI regulations: EU AI Act

<div class="ref-line"><a href="https://eur-lex.europa.eu/eli/reg/2024/1689/oj/eng">Regulation (EU) 2024/1689</a>: a risk-based approach. Most AI tools are minimal risk with no new obligations; general-purpose AI models (e.g. GPT, Gemini, Claude) have their own rules.</div>

<div class="aia-grid">
  <div class="aia-card">
    <h3>Prohibited</h3>
    <p class="aia-when">Unacceptable risk · since 2 Feb 2025</p>
    <ul>
      <li>Social scoring</li>
      <li>Manipulation, exploiting vulnerabilities</li>
      <li>Untargeted scraping of face images</li>
      <li>Emotion recognition at work and in education</li>
      <li>Predicting crime from profiling alone</li>
    </ul>
  </div>
  <div class="aia-card">
    <h3>High risk</h3>
    <p class="aia-when">Strict requirements · from 2 Dec 2027</p>
    <ul>
      <li>Education: admission, grading, proctoring</li>
      <li>Employment: hiring, evaluating workers</li>
      <li>Access to credit and essential services</li>
      <li>Law enforcement, migration, justice</li>
      <li>Risk management, data quality, documentation, human oversight</li>
    </ul>
  </div>
  <div class="aia-card">
    <h3>Transparency</h3>
    <p class="aia-when">Limited risk · since 2 Aug 2026</p>
    <ul>
      <li>Tell people they are talking to an AI</li>
      <li>Mark AI-generated content as machine-readable</li>
      <li>Label deepfakes</li>
      <li>Disclose emotion recognition and biometric categorisation</li>
    </ul>
  </div>
</div>

<div class="card dark aia-bottom">

**Scope:** the AI Act is a product regulation: it applies when AI is placed on the EU market or put into service. AI developed and used only for scientific research is excluded, but if your research will become a product or a service, the Act will apply to it, so plan for it early.<br>
<br>

**Timeline:** in force 1 Aug 2024 · prohibitions and AI literacy 2 Feb 2025 · general-purpose AI models 2 Aug 2025 · transparency 2 Aug 2026 · high risk 2 Dec 2027 (2 Aug 2028 for regulated products), delayed by the <a href="https://artificialintelligenceact.eu/ai-act-explorer/digital-omnibus/">2026 Digital Omnibus</a>
</div>

<style>
.ref-line { font-size: 0.7rem; opacity: 0.75; margin: -0.6rem 0 0.8rem; }
.aia-grid { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 0.75rem; }
.aia-card { padding: 0.6rem 0.8rem; background: var(--asc-surface); border: 1px solid var(--asc-border); border-radius: var(--asc-radius-lg); }
.aia-card h3 { margin: 0; font-size: 1rem; }
.aia-card p { margin: 0; font-size: 0.75rem; line-height: 1.35; }
.aia-card ul { margin: 0; padding-left: 1.1rem; }
.aia-card li { margin: 0; font-size: 0.75rem; line-height: 1.35; }
.aia-card .aia-when { margin: 0.1rem 0 0.4rem; color: var(--asc-muted); }
.aia-bottom { margin-top: 0.75rem; padding: 0.6rem 1.3rem; }
.aia-bottom p { font-size: 0.8rem; line-height: 1.35; margin: 0; }
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

# Responsible AI principles and research integrity

<div class="ref-line"><a href="https://allea.org/code-of-conduct/">ALLEA Code of Conduct</a> | <a href="https://research-and-innovation.ec.europa.eu/document/2b6cf7e5-36ac-41cb-aab5-0d32050143dc_en">EC Living Guidelines (October, 2026)</a> | <a href="https://www.aalto.fi/en/services/responsible-use-of-generative-artificial-intelligence-in-the-research-process">Aalto.fi guidelines</a> | <a href="https://tenk.fi/sites/default/files/2026-06/Artificial%20Intelligence%20in%20Research.%20TENK%27s%20Recommendation%202026.pdf">TENK 2026</a></div>

<div class="allea">
  <div class="al-principle"><h3>Reliability</h3>Quality of research/education, reflected in the design, methodology, analysis, and use of resources.</div>
  <ul class="al-practice">
    <li><strong>Verify</strong> and <strong>reproduce</strong> AI-generated information; watch for bias and inaccuracy</li>
    <li>Check all <strong>references</strong>, <strong>citations</strong> and <strong>summaries</strong>: AI fabricates citations and misstates real ones</li>
    <li>Output is non-deterministic: keep <strong>prompts, logs and model versions</strong> when needed to reproduce or audit</li>
  </ul>

  <div class="al-principle"><h3>Honesty</h3>Doing your work in a transparent, fair, full, and unbiased way.</div>
  <ul class="al-practice">
    <li><strong>Disclose</strong> AI use that shapes your judgement or could affect results; in doubt, disclose</li>
    <li>Say <strong>how you verified</strong> the output (e.g. hallucination checks, bias mitigation)</li>
    <li>Follow your journal's, funder's or discipline's rules on where and how</li>
  </ul>

  <div class="al-principle"><h3>Respect</h3>Towards colleagues, research participants, research subjects, society, cultural heritage, and the environment.</div>
  <ul class="al-practice">
    <li>Protect privacy, confidentiality, IP and <strong>research security</strong>: use <strong>Aalto AI Assistant</strong> for confidential data</li>
    <li><strong>Don't upload unpublished work</strong>, yours or colleagues', to external tools</li>
    <li><strong>Cite and credit sources</strong> that AI output may reproduce; choose the <strong>lowest-impact tool</strong> for the task</li>
  </ul>

  <div class="al-principle"><h3>Accountability</h3>From idea to publication, and all the steps of the study / teaching / research process.</div>
  <ul class="al-practice">
    <li>You remain <strong>fully responsible</strong> for AI-assisted content, also when <strong>agents</strong> act for you</li>
    <li>AI systems are <strong>neither authors, co-authors nor owners</strong>: authorship lies with human researchers</li>
    <li>Peer review and grant evaluation: <strong>never delegate the judgement</strong>; funder and journal rules come first</li>
  </ul>
</div>

<style>
.ref-line { font-size: 0.7rem; opacity: 0.75; margin: -0.6rem 0 0.8rem; }
.allea { display: grid; grid-template-columns: minmax(0, 2fr) minmax(0, 3fr); gap: 0.5rem 0.75rem; }
.al-principle, .al-practice { padding: 0.45rem 0.8rem; font-size: 0.75rem; line-height: 1.35; background: var(--asc-surface); border: 1px solid var(--asc-border); border-radius: var(--asc-radius-lg); }
/* Same colours as the theme's dark card (layouts.css:239) */
.al-practice { margin: 0; padding-left: 1.8rem; background: var(--asc-night); border-color: var(--asc-night); color: var(--asc-paper); }
.al-practice li { margin: 0; font-size: 0.75rem; line-height: 1.35; }
.al-principle h3 { margin: 0 0 0.15rem; font-size: 0.95rem; }
</style>

---
layout: default
---

# Generative AI: the ideal misconduct machine?

<p class="mm-intro">Generative AI systems (like ChatGPT) are ideal fabrication, falsification and plagiarism machines: they are trained to always produce text, and leave the quality control on the validity and reliability of the output to the final users.</p>

<div class="mm-cols">
<div class="mm-box">
  <h3>Plagiarism</h3>
  <p>LLMs can reproduce text from their training data verbatim without citing the original source</p>
  <h3>Fabrication / Falsification</h3>
  <p>GenAI can synthesise or analyse data, so it can be used (willingly or not) to fabricate data or falsify results without the ability to verify and reproduce the process (how many r's in strawberry?)</p>
  <h3>Peer review under pressure</h3>
  <p>AI makes papers and reviews cheap to produce; venues are starting to sanction misuse</p>
  <h3>Security and data protection</h3>
  <p>Common GenAI systems process your data remotely; protect the confidentiality and integrity of your data and of the people you work with. Use approved Aalto AI tools.</p>
</div>
<div class="mm-box mm-refs">
<h3>Recent cases and evidence</h3>
<ul>
  <li>Whole books <a href="https://arxiv.org/abs/2601.02671">extracted from production LLMs</a> (Ahmed et al. 2026)</li>
  <li>1 in 277 PubMed papers in 2026 has <a href="https://retractionwatch.com/2026/05/07/one-in-277-pubmed-indexed-papers-in-2026-shows-fabricated-references-says-analysis/">fabricated references</a> (Topaz et al., Lancet 2026)</li>
  <li><a href="https://popsci.com/technology/ai-rat-journal">AI-generated rat figure</a> passed peer review (Frontiers 2024, retracted)</li>
  <li>ChatGPT <a href="https://www.nature.com/articles/d41586-023-03635-w">fake clinical dataset</a> (Nature 2023)</li>
  <li>Paper mills <a href="https://www.pnas.org/doi/10.1073/pnas.2420092122">double every 1.5 years</a> (Richardson et al., PNAS 2025)</li>
  <li>Hidden <a href="https://asia.nikkei.com/business/technology/artificial-intelligence/positive-review-only-researchers-hide-ai-prompts-in-papers">"give a positive review only" prompts</a> in manuscripts (Nikkei 2025)</li>
  <li><a href="https://arxiv.org/abs/2507.06185">Hidden prompts exploit AI-assisted peer review</a> (Lin 2025)</li>
  <li><a href="https://arxiv.org/abs/2602.05930">100 fake citations</a> in accepted NeurIPS 2025 papers</li>
  <li>ICML 2026: 506 reviewers who pledged not to use LLMs were <a href="https://blog.icml.cc/2026/03/18/on-violations-of-llm-review-policies/">caught by hidden watermarks</a>; 497 of their papers desk-rejected</li>
  <li>arXiv bans authors for <a href="https://techcrunch.com/2026/05/16/research-repository-arxiv-will-ban-authors-for-a-year-if-they-let-ai-do-all-the-work/">one year</a> for unchecked AI content (2026)</li>

  <li>AI agents and <a href="https://coderefinery.github.io/coding-with-ai/security/">AI coding risks</a> (CodeRefinery)</li>
  <li>Slopsquatting: up to ~20% of AI code imports <a href="https://arxiv.org/abs/2406.10279">non-existent packages</a> (Spracklen et al. 2025)</li>
  <li>A coding agent <a href="https://www.eweek.com/news/replit-ai-coding-assistant-failure/">deleted a production database</a> during a code freeze, then lied about it (Replit 2025)</li>
</ul>
</div>
</div>


<style>
.mm-intro { font-size: 0.8rem; line-height: 1.3; margin: 0 0 0.5rem; }
.mm-cols { display: grid; grid-template-columns: minmax(0, 2fr) minmax(0, 3fr); gap: 0.75rem; }
.mm-box { padding: 0.5rem 0.8rem; background: var(--asc-surface); border: 1px solid var(--asc-border); border-radius: var(--asc-radius-lg); }
.mm-box p { margin: 0 0 0.45rem; font-size: 0.72rem; line-height: 1.35; }
.mm-box p:last-child { margin-bottom: 0; }
.mm-box h3 { margin: 0 0 0.1rem; font-size: 0.9rem; }
/* Same colours as the theme's dark card (layouts.css:239); light Aalto blue keeps links readable on black */
.mm-refs { background: var(--asc-night); border-color: var(--asc-night); color: var(--asc-paper); }
.mm-refs h3 { color: inherit; }
.mm-refs ul { margin: 0; padding-left: 1.1rem; }
.mm-refs li { margin: 0 0 0.2rem; font-size: 0.64rem; line-height: 1.3; }
.mm-refs a { color: var(--aalto-blue); }
</style>


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

<div class="dc-cols">
<div class="dc-box dc-why">
  <h3>Why disclose?</h3>
  <ul>
    <li>AI can never be granted authorship: <strong>accountability is liability</strong></li>
    <li>LLMs are probabilistic tools: the chance they generate something fabricated is never zero</li>
    <li><strong>"If you cannot explain it, you cannot stand behind it"</strong> → disclose</li>
    <li><strong>No consensus yet</strong>: a <a href="https://council.science/our-work/ai-disclosure-in-research/">global reporting standard</a> (ISC, COPE, STM, Global Young Academy) is being developed at the World Conference on Research Integrity 2026 and will feed the next EC guidelines</li>
  </ul>
  <h3 class="dc-sub"><a href="https://www.elsevier.com/about/policies-and-standards/generative-ai-policies-for-journals">Example from Elsevier:</a></h3>
  <ul>
    <li>Protect your data, the data of your subjects, IPR/copyright</li>
    <li>Grammar, spelling, punctuation check → no need to declare</li>
    <li>Any other use → declare</li>
    <li>No AI images unless it's for the research design/methods visualisation</li>
  </ul>
</div>
<div class="dc-right">
  <div class="dc-box">
    <h3>European Commission: disclose substantial use</h3>
    <p>Disclose AI use that <strong>shapes your judgement</strong> or could affect results or their interpretation. Using AI as a method or source, or for literature review, research gaps, aims, hypotheses or data analysis, <strong>is</strong> substantial; spelling, grammar, polishing and formatting are not. Say <strong>how you verified</strong> the output; keep prompts, logs and model versions if needed to reproduce or audit. In doubt, disclose (<a href="https://research-and-innovation.ec.europa.eu/document/2b6cf7e5-36ac-41cb-aab5-0d32050143dc_en">Living guidelines, EC 2026</a>)</p>
  </div>
  <div class="dc-box">
    <h3>TENK (Finland): substantial influence → always disclose</h3>
    <p>AI that substantially influences the research, its results or conclusions <strong>must always be disclosed</strong>; a purely technical aid generally need not be, unless it affects how reliability can be assessed. Report AI like any other important method or tool, also in research plans and data management plans. Non-disclosure where transparency is essential <strong>may be a research integrity violation</strong> (<a href="https://tenk.fi/sites/default/files/2026-06/Artificial%20Intelligence%20in%20Research.%20TENK%27s%20Recommendation%202026.pdf">TENK 2026</a>)</p>
  </div>
  <div class="dc-box">
    <h3>STM: a classification of AI use in manuscripts</h3>
    <p><strong>No disclosure</strong>: language editing and formatting · <strong>Disclose</strong>: drafting content, translation, formatting data, illustrative images, data visualisations, code, gathering references · <strong>Prohibited</strong>: presenting AI content as original research data (<a href="https://stm-assoc.org/document/recommendations-for-a-classification-of-ai-use-in-academic-manuscript-preparation/">STM 2025</a>)</p>
  </div>
  <div class="dc-box">
    <h3>Mandatory disclosure when AI is used to…</h3>
    <p>(a) make decisions that directly affect research results · (b) generate content, data or images · (c) analyse content, data or images (<a href="https://www.tandfonline.com/doi/full/10.1080/08989621.2025.2481949">Resnik &amp; Hosseini 2025</a>)</p>
  </div>
</div>
</div>

<style>
.dc-cols { display: grid; grid-template-columns: minmax(0, 2fr) minmax(0, 3fr); gap: 0.75rem; }
.dc-right { display: grid; gap: 0.45rem; }
.dc-box { padding: 0.4rem 0.8rem; background: var(--asc-surface); border: 1px solid var(--asc-border); border-radius: var(--asc-radius-lg); }
.dc-box h3 { margin: 0 0 0.2rem; font-size: 0.9rem; }
.dc-box p { margin: 0; font-size: 0.72rem; line-height: 1.35; }
.dc-why ul { margin: 0; padding-left: 1.1rem; }
.dc-why li { margin: 0 0 0.35rem; font-size: 0.78rem; line-height: 1.35; }
.dc-why .dc-sub { margin-top: 0.6rem; }
/* Right-column boxes: same colours as the theme's dark card (layouts.css:239); light Aalto blue keeps links readable on black */
.dc-right .dc-box { background: var(--asc-night); border-color: var(--asc-night); color: var(--asc-paper); }
.dc-right .dc-box h3 { color: inherit; }
.dc-right .dc-box a { color: var(--aalto-blue); }
</style>


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
      <td class="bp-red">Use AI only to <strong>brainstorm</strong>: ask it what sources to read, get keyword suggestions, then go read the real sources.<br>
      <em>Example: find relevant keywords or ask which statistical methods might fit your data, then go read about them yourself.</em></td>
      <td class="bp-orange">Use AI for <strong>simple delegated tasks</strong> you can fully review. Check everything as carefully as if you had retyped it yourself. This is where overconfidence is most dangerous.<br>
      <em>Examples: generating short code snippets function-by-function. Text revision: ask AI to mark suggested text changes in bold, so you can decide which ones to apply manually to your final text.</em></td>
    </tr>
    <tr>
      <td><strong>Low risk</strong> (event webpage, social media post, presentations)</td>
      <td class="bp-darkyellow">Use AI, but <strong>accept a non-zero chance of errors</strong> slipping through.<br>
      <em>Example: help with CSS for a workshop webpage or vibe-coding a small demo.</em></td>
      <td class="bp-green"><strong>Delegate most of the work to AI</strong>. Verify that the output makes sense.<br>
      <em>Example: generating documentation for scripts you wrote, or drafting an outline of a presentation from a transcription of your own recordings.</em></td>
    </tr>
  </tbody>
</table>

<style>
.ref-line { font-size: 0.7rem; opacity: 0.75; margin: -0.6rem 0 0.6rem; }
p { font-size: 0.8rem; line-height: 1.35; margin: 0 0 0.6rem; }
/* Outer frame on the table, like the theme's tables (layouts.css:176); cells only draw the inner lines */
.bp-matrix { width: 100%; margin: 0; border-collapse: separate; border-spacing: 0; border: 1px solid var(--asc-border); border-radius: var(--asc-radius-lg); overflow: hidden; font-size: 0.7rem; line-height: 1.35; }
.bp-matrix th, .bp-matrix td { padding: 0.4rem 0.6rem; border: 0; border-right: 1px solid var(--asc-border); border-bottom: 1px solid var(--asc-border); vertical-align: top; text-align: left; }
.bp-matrix th:last-child, .bp-matrix td:last-child { border-right: 0; }
.bp-matrix tbody tr:last-child td { border-bottom: 0; }
/* Dark header row, same colours as the theme's dark card (layouts.css:239) */
.bp-matrix th { background: var(--asc-night); color: var(--asc-paper); font-size: 0.85rem; }
.bp-matrix td:first-child { width: 22%; }
.bp-matrix em { display: block; margin-top: 0.35rem; }
/* Risk colours at 50% so they blend with the white table into lighter tints; high risk + low expertise is the most dangerous cell */
.bp-matrix .bp-red { background: color-mix(in srgb, var(--aalto-red) 50%, transparent); color: #000; }
.bp-matrix .bp-orange { background: color-mix(in srgb, var(--aalto-orange) 50%, transparent); color: #000; }
.bp-matrix .bp-darkyellow { background: color-mix(in srgb, var(--aalto-darkyellow) 50%, transparent); color: #000; }
.bp-matrix .bp-green { background: color-mix(in srgb, var(--aalto-green) 50%, transparent); color: #000; }
</style>






---
layout: end
---

# Take home message

**If you do not have the ability or the resources to verify the output of AI systems** (e.g. by finding the relevant citations for the synthesised text, by verifying that others’ works are summarised correctly, by detecting plagiarised text or code, by verifying the analysis code) **then you should not use the output of AI systems beyond self-learning or brainstorming.**

<br>
<br>

We are all learning together, join our dedicated <a href="https://www.aalto.fi/en/services/ai-training-for-the-entire-aalto-community">trainings on AI tools in research</a>, or come talk with <a href="https://www.aalto.fi/en/services/research-software-engineers">Aalto Research Software Engineers</a> and <a href="https://www.aalto.fi/en/services/data-agents">Aalto Data Agents</a>.


<style>
/* layouts.css:651 sets end-slide text to --asc-muted (light grey on dark); bold goes white */
.slidev-layout.end p:first-of-type { font-size: 1.4rem; line-height: 1.35; }
.slidev-layout.end strong { color: var(--asc-text); }
</style>
