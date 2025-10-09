---
theme: '@doctolib/slidev-theme'
title: Debt Busters - How AI Became My Technical Debt Sidekick
info: |
  ## Debt Busters: How AI Became My Technical Debt Sidekick
  A talk about leveraging AI to tackle technical debt effectively.
class: text-center
drawings:
  persist: false
transition: slide-left
mdc: true
background: https://images.unsplash.com/photo-1558317374-067fb5f30001?q=80&w=1740&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
favicon: 'https://www.doctolib.fr/icon_patient/180x180.png'
---

# Debt Busters

How AI Became My Technical Debt Sidekick

---
layout: cover
background: https://images.unsplash.com/photo-1529220502050-f15e570c634e?q=80&w=1858&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
class: text-white
---

# Case Study #1

Fix all tests related to Organization for Patient Base Migration

---

# The Challenge

<div class="grid grid-cols-2 gap-8">
<div>

## The Problem
- Organization violations was not track in test files
- Hundreds of tests to refactor
- Complex test dependencies
- Time-sensitive project

</div>
</div>

---

# What Happened Concretely

<div class="space-y-6">

## Step-by-Step Process

- **Plan**: AI analyzed 200+ test files, identified common patterns and define resolution patterns
- **Fix in Batch**: Start 10 agents to fix all tests
- **Run all tests to check**: Detect complex cases
- **Alignement**: Manual review and edge case handling
- **Trade-off**: Some tests was too complex to be fixed and are removed from the PR


<v-clicks>

## Result 💡

<div class="mt-2 p-4 bg-blue-500/10 rounded">
More than half tests refactored with AI assistance letting all teams focusing on the complex cases
</div>

</v-clicks>

</div>

---

# Key Takeaways

<div class="grid grid-cols-2 gap-8">
<div>

## What Worked ✅

- AI is great to apply refactoring patterns at scale
- **Batch processing** allow a quick fix
- Combining AI speed with **human review** to ensure acceptation

</div>
<div>

## What Didn't Work ❌

- AI struggled with **edge cases** and complex business logic
- Factories with **non-standard** implementation like Agenda
- Some tests needed **100% manual** refactoring

</div>
</div>

## Lessons Learned 💡

<div class="mt-2 p-4 bg-blue-500/10 rounded">
AI is a powerful accelerator, but not a replacement for understanding your codebase
</div>

---
layout: cover
background: https://images.unsplash.com/photo-1577401159468-3bbc7ee440b5?q=80&w=1740&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
class: text-white
---

# Case Study #2

Finding Owners for 54 Feature Switches

---

# On a sunny monday morning - Vitals on fire

<div class="relative h-full pt-8">
  <div class="flex items-start justify-center">
    <img v-click="3" src="/list3.png" class="w-80 shadow-lg -mr-20" />
    <img v-click="1" src="/list1.png" class="w-80 shadow-lg -mr-20" />
    <img v-click="2" src="/list2.png" class="w-80 shadow-lg -mr-20" />
    <img v-click="4" src="/list4.png" class="w-80 shadow-lg" />
  </div>

  <div v-click="5" class="absolute top-1/3 left-1/2 transform -translate-x-1/2 -translate-y-1/2">
    <iframe src="https://giphy.com/embed/Cdkk6wFFqisTe" width="480" height="331" frameBorder="0" class="giphy-embed shadow-2xl" allowFullScreen></iframe>
  </div>
</div>

---

# The Challenge

<div class="grid grid-cols-2 gap-8">
<div>

## The Problem
- 54 feature switches affected **by default** to our team
- Reassigned to our team "by mistake"
- No documentation
- Unknown business impact

</div>
<div v-click>

## AI-Assisted Methodology

1. **Create a plan**: Ask AI to generate a file with each FS, owner and a rational with a placeholder... Commit !
2. **Code archaeology**: started 10 agents with a mission to use MCPs to investigate
3. **Ownership assignation**: Fill the file with suggested owner, level of certitude and a rational with a link
4. **Ping all teams**: Start negociation

</div>
</div>

---

# PR creation

<div class="space-y-4">

## MCPs for the win

<v-clicks>

- **AI scanned github && git history** for each switch: original PRs, authors, related changes
- **Confluence and JIRA**: who created FS and where are they used
- **DUST**: gather a vision from another LLM

</v-clicks>

<div v-click class="mt-6 grid grid-cols-3 gap-4">

<div class="p-4 bg-green-500/10 rounded">

**50 FS**
reaffected

</div>

<div class="p-4 bg-yellow-500/10 rounded">

**4 FS**
deleted

</div>

<div class="p-4 bg-blue-500/10 rounded">

**0 FS**
for our team 🎉

</div>

</div>

<div v-click class="grid w-auto h-100px"><iframe src="https://giphy.com/embed/qngUbAbaWRuFy" width="100%" height="100%" frameBorder="0" class="giphy-embed" allowFullScreen></iframe></div>

</div>

---

# Ownership assignment

<img src="/fire.gif" />

---

# Key Takeaways

<div class="grid grid-cols-2 gap-8">
<div>

## What Worked ✅

- Commit a plan at first and ask AI to update it faciliate parallelization
- Ai detected unused FS and suggeted to delete them
- 1 PR helps to gather aggreement between teams
- Having a suggested ownership and a rational forced teams to suggest a better owner

</div>
<div>

## What Didn't Work ❌

- More than half suggestions was invalid 🙃
- **Hallucination** on one team name and suggested deleted Doctoteams

</div>
</div>

---

# Pull Requests

<div class="space-y-8">

## Case Study #1: Test Refactoring
[PR Link - Tests Organization Migration](https://github.com/doctolib/doctolib/pull/216509)

## Case Study #2: Feature Switch Ownership
[PR Link - Feature Switch Ownership](https://github.com/doctolib/doctolib/pull/217841)

</div>

---
layout: cover
background: https://images.unsplash.com/photo-1665789318391-6057c533005e?q=80&w=2064&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D
class: text-center
---

# Questions?

Thank you!

<img src="/QrCode.png" class="absolute bottom-10 right-10 w-40 h-40 bg-white p-2 rounded" />
