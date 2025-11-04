---
layout: page
title: AgenticSE workshop
description: First international Wokrshop on Autonomous Agents in Software Engineering, co-located iwth ASE 2025, Seoul, South Korea
---

<img src="assets/img/agenticSE.png" alt="banner" style="display: block; margin: auto; width: 500px;">


Autonomous agents powered by Large Language
Models are reshaping software engineering, enabling AI systems
that plan, code, test, and deploy with less human intervention. Despite rapid progress and growing industry interest, the Software
Engineering community lacks a dedicated venue to explore these
developments. The Autonomous Agents in Software Engineering
(AgenticSE) workshop aims to fill this gap by bringing together
researchers and practitioners to discuss agentic architectures,
applications in code generation, testing, DevOps, human-agent
collaboration, and evaluation. AgenticSE is a timely and essential
step toward building a community around this transformative
and underexplored direction in software engineering.

AgenticSE will be held on **November 20, 2025** co-located with ASE'25.


### Organizing Committee
<!-- <div align="center" style="display: flex; justify-content: center; gap: 10px;">

  <figure style="text-align: center;">
    <img src="assets/img/mali.jpg" alt="mali" style="width:30%;">
    <figcaption>Maliheh Izadi, TU Delft</figcaption>
  </figure>

  <figure style="text-align: center;">
    <img src="assets/img/michael.jpg" alt="michael" style="width:30%;">
    <figcaption>Michael Pradel, Stuttgart</figcaption>
  </figure>

  <figure style="text-align: center;">
    <img src="assets/img/satish.jpg" alt="satish" style="width:30%;">
    <figcaption>Satish Chandra, Google</figcaption>
  </figure>
