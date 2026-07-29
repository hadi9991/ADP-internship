# Task 2 — Your First IVR: The Cinema Line 🎬

**Time:** ~1 hour · **Due:** before Day 3 · **Tools:** Call Studio
**Elements allowed:** `Audio`, `Menu`, `Number` — nothing else yet

---

## The idea

Yesterday you listened to real IVRs. Today you build one.

It is small on purpose. The point is not to build something impressive — it is to build something that **never dead-ends**, no matter which key the caller presses.

---

## Before you open Call Studio ✏️

**Draw the flow on paper first.** Every box, every arrow, every option.

Do not skip this. Ten minutes on paper saves an hour of clicking. This is exactly what a designer does on a real project before anything gets built.

---

## What to build

A phone line for a cinema. The caller should be able to hear what is playing, hear the prices, or book tickets.

### The flow

**1. Welcome**
An `Audio` element that greets the caller.

> "Welcome to Nile Cinema."

**2. Main menu**
A `Menu` element with three options:

| Key | Option |
| :-- | :--- |
| `1` | Today's showtimes |
| `2` | Ticket prices |
| `3` | Book tickets |

**3. Option 1 — Showtimes**
An `Audio` element that reads out two or three films and their times, then returns the caller to the main menu.

**4. Option 2 — Prices**
An `Audio` element with the ticket prices, then back to the main menu.

**5. Option 3 — Book tickets**
A `Number` element that asks how many tickets the caller wants.
Then an `Audio` element that confirms the booking, and a goodbye.

**6. Goodbye**
An `Audio` element that thanks the caller and ends the call.

---

## The part that actually matters ⭐

Anyone can build the happy path. Your task is to handle everything else:

- **The caller presses `7`.** What happens? It must not crash and it must not go silent.
- **The caller says nothing at all.** What happens after the silence?
- **The caller gets it wrong three times in a row.** Where do they end up? A caller must never be stuck in a loop forever.
- **The caller finishes listening to the showtimes.** Where do they go next? Never leave a branch hanging.

Write a short "sorry, I didn't get that" prompt and re-play the menu. After three failed attempts, send the caller to the goodbye message.

> A caller should always end up somewhere. If any path in your flow just stops, the task is not finished.

---

## Rules

- ✅ Only `Audio`, `Menu` and `Number`. No other elements yet — you will learn those this week.
- ✅ Every prompt must have text written for it. Use TTS text for now; you will generate real audio files in week 2.
- ✅ Every single path must reach either the main menu or the goodbye.
- ❌ No dead ends. Not one.
- ❌ Do not build the whole cinema. Three menu options is the task.

---

## Test it before you submit

Walk through **every** path yourself, including the wrong ones:

- [ ] Press `1` → showtimes → back to menu
- [ ] Press `2` → prices → back to menu
- [ ] Press `3` → enter a number → confirmation → goodbye
- [ ] Press `7` → error prompt → menu again
- [ ] Press nothing → error prompt → menu again
- [ ] Get it wrong three times → goodbye, not an endless loop

If you have not clicked through all six, you have not tested it.

---

## Stretch goals 🚀

Only if the core flow works and every path is covered:

1. Add a `0` option to the menu that repeats the greeting.
2. Read the number of tickets **back** to the caller in the confirmation — "You have booked 4 tickets." (Look into how an element's captured value can be used in a later prompt.)
3. Add a second `Number` element that captures the caller's mobile number for the booking confirmation.

---

## What to submit

1. **Your paper flow** — a photo of the sketch is fine.
2. **The Call Studio project folder**, zipped.
3. **Three sentences:** what was harder than you expected, and what broke first.

---

## What we are looking for

Not a beautiful IVR. We want to see whether you:

- **thought about the flow before building it** — the sketch tells us this
- **covered every branch**, including the ones a caller reaches by mistake
- **never left a caller stranded** in silence or in a loop

That is the entire skill. Everything else this month is detail on top of it.
