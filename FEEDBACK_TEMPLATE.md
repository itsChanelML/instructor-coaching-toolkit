# Feedback Template

Structured as **Situation → Behavior → Impact → Suggestion** (SBI+):
what was happening, what the instructor specifically did, what effect it
had on the room, and one concrete thing to try next time. Every piece of
feedback — praise included — uses this shape. "Great job today" is not
feedback; it's applause. It doesn't tell anyone what to repeat.

## Why this shape

- **Situation** anchors the feedback to a moment, not a vibe — "in the step
  2 walkthrough" beats "sometimes."
- **Behavior** describes what the instructor *did*, observably — not a
  trait ("you rushed") but an action ("you moved to step 3 while four hands
  were still up").
- **Impact** names the effect on the room, not on you as the observer. The
  instructor needs to see the learner-side consequence to want to change it.
- **Suggestion** is one thing, specific enough to do literally next time,
  not a general principle to internalize.

## Template

```
SITUATION:   [When, in the session, did this happen?]
BEHAVIOR:    [What did the instructor specifically say or do?]
IMPACT:      [What effect did this have on the room / on learning?]
SUGGESTION:  [One concrete, repeatable action for next time.]
```

## Worked examples

**A strength, written up so it's repeatable — not just "good job":**
```
SITUATION:   Step 2, right after the first person hit the "loop never
             terminates" bug.
BEHAVIOR:    Instead of debugging it themselves, you asked "what does
             len(messages) do at the top of your loop?" and let the
             participant find it.
IMPACT:      They fixed it themselves in under a minute, and you'd
             clearly used that exact diagnostic question before —
             three other people around them overheard it and used
             the same check on their own code without being asked.
SUGGESTION:  Say that diagnostic question to the whole room proactively
             at the start of step 2 next time, before anyone hits the
             bug — it seems to prevent it as often as it fixes it.
```

**A gap, written up so it's fixable — not a verdict:**
```
SITUATION:   Step 4, introducing RETRY vs ESCALATE.
BEHAVIOR:    You showed the code for both branches back-to-back before
             asking the room which one applies to a hallucinated tool
             name vs a renamed CSV column.
IMPACT:      About a third of the room could recite both branches but
             couldn't say, unprompted, which failure mode each one is
             for — the distinction that's actually the point of the
             exercise.
SUGGESTION:  Ask "whose fault is this failure — the model's or the
             data's?" before showing either branch of code. Land the
             concept, then show the code as the answer, not the setup.
```

## Delivering it live

- Lead with what to keep doing. Not as a softening tactic — because if you
  only ever hand someone corrections, they drift away from things that were
  already working, and you'll have to re-teach those too.
- One suggestion per weak dimension per session, not eight at once. An
  instructor acting on one specific change is worth more than an instructor
  overwhelmed by a complete rubric printout.
- Ask before telling: "what did you notice about the room during step 2?"
  often surfaces the same gap the observer saw — and self-noticed feedback
  sticks better than delivered feedback.
