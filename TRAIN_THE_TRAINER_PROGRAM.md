# Train-the-Trainer Program

How a subject-matter expert becomes a certified instructor for a given
session — using
[Build Your First Tool-Calling Agent with Claude](https://github.com/itsChanelML/engineer-agent-adoption-workshop)
as the running example throughout. Four stages, each with a clear exit
condition — nobody advances on a calendar date, only on the rubric.

## Why a pipeline instead of "read the deck and go"

A facilitator guide tells you what *should* happen. It does not tell you
whether a specific person can *make* it happen in front of a room that
isn't cooperating — the SME who wrote a workshop is not automatically the
best person to deliver it live, and the reverse is also true. This pipeline
exists to find that out before a real cohort is the one who discovers it.

## Stage 1 — Shadow (1–2 sessions)

The candidate observes a certified instructor teach the full session,
**using `OBSERVATION_RUBRIC.md` themselves** — not just watching, but
practicing the act of observing. This does two things at once: it's their
first real exposure to the material being taught live (not just read), and
it's low-stakes practice with the rubric's vocabulary before they're the one
being scored against it.

*Exit condition:* the candidate can point to a specific moment in the
session and describe it in SBI shape, unprompted.

## Stage 2 — Co-teach (1 session)

The candidate delivers one or two modules solo — for this workshop,
typically Step 1 and Step 3, the two steps with the least live-troubleshooting
surface area — while the certified instructor runs the rest and floats
during the candidate's modules to catch anything that goes sideways.

The certified instructor fills out the rubric **only for the modules the
candidate delivered**, not the whole session.

*Exit condition:* Solid or better on dimensions 3 (clarity), 4 (checking
understanding), and 7 (engagement) for their modules. Dimensions 2
(pacing) and 5 (lab facilitation) are allowed to still be Developing here —
those are the two the next stage exists to build, since a two-module slice
doesn't exercise them under real pressure.

## Stage 3 — Solo teach, observed (1–2 sessions)

The candidate runs the entire session. The certified instructor observes
silently — no floating, no rescuing a stuck learner unless something is
actually at risk — and fills out the full rubric plus SBI feedback per
`FEEDBACK_TEMPLATE.md`.

This is the stage that surfaces pacing and lab-facilitation gaps that
smaller slices can't: whether Step 2's time budget survives contact with a
room that's slower than expected, whether the candidate notices four silent
stuck people instead of only the two who raised their hands.

*Exit condition:* see the certification bar below.

## Certification decision

**Solid or better on all eight dimensions, across at least two solo-observed
sessions.** Two, not one, because a single good session is as likely to be a
cooperative room as a repeatable skill — the bar is "this instructor
performs this way regardless of the room," and one data point can't
establish that.

A candidate who is Solid on seven dimensions and Developing on one does not
get certified with a footnote — they get one more targeted solo session
aimed specifically at that dimension, using the single-suggestion approach
in `FEEDBACK_TEMPLATE.md`. See `WORKED_EXAMPLE.md` for exactly this
situation, played out in full.

## Stage 4 — Ongoing calibration

Certification is not permanent by default. Two things keep it real over
time:

- **Re-observation on a cadence** (quarterly is reasonable for a
  frequently-taught session), not just at onboarding — skills drift, and so
  does the material itself as it's revised.
- **Coach calibration sessions**, where two or more certified coaches
  observe the *same* recorded session independently and compare rubric
  scores before comparing notes. Divergence here means the rubric — or the
  coaches' shared understanding of it — needs tightening, not that one coach
  is wrong. This is what keeps "Solid" meaning the same thing across every
  coach on the team as the program scales past one person doing all the
  observing.
