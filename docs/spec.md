# Portfolio Site — Spec

Source-of-truth content/requirements for the `portfolio-draft` site. Update
this file whenever content changes so it stays in sync with `index.html`.

## Status

- [x] Trial repo built and deployed
- [ ] Add email / LinkedIn / other links
- [ ] Add featured projects section
- [ ] Add resume PDF
- [ ] Add profile photo
- [ ] Migrate to final `aibyanand.github.io` repo once approved

## Identity

- **Name:** Anand Shridhar Sawant
- **Role / title:** Director, Power, Performance & On-device Machine Learning
- **GitHub:** https://github.com/aibyanand
- **Email:** _not provided yet_
- **LinkedIn:** _not provided yet_
- **Other links:** _none yet_

## Bio

Director-level engineering leader with 14+ years at Intel and 10 years at
Texas Instruments driving Power, Performance, Thermal, and On-Device AI/ML
(ODML) optimization at SoC & System level. Proven track record of optimizing
& shipping 20+ Android phones/tablets, ChromeOS, and Linux laptop products —
ranging from the Chromebook with the lowest battery (38 WHr) to the Sep '26
launch of the Panther Lake-based Googlebook. Deep expertise of optimizing AI
workloads — delivering up to 30% performance gains in Gemini Nano LLM
inference on NPU/GPU and 25% power savings in Video Conf with AI effects.
Fluent with handling the entire PnP pipeline from targets, feature dev,
optimization to customer support. Master's in Telecom from IISc, Bangalore
plus four advanced AI/ML courses (Deep Learning, Generative AI, Reinforcement
Learning, LLM Inference & Agents) applied directly to production platforms
and recent focus on inference optimization on consumer/DC GPUs using various
techniques. Proven track record of building and leading high-performing
multi-geo engineering organization that has filed 10+ patents & published
10+ papers.

## Skills / Focus Areas

1. **On-Device AI / LLM Optimization** — Gemini Nano, Llama, Stable Diffusion
   inference optimization on NPU & GPU for encode/decode latency/memory;
   Video Conferencing (VC) with AI effects.
2. **Power, Performance, Thermal, User Exp** — Standby & Active Power for SoC
   & System, CPU/GPU/Browser/Memory Performance, long-duration Thermal, Key
   Product User Experience.
3. **Emerging KPIs & Compliance** — App Performance, Gaming, Energy & Noise
   Compliance.
4. **Silicon Bring-up & Power Frameworks** — Power Management Framework &
   PnP feature development on pre- and post-Si platforms; Platform
   configuration & tuning.
5. **Engineering & Program Management** — Multi-geo teams, planning,
   execution, career development, contractor management, program management
   & Arch forum interface.
6. **Customer & Ecosystem Collaboration** — Google co-development for
   Chromebook & Googlebook, ODM/OEM support for lead/scaling products,
   Marketing support for design wins.
7. **Innovation & IP** — Team filed 10+ patents & 10+ papers; AI/Agentic
   tools for Automation & Optimization.

## Projects

None listed currently (explicitly deferred — see Status above).

## Design requirements

- Single page, responsive (works down to ~400px wide).
- Light/dark mode support, follows system preference by default, with a
  manual toggle.
- No external dependencies/CDNs — system fonts only.
- Sections: top nav → hero → about (with stat row) → skills grid → contact →
  footer.

## Deployment target

- **Current (trial):** `aibyanand/portfolio-draft` →
  https://aibyanand.github.io/portfolio-draft/
- **Final (pending approval):** migrate to `aibyanand/aibyanand.github.io` →
  https://aibyanand.github.io/
