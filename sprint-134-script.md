# Sprint 134 Recap — Presentation Script
**Sprint 134 | March 30 – April 10, 2026**
Target time: ~20 minutes presentation + 10 minutes discussion

---

## Slide 1 — Sprint Headline (2 min)

"Alright everyone, Sprint 134 is in the books. Let me walk you through how we did.

268 items this sprint — that's actually down from 302 in Sprint 133. We completed 205 of those, landing at 76.5% item completion. Now that's lower than last sprint's 84%, and I'll explain why in a moment, but here's the important number — our task-hour burn rate was 83.9%. That's nearly identical to Sprint 133's 83.4%. So the team's execution efficiency held steady — we just had a different mix of work this sprint.

On the strengths side — EventFlow Segmentation is done. Thomas delivered all 8 phases. Six team members hit 100% completion. And our bug ratio improved significantly, down from 69% to 52%.

The concern — and I'll dig into this — is Legacy AX. It jumped from 4% of last sprint to 19% of this sprint, and it's only at 33% completion. That's what's pulling our overall numbers down."

---

## Slide 2 — S133 vs S134 Comparison (2 min)

"Let me put the two sprints side by side so you can see the full picture.

Items dropped 11% — 302 to 268. Completion fell from 84.1% to 76.5%. That looks like a step back. But look at the hours — we estimated 785 hours of task work and burned 659 of it. That's 83.9%, almost exactly matching last sprint's 83.4%.

What that tells us is the items that were in scope got executed well. The completion gap is almost entirely explained by the Legacy AX surge — 51 items came in at only 33% done.

The good news on the quality front — bug ratio dropped from 69.2% to 52.1%. We spent more time on features relative to bugs than we did last sprint."

---

## Slide 3 — What Shipped (3 min)

"Let's talk about what actually got delivered. A lot of big things landed this sprint.

The headline is **EventFlow Segmentation** — Thomas Holland completed the entire initiative. Phases 1 through 8. Service bus topic segregation, channel tier routing, dispatcher restructure, DLQ retry updates. This was a massive body of work done by one person in one sprint — 16 PBIs, all complete.

**Joshua Hise** had a breakout sprint on M365 Forms — he shipped Tab Sets across BFF, FE, and MCore. Product Detail Message Center across BFF, FE, and MCore. SSO Maintenance BFF and MCore. That's 10 PBIs in a single sprint spanning the full stack.

**Dariusz** completed the Dapr service-invocation API replacement — this was a multi-sprint effort that's now done. He also shipped Global Change Request History and the ADO baseline cleanup.

**Marcin** landed the .NET 10 SDK upgrade kickoff and Entity Change Request Scope Set on the frontend side.

On the infrastructure side — **Grzegorz** finished the Scheduled Cleanup Job Plan with Quartz.NET and Cosmos DB. **Kamil** completed the Preview Environment Activation Redirect and the Right-side Panel feature. **Clint** shipped the report generation API.

And **Tymoteusz** continued the Landing Page Builder stabilization — 12 more bugs fixed including field size, checkbox ordering, dropdown behavior, and folder management."

---

## Slide 4 — Ready for Testing (1 min)

"Five items ended the sprint in review or testing states — these are the ones that need QA attention going into Sprint 135.

The big one is Clint's **DeliveryConfirmation generator** — that's the first real NotificationType for the Notification System. It's sitting in PR Waiting Approval. Once that's merged, it unlocks the AX2009 trigger point work.

The other four are all AX Dev Items — Sandra Brodowski has two in AXDev Testing, Lindsay has one, and Thomas has one that's already Testing Approved.

Overall the testing backlog is light — which is a good sign. Most of what got developed also cleared review within the sprint."

---

## Slide 5 — Incomplete Work & Impact (2 min)

"Now let's talk about what didn't finish and what it means.

**High impact items** — there are five. Justin Barreira's OneSource Tax Middleware API is still in New state. This has been flagged for three sprints now. The .NET 10 SDK upgrade and Dapr API replacement are both In Progress with Jacek — those are multi-sprint platform initiatives that are tracking. Clint's DeliveryConfirmation is in PR — close to done. And there's an unassigned Landed Cost consolidation feature.

**Medium impact** — nine items. A mix of AX Dev work in Coding or Testing states, some forms bugs, and Joshua's SSO Maintenance FE piece.

**Low impact** — these are mostly New items that weren't started, or items that were Removed.

The timeline impact: OneSource is the one I'd flag. It's been sitting for multiple sprints and if it's a priority, it needs dedicated focus in Sprint 135. The .NET 10 and Dapr work are progressing normally — those are expected to be multi-sprint."

---

## Slide 6 — Mid-Sprint Discovery (1.5 min)

"Scope creep — and I want to be precise here because we've refined how we measure this. The adjusted number is 13.8% — that's 37 items added after the sprint started, counting only PBIs and Bugs, not task decomposition.

Of those 37, 19 were PBIs and 18 were bugs. But here's the context — 16 of those 19 PBIs were Thomas's EventFlow Segmentation phases. That was planned work being broken down into trackable items on day one, not unplanned scope.

The 18 bugs were a mix of Landing Page Builder defects found by Tymoteusz and Marcin, plus a handful of EventFlow and deployment issues. That's typical discovery during active development.

So the real unplanned additions are roughly the 18 bugs — about 6.7% of the sprint. That's healthy."

---

## Slide 7 — Work Categories (2 min)

"This is the slide I want everyone to pay attention to because it tells the investment story.

