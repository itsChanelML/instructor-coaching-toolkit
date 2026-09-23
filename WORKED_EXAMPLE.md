# Worked Example — Stage 3 Observation

A filled-out rubric and feedback writeup for a fictional candidate,
**Jordan Lee**, delivering
[Build Your First Tool-Calling Agent with Claude](https://github.com/itsChanelML/engineer-agent-adoption-workshop)
solo, observed, per Stage 3 of `TRAIN_THE_TRAINER_PROGRAM.md`. This is a
constructed example — no real session — built to show the rubric and
feedback template actually applied to this specific workshop's actual
failure modes, not a generic one.

---

## Session context

- **Session:** Build Your First Tool-Calling Agent with Claude
- **Format:** 90 minutes, 16 participants, in-person
- **Stage:** 3 (solo teach, observed) — candidate's first full solo delivery
- **Observer role:** silent observation only, per Stage 3 rules

---

## Rubric scores

| # | Dimension | Score |
|---|---|---|
| 1 | Technical accuracy | Solid |
| 2 | Pacing & time management | **Developing** |
| 3 | Clarity of explanation | Solid |
| 4 | Checking for understanding | Solid |
| 5 | Hands-on lab facilitation | **Developing** |
| 6 | Handling questions | Exemplary |
| 7 | Engagement & energy | Solid |
| 8 | Inclusivity & accessibility | Solid |

**Decision: not yet certified.** Six of eight at Solid or better, but two
Developing scores share one root cause (see below) — per the program's
certification bar, this earns one more targeted solo session rather than a
pass with a footnote.

---

## What actually happened (the shared root cause)

Step 2 is where `FACILITATOR_GUIDE.md` already flags the highest-risk
mistake: forgetting to append Claude's response to `messages` before
checking for tool_use blocks, which makes the loop look like it's "stuck"
repeating the same call. Jordan knew this was the likely failure mode — it
came up in their Stage 1 shadow notes — but during the live session, three
participants hit it within two minutes of each other, and Jordan
diagnosed each one from scratch at each desk rather than recognizing the
pattern after the first and addressing the room.

That cost about eight minutes of Step 2's twenty-minute budget, which is
what drove the Pacing score, and it's the same underlying gap — not
proactively watching for a known failure pattern across the whole room —
that drove the Lab Facilitation score. One cause, two rubric lines. That's
worth naming explicitly in the feedback: this isn't two things to fix, it's
one thing.

---

## Feedback delivered (SBI)

**A strength, so it's repeatable:**
```
SITUATION:   A participant asked, during Step 4, whether an ESCALATE
             could ever be "wrong" — i.e., whether the tool itself
             might have a bug rather than the data.
BEHAVIOR:    You said "that's a great edge case — the rubric here is
             'can retrying fix it,' and a tool bug technically means
             no, so it's still ESCALATE-shaped even though the room's
             intuition says 'attribution matters.' Let's sit with that
             tension for a second" — and let the room actually discuss
             it for a minute before moving on.
IMPACT:      You didn't just answer the question, you used it to
             sharpen the distinction the whole step is built around,
             and the room was visibly more engaged in the discussion
             that followed than at any other point in the session.
SUGGESTION:  Keep doing exactly this — you're already flagging good
             tangents in real time and using them instead of deflecting
             them. No change needed here.
```

**The gap, written as one fixable thing:**
```
SITUATION:   Step 2, roughly minutes 6–14.
BEHAVIOR:    Three participants independently hit the "loop looks
             stuck" symptom from a missing messages.append call. You
             diagnosed each one individually at their desk, re-deriving
             the same explanation each time.
IMPACT:      Step 2 ran 8 minutes over budget, which compressed Step 4's
             time later in the session, and two other participants who
             likely had the same bug never got seen because you were
             heads-down with the first three.
SUGGESTION:  The first time you see this specific symptom, say it to
             the whole room once ("if your loop looks stuck repeating
             the same call, check whether messages is actually
             growing — most of you will find the fix in ten seconds")
             before going desk to desk. You already know this failure
             mode cold — the fix is surfacing it to the room the
             moment you see it once, not after the third time.
```

---

## Next step

One more Stage 3 solo session, focused specifically on Step 2. Nothing else
needs re-observing — dimensions 1, 3, 4, 6, 7, and 8 are already at the
certification bar and don't need to be re-proven. Per
`FEEDBACK_TEMPLATE.md`'s "one suggestion per weak dimension," Jordan leaves
this session with exactly one thing to change, not a rubric printout.
