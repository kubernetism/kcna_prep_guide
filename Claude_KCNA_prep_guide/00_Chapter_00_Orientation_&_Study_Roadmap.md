# Chapter 0: Before You Begin — Orientation & Study Roadmap

*KCNA Prep Guide Writer | Facts verified against official Linux Foundation/CNCF sources — see citations throughout. Exam pricing, weights, and policy change periodically; always cross-check the [official exam page](https://training.linuxfoundation.org/certification/kubernetes-cloud-native-associate/) before you register.*

---

## 0.1 What This Guide Is (and Isn't)

This is a study companion for the **Kubernetes and Cloud Native Associate (KCNA)** exam, issued by the Cloud Native Computing Foundation (CNCF) and administered by The Linux Foundation. It will walk you domain-by-domain through the official curriculum, point you to primary documentation, and give you original practice questions to test yourself with.

What this guide will **never** do: present real, leaked, or reconstructed exam questions as study material. The Linux Foundation's Candidate/Certification Agreement explicitly prohibits sharing or soliciting actual exam content — commonly called "braindumping" — and violating it can get a certification revoked. Every practice question in this guide is original, written to match the style and difficulty of the public curriculum, and clearly labeled as unofficial.

If you find yourself on a site promising "real exam dumps" or a "guaranteed pass" test engine, close the tab. Those sites are a policy violation waiting to happen, and in my experience they're also frequently just wrong — stale weightings, invented question formats, no accountable author. This guide sources exam facts only from official Linux Foundation/CNCF pages, and technical concepts only from primary project documentation.

---

## 0.2 Exam Snapshot

| Attribute | Detail |
|---|---|
| Full name | Kubernetes and Cloud Native Associate (KCNA) |
| Issuer | CNCF, administered by The Linux Foundation |
| Level | Pre-professional / entry-level — no prerequisites |
| Format | Online, remotely proctored, multiple-choice (single- and multi-answer) |
| Length | 60 questions in 90 minutes (~90 seconds/question budget) |
| Passing score | 75% |
| Price | $250 exam-only · $299 bundled with LFS250 course · $495 bundled with a THRIVE-ONE annual subscription |
| Scheduling window | 12 months from purchase to sit the exam |
| Attempts | 2 (one free retake included) |
| Validity | 2 years from the pass date |

*Source: [official KCNA certification page](https://training.linuxfoundation.org/certification/kubernetes-cloud-native-associate/). Prices and bundles are the kind of thing that shifts — verify before you buy.*

**Important framing:** unlike CKA or CKAD, KCNA has **no hands-on lab component**. It's entirely multiple-choice. That doesn't mean you should skip the terminal — running `kubectl` builds the intuition that makes multiple-choice questions about Kubernetes behavior easy instead of a memorization slog. More on that in §0.5.

---

## 0.3 Who This Is For

KCNA is designed as an **entry point**, not a professional credential proving hands-on operational skill. It's a good fit if you are:

- New to Kubernetes and want a structured, vendor-neutral way to prove foundational knowledge
- A developer, PM, sales engineer, or support engineer who touches cloud-native systems but doesn't administer clusters day-to-day
- Planning to eventually pursue CKA (administration), CKAD (application development), or KCSA (security) and want a lower-stakes first certification to build momentum
- Working toward the CNCF **Kubestronaut** program, which recognizes people who've earned KCNA plus the other core CNCF certifications

It's a *less* good fit — though still valuable — if you're already administering production Kubernetes clusters; you may find the material easy and want to skip straight to CKA.

---

## 0.4 Domain Breakdown & Where to Spend Your Time

Domain weights come directly from the official curriculum. **Note:** you'll encounter older blog posts and study guides online citing a different breakdown (Kubernetes Fundamentals 46%, Container Orchestration 22%, Cloud Native Architecture 16%, Observability 8%, Application Delivery 8%, as five separate domains). That reflects a prior version of the curriculum. Always trust the live weighting on the [official exam page](https://training.linuxfoundation.org/certification/kubernetes-cloud-native-associate/) and the [CNCF curriculum PDF](https://github.com/cncf/curriculum/blob/master/KCNA_Curriculum.pdf) over any cached number — including the table below, which you should re-verify at the start of your studies.

| Domain | Weight | Competencies |
|---|---|---|
| **Kubernetes Fundamentals** | 44% | Core Concepts, Administration, Scheduling, Containerization |
| **Container Orchestration** | 28% | Networking, Security, Troubleshooting, Storage |
| **Cloud Native Application Delivery** | 16% | Application Delivery, Debugging |
| **Cloud Native Architecture** | 12% | Observability, Cloud Native Ecosystem & Principles, Community & Collaboration |

**Study time allocation should roughly track these weights.** Kubernetes Fundamentals and Container Orchestration together are 72% of the exam — that's where the bulk of your hours belong. Don't let the "soft-sounding" Cloud Native Architecture domain (CNCF governance, project maturity levels, the landscape, personas) get skipped just because it feels less technical — it's still 12% of your score, and it's some of the easiest material to learn quickly because it's conceptual, not hands-on.

---

## 0.5 Why You Should Still Touch a Terminal

The exam is 100% multiple-choice — no live cluster, no YAML to write under pressure. So why practice `kubectl`?

Because KCNA questions test *behavioral intuition*: "If you scale a Deployment from 3 to 5 replicas, what happens to the underlying ReplicaSet?" is much easier to answer correctly if you've actually watched it happen, rather than memorized a diagram. A few hours in a free sandbox will save you more exam points than the same hours spent re-reading definitions.

You don't need a paid cloud account. Free options:
- [Killercoda](https://killercoda.com/) — interactive, browser-based Kubernetes scenarios, no install required
- [Play with Kubernetes](https://labs.play-with-k8s.com/) — spin up a throwaway multi-node cluster in the browser
- [minikube](https://minikube.sigs.k8s.io/docs/start/) — a real local single-node cluster on your own machine
- [kind](https://kind.sigs.k8s.io/) — local multi-node clusters running in Docker

A good minimum viable practice set: deploy a Pod, scale a Deployment, expose it via a Service, look at its logs and events, and deliberately break something (bad image name, wrong port) so you recognize `CrashLoopBackOff` and `ImagePullBackOff` on sight rather than from a textbook definition.

---

## 0.6 How This Guide Is Organized

| Chapter | Covers |
|---|---|
| 0 (this chapter) | Orientation, exam facts, personalization |
| 1 | Cloud Native Architecture — CNCF, the landscape, project maturity, personas |
| 2 | Kubernetes Fundamentals — architecture, objects, API, scheduling |
| 3 | Container Orchestration — networking, storage, security, troubleshooting |
| 4 | Cloud Native Application Delivery — CI/CD, GitOps, debugging |
| 5 | Observability — logs, metrics, traces |
| 6 | Hands-on lab walkthroughs |
| 7 | Full-length original practice exam + answer explanations |
| 8 | Exam-day logistics and what comes after |

Each domain chapter follows the same shape: must-know terms with plain-language explanations, links to the specific primary-documentation page (not just a homepage), and a short practice question set labeled clearly as original, unofficial material.

---

## 0.7 Quick Personalization Check

Before I build out your study timeline (4-week intensive vs. 8-week steady-pace, or something scaled to an already-booked exam date), it'll help to know where you're starting from.