By item count, Platform was 60.8% of the sprint. But by task hours, it was 68.2%. Platform hours burned at 94.4% — excellent execution. Business was 20% of items but only 11.8% of hours — business items are smaller, quicker tasks. Business burned at 91.4% — also strong.

The outlier is Legacy AX. It was 19% of items and 20% of hours — a big jump from Sprint 133 where it was only 4%. And it burned at just 43.9%. This is the category dragging overall completion down.

The strategic question remains the same as in the QBR — we're running at roughly a 6:1 platform-to-business hour ratio this sprint. That's by design right now with the infrastructure investments, but it's worth keeping in mind as we plan next quarter."

---

## Slide 8 — Team A Performance (2 min)

"Team A.

**Thomas Holland** — 45 out of 45. 108 hours out of 108. Perfect sprint. The EventFlow Segmentation delivery was the standout achievement of this sprint. He also fixed 4 bugs and shipped the Archive Plans feature. Two consecutive sprints of elite output.

**Joshua Hise** — 32 out of 34, 94%. This was a breakout sprint for Joshua. He shipped 10 PBIs across the full BFF/FE/MCore stack — Tab Sets, Message Center, SSO Maintenance. Plus 6 bug fixes. Up from 20 items last sprint. Big step up.

**Clint Wilkes** — 10 out of 15, 67% by items but 93% by hours. The hours tell the better story here — most of his estimated work got done. The incomplete items are the DeliveryConfirmation PR and AX2009-related work.

**Justin Barreira** — 7 out of 16, 44% items, 73% hours. He's the lowest on the team. The OneSource initiative isn't progressing — the Middleware API PBI and 5 AX Dev Items are still New. We need to discuss whether OneSource has the right priority or if there are blockers we're not seeing."

---

## Slide 9 — Team B Performance (2 min)

"Team B had four members hit 100% this sprint.

**Adam Wojciechowski** — 6/6, 37 hours, perfect. Scope Sync pipeline fix, JSON converters, SmallDateTime handling. Clean delivery.

**Dariusz Uchman** — 8/8, 76 hours, perfect. Dapr replacement done, Global Change Request History, ADO cleanup. Consistently one of our most reliable executors.

**Grzegorz Giera** — 4/4, 5 hours, perfect. Light sprint — just the Quartz.NET cleanup job plan. Down from 52 hours last sprint.

**Marcin Miazga** — 10/10, 67 hours, perfect. .NET 10 SDK upgrade, Entity Change Request Scope Set FE, Dynamic Lookup bug fix, and 2 Landing Page Builder bugs. Back to 100% after a strong S133 as well.

**Jacek Smigiel** — 15/19, 88% hours. Preview Feature Registry AppName, Scope Check via OrgMgmt, Terraform pipeline fix. The incomplete items are the .NET 10 upgrade and Dapr replacement — both multi-sprint initiatives that are progressing.

**Mateusz Janiszewski** — 2/2, but only 1 hour estimated. That's a dramatic drop from last sprint's 40 hours. We should check if this was intentional reallocation or if something else is going on."

---

## Slide 10 — Shared Members (1 min)

"Shared members.

**Tymoteusz Tracz** — 34/36, 90% hours. He's our Landing Page Builder workhorse — 12 bugs fixed this sprint on top of EventFlow BatchJobs UI work. Consistently strong contributor.

**Kamil Trescinski** — 12/13, 90% hours. Preview Environment Activation Redirect shipped, Right-side Panel shipped, plus 4 bug fixes across Entity Change Requests and Forms. Solid sprint.

**Alec** had no items assigned this sprint."

---

## Slide 11 — Key Findings & Next Sprint (2 min)

"Let me land the key takeaways.

**First — EventFlow Segmentation is complete.** This was the biggest platform initiative this sprint and Thomas delivered it solo. Huge win.

**Second — hour burn held steady.** 83.9% vs 83.4% last sprint. The team maintained execution quality despite a different work mix.

**Third — six members at 100%.** That's strong across both teams.

**Fourth — and this is the flag — Legacy AX is dragging us.** 51 items at 33% completion, 43.9% hour burn. It accounts for almost all of our completion gap versus Sprint 133.

**Fifth — bug ratio improved.** Down 17 points from 69% to 52%. We're spending more time building and less time fixing.

**Sixth — OneSource needs a decision.** It's been flagged for three sprints. Either we commit resources to push it through or we acknowledge it's not a current priority.

**Seventh — Joshua's breakout sprint.** 32 out of 34 items, 10 PBIs shipped across the full stack. Major Forms velocity.

For Sprint 135, our priorities should be:
1. Get DeliveryConfirmation merged and through testing
2. Make a call on OneSource — focus or defer
3. Clear the Legacy AX testing backlog with Sandra
4. Continue Landing Page Builder stabilization
5. Deploy EventFlow Segmentation to all environments
6. Continue the .NET 10 SDK upgrade

That's Sprint 134. Questions?"

---

## Discussion Prompts (if needed)

- "Justin — can you walk us through what's blocking OneSource? Is it priority or complexity?"
- "Mateusz — your load dropped from 40h to 1h this sprint. Was that planned?"
- "For the Legacy AX work — are we expecting this volume to continue in Sprint 135 or was this a one-time spike?"
- "Thomas — now that Segmentation is done, what's the plan for EventFlow in 135? Cross-training?"
- "Clint — what's needed to get the DeliveryConfirmation PR approved? Who's reviewing?"
