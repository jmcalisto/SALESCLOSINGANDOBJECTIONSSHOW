# Jack's Solution & Close — Solution, Closing & Objections (Show)

A single self-contained HTML training activity (the "Solution, Closing & Objections — Show
section" comic) for Wall Street English sales training. No build step, no dependencies beyond
Google Fonts — open `show_jack_solution_close.html` directly in a browser to preview or deliver
it.

## What it is

A narrated, comic-book-style playback of a complete solution-and-close conversation between the
consultant and Jack (a prospective student). The learner reads it panel by panel — tapping
"Next" to advance — while "Notice how…" chips call out the technique behind each line: the
partial close, the two options, the calm price and the silence that follows it, the guarantee,
the alternative close, the Three Magic Steps used on Jack's price objection, and finally the
buying signal. It ends with a recap of the techniques demonstrated.

It is the demonstration counterpart to the learner-driven role-play in the
`SALESCLOSINGANDOBJECTIONSDO` repo — same seven phases, same techniques, shown rather than
practiced.

## Localization

Everything a learner sees lives in two JavaScript objects near the top of the `<script>` block:

- `UI` — interface strings, the phase labels, and the closing techniques recap
- `SCRIPT` — the dialogue itself, as a flat ordered array of `{phase, who, text, chip}` lines,
  where `chip` is the optional "Notice how…" callout attached to that line

To produce a new language version, translate the string values in these two objects and re-host
the file. Nothing else needs to change. Lines also support an optional audio hook for a
per-language voice clip; leaving it unwired keeps the activity text-only.

## Design system

This activity follows the comic/narrative "Show section" visual style used across Wall Street
English sales training activities — distinct from the multiple-choice "Do section" style. See
the companion style-guide repo for the full design tokens, component inventory, and a blank
template for building new activities in the same comic style.
