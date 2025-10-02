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
- Patient Base migration needed
- Hundreds of tests to refactor
- Complex test dependencies
- Time-sensitive project

</div>
<div v-click>

## AI-Assisted Approach

1. **Analyze patterns** in existing tests
2. **Generate refactoring rules** with AI
3. **Batch processing** with AI validation
4. **Human review** of critical changes

</div>
</div>

---

# What Happened Concretely

<div class="space-y-6">

## Step-by-Step Process

<v-clicks>

- **Week 1**: AI analyzed 200+ test files, identified common patterns
- **Week 2**: Generated transformation scripts for test structure changes
- **Week 3**: Applied changes in batches of 20-30 tests with AI review
- **Week 4**: Manual review and edge case handling

</v-clicks>

<div v-click class="mt-2 p-4 bg-blue-500/10 rounded">
Result: 85% of tests refactored with AI assistance, 4 weeks instead of estimated 12
</div>

</div>

---

# Key Takeaways

<div class="grid grid-cols-2 gap-8">
<div>

## What Worked ✅

- AI excels at **pattern recognition** in code
- **Batch processing** with validation caught most issues
- Combining AI speed with **human judgment** for critical paths

</div>
<div>

## What Didn't Work ❌

- AI struggled with **edge cases** and complex business logic
- Required **constant validation** to avoid introducing bugs
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

Finding Owners for 60+ Feature Switches

---

# The Challenge: Feature Switch Ownership

<div class="grid grid-cols-2 gap-8">
<div>

## The Problem
- 60+ orphaned feature switches
- Reassigned to our team
- No documentation
- Unknown business impact

</div>
<div v-click>

## AI-Assisted Methodology

1. **Code archaeology**: trace usage patterns
2. **Git history analysis**: find original authors
3. **Impact assessment**: understand dependencies
4. **Documentation generation**: create ownership records

</div>
</div>

---

# What Happened After

<div class="space-y-4">

## The Investigation Process

<v-clicks>

- **AI scanned git history** for each switch: original PRs, authors, related changes
- **Generated usage reports**: where switches are used, how often toggled
- **Identified stakeholders**: mapped code ownership to team structure
- **Created documentation**: automated feature switch registry

</v-clicks>

<div v-click class="mt-6 grid grid-cols-3 gap-4">

<div class="p-4 bg-green-500/10 rounded">

**30 switches**
Owners found

</div>

<div class="p-4 bg-yellow-500/10 rounded">

**20 switches**
Deprecated

</div>

<div class="p-4 bg-blue-500/10 rounded">

**10 switches**
Need discussion

</div>

</div>

</div>

---

# Key Takeaways: Feature Switch Ownership

<div class="space-y-6">

## What Worked ✅

- AI + git history = powerful **archaeology tool**
- Automated **documentation generation** saved hours
- Pattern matching across **thousands of commits**

## Challenges ⚠️

- Old switches had **lost context** over time
- Required **human validation** of assumptions
- Some decisions still needed **business input**

## Best Practices 🎯

- **Document ownership** from day one
- Use AI for investigation, **humans for decisions**
- Feature switches need **lifecycle management**

</div>

---
layout: center
class: text-center
---

# Conclusion

## AI is Your Technical Debt Sidekick, Not a Silver Bullet

<div class="pt-8">

Use AI for speed, use humans for judgment

</div>

---
layout: center
class: text-center
---

# Questions?

Thank you!
