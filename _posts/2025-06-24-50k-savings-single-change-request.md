---
title: "How I Saved $50K+ on a Government Change Request by Asking One Question"
description: "A simple, pragmatic solution that avoided 400+ hours of work and saved $50,000."
date: 2025-06-24
author: Jesse Schauer
tags: [government IT, legacy systems, cost savings, SPACES, public sector tech, database views, case study]
layout: single
excerpt: "One question. One database view. $50K+ saved. Sometimes that’s all it takes."
image: /assets/images/50k_change_preview.png
head_scripts:
  - custom-og-image.html
---

<!-- TEMP: force Open Graph image -->
<meta property="og:image" content="https://www.jesseschauer.com/assets/images/50k_change_preview.png">

In 2020, I sat in a design review meeting for a proposed new module in **SPACES** — North Dakota’s public benefits management system.

If you’ve worked in government IT with benefits management, you probably know SPACES — or at least a variation of it. The name itself is a North Dakota-specific acronym coined during the benefits modernization effort. Under the hood, it’s a heavily customized case management system originally developed by a major consulting firm nearly 20 years ago and later adapted and implemented under different names in other states. It’s often jokingly referred to as:

> *“The 20-year-old system that replaces 40-year-old systems.”*

With that kind of legacy comes layers of process, paperwork, and tightly coupled architecture. Which is why the proposed change request on the table was so familiar — and so expensive.

---

## The Original Plan: Full Module Buildout

The ask seemed simple: a handful of users at the Department of Health and Human Services (DHHS) needed to **securely view and export a specific subset of data**.

The solution presented?

- A new **module** with multiple screens  
- Custom **security groups** and role-based access control  
- Built-in **reporting and export functionality**  
- Full design, development, testing, and documentation cycles

On paper, it made sense. But the real cost was already snowballing. Between development, multiple rounds of SIT/UAT testing, and security provisioning across environments, this was shaping up to be **a 400+ hour effort** — easily **$50,000 to $70,000** in initial vendor and internal costs.

---

## The Turning Point: Just Listen

I was brought in to review the proposed design and provide the technical approach and estimates. While the team walked through their documents, a casual comment from the stakeholders stopped me in my tracks:

> *“We currently just run queries in our viewer tool and export the data to Excel.”*

So I asked a simple question:  
**“Why don’t we just continue doing that — but with a secured, predefined view in the SPACES database?”**

You could hear the pause.

Not because it was a wild idea — but because no one had considered it.

---

## The Lazy Solution That Worked

I’m not being modest when I say: I’m lazy.  
**The good kind of lazy — the kind that looks for outcomes, not process for process’ sake.**

Instead of writing a single line of Java, I:

- Created a **predefined SQL view** scoped to the exact data they needed  
- Configured **read-only access** for authorized users  
- Documented how to connect to the database securely using their existing tools

That’s it.  
**No new modules. No new screens. No added maintenance.**

The users got exactly what they needed. It took only a couple of hours of actual work — plus the usual herding of cats to get access and approvals.

---

## The Real Savings: Time, Cost, Complexity

By choosing a lean solution that fit the real use case, we avoided:

- Hundreds of hours in **design, development, and testing**  
- Time-consuming **security role design and approvals**  
- Dozens of pages of **documentation and test script authoring**  
- Ongoing **maintenance debt**

The result?  
A working, secure solution delivered in **1/400th** of the estimated time.  
At standard government contracting rates, that’s **$50,000+ in cost avoidance** — for a feature that was already being done manually.

---

## Lessons for Public Sector Tech

This story isn’t about being clever. It’s about asking the right question at the right time — and having enough technical context to offer a better path.

> Legacy modernization doesn’t always mean “rewrite it.”  
> Sometimes it means **don’t write it at all**.

When we stop treating every request as a dev project, and instead look at the system as a whole, we uncover opportunities for massive savings — in time, money, and stress.

I’ll always advocate for code when it’s needed.  
But I’ll also keep speaking up when it’s not.

---

## Wrapping Up

This isn’t the only time I’ve helped state agencies and enterprise teams save tens of thousands — even hundreds of thousands — by questioning the default build-it instinct or status quo. But it’s one of my favorite examples because the fix was so simple — and the ripple effects so big.

**One question. One database view. $50K+ saved.**  
Sometimes that’s all it takes.

---

*Want more behind-the-scenes insights on government IT, pragmatic legacy modernization, and automation that actually works?*  
👉 Visit [JesseSchauer.com](https://www.jesseschauer.com) or connect with me on [LinkedIn](https://linkedin.com/in/jesse-schauer).
