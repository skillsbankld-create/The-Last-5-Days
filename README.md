# The Last 5 Days – online (Activity 1 + 1.1)

A single-page web app for **Activity 1 (The Last 5 Days)** and **Activity 1.1 (The Performance Aftermath)**.
One `index.html` file, no build step, no libraries. It runs on **GitHub Pages**.

## Publish it on GitHub (5 minutes)
1. On github.com create a **new public repository**, for example `last5days`.
2. **Add file → Upload files**: drag in **`index.html`** (and `.nojekyll`), then **Commit changes**.
3. **Settings → Pages**: *Deploy from a branch*, branch **main**, folder **/(root)**, **Save**.
4. After 1–2 minutes the site is at `https://YOUR-USERNAME.github.io/last5days/`.
   (Pages on a private repository needs a paid plan, so keep the repository public.)

To change anything later, upload a new `index.html` to the same repository.

## Facilitator access
Open the site → **Facilitator** → enter the code **2026**. The same code opens **Compare (1.1)**.
(To use another code, open `index.html` in a text editor and change `const FAC_PIN = "2026";`.)
This keeps casual visitors out; it is not strong security, because the code is inside the page file.

## Run a session
1. **Setup and group link**: a random **session code** is created for you (press *New session code* for every session). Copy the **group link** and send it to the groups.
2. Groups open the link, pick their **group number** and press **Join**. A green dot appears next to their group in your console. While they wait, each group reads the **case briefing**: "Your sales team is at 82% of the quarterly target. There are only 5 working days left…", the team (2 Top, 2 Core, 2 Struggling Performers) and its three scores right now: **Target 82%, Team Capacity 75%, Team Trust 75%**.
3. Press **Open 5 Days**. Every group screen unlocks by itself and shows the situation and options A–D. The days are written as a countdown: **5 Days, 4 Days, 3 Days, 2 Days, 1 Day**.
4. At 5 Days the group sees the **three scores with the numbers it already knows** from the case. It chooses **one action** and presses **Lock in our choice**, and then sees **only the effect on the Target**, so the team can be pleased with the result. Capacity and Trust stay at their starting numbers on its screen, and **its choice appears in your table by itself** (the cell flashes). You do not type anything.
5. Press **Open 4 Days** when you are ready. Each group first gets a **full-screen "WATCH OUT" alert**: its 5-Days decision did not only change the Target, it also changed **Capacity** and **Trust**, with the exact movement (for example "Capacity decreased by 8 (75% → 67%)", "Trust increased by 3", or "did not change"). The group presses **Got it · show me everything**, and the **Capacity and Trust tiles flip and move** to their real numbers next to the Target. From then on **every effect of every choice is shown straight away** (Target, Capacity and Trust, with arrows ↑ ↓), and the cards show how each number moved since the last day. (You can move the reveal day in Setup.)
6. Continue with 3 Days, 2 Days, 1 Day, then **Final reveal**: everything is visible and **Real Target** (the average of Target, Capacity and Trust) is shown.
7. **Projector view** shows the room only what groups are allowed to see: Target, Capacity and Trust are always there; **Capacity and Trust keep their starting numbers and start to move when you open 4 Days**; Real Target appears at the Final reveal. Switch back to see every number.
8. **Compare (1.1)** is the debrief screen. Groups continue to **Aftermath (1.1)**: a chart of their decisions, WHAT? SO WHAT? NOW WHAT?, and Keep / Stop / Start (one item each).

You can still **edit any cell** in the table. The change is sent to that group's screen.

## Language: English / Arabic
- The top bar has a **العربية / English** button on every screen (including the join and facilitator pages). **Each person switches their own device**; the choice is remembered on that device.
- Arabic is **simplified Modern Standard Arabic** and the page flips to **right-to-left**. The core terms stay in English on purpose: Target, Capacity, Trust, Real Target, WHAT? / SO WHAT? / NOW WHAT? and Keep / Stop / Start.
- In the facilitator console, **Copy Arabic link** gives you the group link with `&lang=ar` at the end, so a group opens straight in Arabic. (Any link can also be opened in Arabic by adding `&lang=ar` to it, or `&lang=en` for English.)
- Everything is translated: the screens, the case and cards, the buttons, the pop-up messages, the trainer notes and the debrief. The only thing that stays in English is the browser tab title until the page loads.

## Game feel
- Each stage opens with a full-screen **countdown splash** ("5 DAYS · left · Pressure Arrives"); the screen then slides in. The 4-Days stage has a warmer splash: "the numbers you could not see are about to move".
- A **progress track** (5 → 1, "days left") fills as the group plays.
- Numbers **count up or down** to their new value and flash green or coral. At 4 Days the hidden tiles **flip open** and the "Watch out" card drops in with a pulse.
- After **Lock in** a "Locked in ✓" stamp appears and the effects pop in one by one. The **Final reveal** shows the four scores in sequence and fills the Real Target bar.
- Facilitator console: a **toast** appears when a group joins or locks a choice, and scoreboard numbers move when they change.
- Devices set to "reduce motion" get no animations or splash, only the content.

## Sound effects
Sound uses short synthesized sounds (no files) and is **on by default on every screen**, including the facilitator console. Browsers only allow sound after the first tap or click on the page, so the first sound plays after that first tap. The **Sound on / Sound off** button in the top bar turns it off for that device and the choice is remembered (press it again to turn it back on).
- **Taps and choices:** a soft click on every button, a different note for options A, B, C and D, a "lock" thud-and-chime when the choice is locked.
- **Countdown:** a whoosh, a boom and **one tick for every day left** when a stage opens (5 ticks for 5 Days, 1 for 1 Day).
- **Warning (4 Days):** a siren with a low rumble, then a "flip" sparkle for each tile that unlocks.
- **Results:** a rising chime for an increase, a falling buzz for a decrease, a neutral note for no change; a glide up or down while numbers count.
- **Final reveal:** a fanfare, a note for each score and a rising sweep as the Real Target fills.
- **Other:** a welcome jingle when joining, a short error buzz for a wrong code, an "unlock" chime for a right one, and a ping on the facilitator console when a group joins or locks.

## How the live connection works
A website on GitHub has no server, so the app sends tiny messages (group number, day, letter) through the **free public relay ntfy.sh**, on a private topic built from your session code. Because of that:
- Use a **new session code for every session** (anyone who knows the code could read or send messages for that session).
- The relay keeps messages for about 12 hours. Reloading a page rebuilds the session from them.
- If a group (or the venue network) is offline, the screen shows **Live sync: offline**. That group can press **Copy** on its code (like `G3-BCA`) and send it to you; paste it in **Paste group codes**. Each day also has a **backup 4-digit code** on your console.
- Please **rehearse once with two phones** before a live session.
- Advanced: you can point the app to your own ntfy server by opening the site with `?relay=https://your-server/` in the link.

## Good to know
- Everything is saved in the browser of the device in use. *Reset session* clears the facilitator side (and creates a new session code); *Leave* clears a group device.
- The hidden effects are part of the page code, so this is a classroom tool, not a secure exam. Group devices only show the group pages.
- You can test the app offline by double-clicking `index.html` (live sync needs internet).

Built for the Skills Bank "People First Leadership for Sales Leaders" programme.