</div> -->
<style>
  /* Organizing/Program committee tiles: responsive layout */
  .committee-grid { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 16px; width: 100%; text-align: center; }
  .committee-grid figure { margin: 0; padding: 10px; box-sizing: border-box; }
  .committee-grid img { width: 100%; max-width: 320px; height: auto; display: block; margin: 0 auto; }
  @media (max-width: 900px) {
    .committee-grid { grid-template-columns: repeat(2, minmax(0, 1fr)); }
  }
  @media (max-width: 600px) {
    .committee-grid { grid-template-columns: 1fr; }
  }
  /* Program Committee table responsiveness */
  .responsive-table { width: 100%; overflow-x: auto; -webkit-overflow-scrolling: touch; }
  .responsive-table table { width: 100%; border-collapse: collapse; }
  .responsive-table th, .responsive-table td { padding: 8px; border-bottom: 1px solid #ddd; text-align: left; white-space: nowrap; }
  .responsive-table thead { background: #f7f7f7; }
  @media (max-width: 700px) {
    .responsive-table th, .responsive-table td { padding: 6px; }
  }
</style>

<div class="committee-grid">

  <figure>
    <img src="assets/img/mali.jpg" alt="x" style="width: 100%; height: auto; display: block; margin: 0 auto;">
    <figcaption style="margin-top: 10px; padding: 10px; border: 1px solid #ccc; background-color: #f9f9f9; font-weight: bold;">
      <a href="https://malihehizadi.github.io/">Maliheh Izadi</a>, TU Delft
    </figcaption>
  </figure>

  <figure>
    <img src="assets/img/michael.jpg" alt="x" style="width: 100%; height: auto; display: block; margin: 0 auto;">
    <figcaption style="margin-top: 10px; padding: 10px; border: 1px solid #ccc; background-color: #f9f9f9; font-weight: bold;">
      <a href="https://software-lab.org/people/Michael_Pradel.html">Michael Pradel</a>, CISPA
    </figcaption>
  </figure>

  <figure>
    <img src="assets/img/satish.jpg" alt="x" style="width: 100%; height: auto; display: block; margin: 0 auto;">
    <figcaption style="margin-top: 10px; padding: 10px; border: 1px solid #ccc; background-color: #f9f9f9; font-weight: bold;">
      <a href="https://sites.google.com/site/schandraacmorg/">Satish Chandra</a>, Meta Platforms, Inc
    </figcaption>
  </figure>

</div>


### Speakers
We are excited to welcome distinguished speakers who will share their expertise on the role of agents in advancing software engineering, offering insights from both research and practice.

<strong><a href="https://alexandermossin.com/">Alexander Mossin</a></strong> is a software engineer with a passion for building beautiful and intelligent products who is currently at Google Labs, working on the next generation of AI tools. Alexander's primary expertise and interest is building robust distributed systems, ML infrastructure, automated evaluation solutions and data pipelines for AI. His team's mission is to harness cutting-edge AI to revolutionize the usefulness of AI and foundation models. His most recent accomplishments include launching AI-based video dubbing using foundation models and combining information retrieval with deep learning for medical records.

<strong><a href="https://www.linkedin.com/in/mehadi-hassen-05306016/">Dr. Mehadi Hassen</a></strong> is a Staff Research Engineer at Google with extensive experience developing and leading AI-powered coding products. He holds a PhD in Computer Science and is the current Research/Modeling Lead for Jules (jules.google.com). He has over a decade of experience studying the intersection of machine learning, coding, and computer security.

<strong><a href="https://chao-peng.github.io/">Dr. Chao Peng</a></strong> is a Principal Research Scientist at ByteDance. He received his PhD degree from The University of Edinburgh. At ByteDance, he leads the Trae Research team, where they conduct research on AI agents for software engineering including the application and evaluation of AI agents, and training LLMs for agents. He is also responsible for academic development and university collaboration. Dr. Chao Peng has published research and industry papers at premier venues including ICSE, FSE, ASE, ACL and serves as a PC member for FSE and ASE.

<style>
  /* Keynotes layout: two side-by-side photos with a shared description; responsive */
  .keynotes { display: flex; flex-direction: column; gap: 24px; width: 100%; }
  .keynote-grid { display: grid; grid-template-columns: repeat(2, minmax(0, 1fr)); gap: 16px; align-items: start; }
  .keynote-grid.columns-1 { grid-template-columns: 1fr; }
  .keynote-grid figure { margin: 0; }
  /* Prevent overly large profile photos while keeping them responsive */
  .keynote-grid img { width: 100%; max-width: 320px; height: auto; display: block; margin: 0 auto; }
  .keynote-grid figcaption { margin-top: 8px; padding: 10px; border: 1px solid #ccc; background-color: #f9f9f9; }
  .keynote-desc { grid-column: 1 / -1; padding: 12px; border: 1px solid #ccc; background-color: #fdfdfd; }
  @media (max-width: 700px) {
    .keynote-grid { grid-template-columns: 1fr; }
  }
</style>

<div class="keynotes">

  <!-- Keynote 1: Google (alphabetical among Google): Hassen, Mossin) -->
  <div class="keynote-grid columns-2">
    <figure>
      <img src="assets/img/mehadi.jpg" alt="Portrait of Mehadi Hassen">
      <figcaption>
        <strong><a href="https://www.linkedin.com/in/mehadi-hassen-05306016/">Mehadi Hassen</a></strong>, Google
      </figcaption>
    </figure>
    <figure>
      <img src="assets/img/alexandermossin.jpg" alt="Portrait of Alexander Mossin">
      <figcaption>
        <strong><a href="https://alexandermossin.com/">Alexander Mossin</a></strong>, Google
      </figcaption>
    </figure>
    <div class="keynote-desc">
      <strong>Title</strong>: Building Jules, Google's first external coding agent
      <br/>
      <strong>Abstract</strong>: We explore critical considerations for developing and deploying coding agents at scale in a production environment that has generated over 250k commits to date. We delve into architectural decisions, including interactivity, multi-agent systems, orchestration, state management, security, sandboxing, observability, and effective tool design. We will also address real-world challenges such as debugging, balancing quality with user experience needs (features, latency), and the trade-offs between rapid iteration and careful measurement.
    </div>
  </div>

  <!-- Keynote 2: ByteDance -->
  <div class="keynote-grid columns-1">
    <figure>
      <img src="assets/img/Chao.jpg" alt="Portrait of Chao Peng">
      <figcaption>
        <strong><a href="https://chao-peng.github.io/">Chao Peng</a></strong>, ByteDance
      </figcaption>
    </figure>
    <div class="keynote-desc">
      <strong>Title</strong>: Trae Agent: SOTA Open-source AI Coding Agent for SWE-bench
      <br/>
      <strong>Abstract</strong>: In this talk, we spotlight Trae Agent’s remarkable achievement of securing the top position on the SWE-bench Verified leaderboard with a 75.2% success rate. Trae Agent, an intelligent LLM-based assistant, has demonstrated exceptional capabilities in autonomously debugging complex issues, implementing robust fixes, and navigating intricate codebases. This session will explore the methodologies behind Trae Agent’s performance, including its innovative patch generation and selection strategies, and the integration of multiple LLMs. Additionally, we will discuss the significance of making Trae Agent open-source, fostering community collaboration, and accelerating the evolution of AI in software development.
    </div>
  </div>

</div>


### Support Team
<div class="committee-grid">

  <figure>
    <img src="assets/img/mehdi.jpg" alt="x" style="width: 100%; height: auto; display: block; margin: 0 auto;">
    <figcaption style="margin-top: 10px; padding: 10px; border: 1px solid #ccc; background-color: #f9f9f9; font-weight: bold;">
      <a href="https://ashkboos.github.io/MyWebsite/">Mehdi Keshani</a><br/>Proceeding Chair
    </figcaption>
  </figure>

  <figure>
    <img src="assets/img/razvan.webp" alt="x" style="width: 100%; height: auto; display: block; margin: 0 auto;">
    <figcaption style="margin-top: 10px; padding: 10px; border: 1px solid #ccc; background-color: #f9f9f9; font-weight: bold;">
      <a href="https://razvain.github.io/">Razvan Popescu</a><br/>Web Chair
    </figcaption>
  </figure>

  <figure>
    <img src="assets/img/roham.webp" alt="x" style="width: 100%; height: auto; display: block; margin: 0 auto;">
    <figcaption style="margin-top: 10px; padding: 10px; border: 1px solid #ccc; background-color: #f9f9f9; font-weight: bold;">
      <a href="http://rohamkoohestani.com/">Roham Koohestani</a><br/>Web Chair
    </figcaption>
  </figure>
</div>

### Target Audience
- Software Engineering (SE): researchers and practitioners interested in AI-driven development, automation, program analysis, testing, maintenance, and DevOps. 

- Artificial Intelligence (AI): those working on LLMs, planning agents, multi-agent systems, and human-AI interaction. 

- Programming Languages (PL): experts in program synthesis, static analysis, compilers, and formal methods who can explore how agents reason about code and specifications.

- Human-Computer Interaction (HCI): researchers studying how developers interact with AI assistants/agents, UX design
for AI agents, and cognitive implications of AI partners. Systems and DevOps: practitioners in CI/CD and software infrastructure interested in autonomous agents for environment setup, deployment, monitoring, and optimization.

We expect a mix of academia and industry attendees. **Industrial participation** is highly encouraged (e.g., teams building
AI-powered developer tools and intelligent IDEs, autonomous bots in DevOps workflows, or automated project management). By drawing from multiple communities (AI, SE, PL, HCI), the workshop promotes diverse viewpoints and networking among groups that do not often overlap, seeding a new collaborative community.


### Format and Dates
Types of submissions include **full papers, short papers, and late-breaking talk-only (extended abstract)** submissions:

* **Long papers** = 8 pages (inclduing references) in IEEEtran two-column formatting
* **Short papers** = 4 pages (inclduing references) in IEEEtran two-column formatting
* **Talk-only**: Text-only abstract, without a formal publication (no proceedings)

- **Paper submission**: ~~Aug 22nd, 2025~~ **Aug 26th, 2025, 23:59 AOE**
- **Notification Date**: Sep 26th, 2025, 23:59 AOE
- **Camera-ready deadline**: Oct 5th, 2025, 23:59 AOE

### Topics of Interest
Topics of Interest include, but are not limited to:
- Architectures and frameworks for autonomous software engineering agents
- Multi-agent collaboration in software development environments
- LLM-powered autonomous development and debugging assistants
- Self-improving and self-repairing software systems
- Automated requirements elicitation and refinement via agents
- Autonomous testing, verification, and validation strategies
- Human–agent interaction and collaboration in SE workflows
- Safety, reliability, and trust in agentic software engineering tools
- Evaluation metrics and benchmarks for autonomous SE agents
- Ethical, legal, and societal implications of agentic SE tools
- Case studies and industrial experiences with autonomous agents in SE
- Tool demonstrations and experimental platforms for agentic SE

### Review Procedure
All submitted papers will undergo peer-review process. Each paper will be reviewed by at least 3 PC members
to ensure multiple perspectives. We will follow a double-blind reviewing process. Reviewers will evaluate submissions
based on relevance to the workshop, technical quality, novelty/originality, and potential to stimulate discussion. Position
and vision papers might be judged more on insightfulness and
relevance than on new results, given the emerging nature of
the field.


### Program Committee

<div class="responsive-table">
  <table>
    <thead>
      <tr>
        <th>Name</th>
        <th>Affiliation</th>
        <th>Country</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><a href="https://www.cs.queensu.ca/people/Ahmed%20E./Hassan">Ahmed Hassan</a></td>
        <td>Queen's University</td>
        <td>Canada</td>
      </tr>
      <tr>
        <td><a href="https://ankit.website">Ankit Agrawal</a></td>
        <td>Saint Louis University</td>
        <td>USA</td>
      </tr>
      <tr>
        <td><a href="https://chao-peng.github.io/">Chao Peng</a></td>
        <td>ByteDance</td>
        <td>China</td>
      </tr>
      <tr>
        <td><a href="https://ctreude.ca/">Christoph Treude</a></td>
        <td>Singapore Management University</td>
        <td>Singapore</td>
      </tr>
      <tr>
        <td><a href="https://www.microsoft.com/en-us/research/people/gsoares/">Gustavo Soares</a></td>
        <td>Microsoft</td>
        <td>USA</td>
      </tr>
      <tr>
        <td><a href="https://heye.me/">He Ye</a></td>
        <td>University of College London</td>
        <td>UK</td>
      </tr>
      <tr>
        <td><a href="https://ics.uci.edu/~iftekha/">Iftekhar Ahmed</a></td>
        <td>University Of California, Irvine</td>
        <td>USA</td>
      </tr>
      <tr>
        <td><a href="https://insights.sei.cmu.edu/authors/ipek-ozkaya/">Ipek Ozkaya</a></td>
        <td>Carnegie Mellon Software Engineering Institute</td>
        <td>USA</td>
      </tr>
      <tr>
        <td><a href="https://www.software-lab.org/people/Islem_Bouzenia.html">Islem Bouzenia</a></td>
        <td>University of Stuttgart</td>
        <td>Germany</td>
      </tr>
      <tr>
        <td><a href="https://sites.google.com/view/jie-zhang/home">Jie M. Zhang</a></td>
        <td>King's College London</td>
        <td>UK</td>
      </tr>
      <tr>
        <td><a href="https://jxhe.info/">Jingxuan He</a></td>
        <td>UC Berkeley</td>
        <td>USA</td>
      </tr>
      <tr>
        <td><a href="http://JKatzy.nl">Jonathan Katzy</a></td>
        <td>Delft University of Technology</td>
        <td>Netherlands</td>
      </tr>
      <tr>
        <td><a href="https://ipa-lab.github.io/">Jürgen  Cito</a></td>
        <td>TU Wien</td>
        <td>Austria</td>
      </tr>
      <tr>
        <td><a href="https://people.csiro.au/L/Q/Qinghua-Lu">Qinghua Lu</a></td>
        <td>CSIRO</td>
        <td>New Zealand</td>
      </tr>
      <tr>
        <td><a href="https://research.google/people/108096/?&type=google">Sarah D'Angelo</a></td>
        <td>Google</td>
        <td>Australia</td>
      </tr>
      <tr>
        <td><a href="https://bryksin.me/">Timofey Bryksin</a></td>
        <td>JetBrains Research</td>
        <td>Cyprus</td>
      </tr>
      <tr>
        <td><a href="https://petertsehsun.github.io/">Tse-Hsun (Peter) Chen</a></td>
        <td>Concordia University</td>
        <td>Canada</td>
      </tr>
      <tr>
        <td><a href="https://yilinglou.github.io/">Yiling Lou</a></td>
        <td>Fudan University</td>
        <td>China</td>
      </tr>
      <tr>
        <td><a href="http://ziyou.li">Ziyou Li</a></td>
        <td>Delft University of Technology</td>
        <td>Netherlands</td>
      </tr>
    </tbody>
  </table>
</div>



### Publication of Proceedings
We intend for accepted papers to be published in the ASE 2025 workshop proceedings. ASE workshop track home: [https://conf.researchr.org/track/ase-2025/ase-2025-workshops](https://conf.researchr.org/track/ase-2025/ase-2025-workshops).


### Submission Link
Submission site: [https://agenticse2025.hotcrp.com/](https://agenticse2025.hotcrp.com/)



For more info or questions reach out to m[dot]izadi[at]tudelft.nl



