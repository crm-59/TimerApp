The timer app includes:

	•	Live clock with date and local time
	•	Stopwatch with Start, Stop, Pause/Resume, and Reset
	•	Location detection — tries GPS first, falls back to IP geolocation, with flag display and coordinates
	•	Sleek dark UI with that glassmorphism card style

Countdown mode

	•	Toggle between ⏱ Stopwatch and ⏳ Countdown with the pill switch at the top
	•	Manual H/M/S input fields when in countdown mode
	•	Quick preset buttons: 1hr, 30min, 10min, 5min, 1min, 30sec
	•	Progress bar that drains as time runs out
	•	Last 10 seconds pulse red with a warning animation
	•	A “⏰ Time’s up!” toast notification slides in from the top when it hits zero

Responsive & mobile-friendly

	•	Card stretches to fit the screen width on phones, capped at 480px on desktop
	•	All font sizes scale with clamp() — never too big or too small
	•	Buttons use flex-wrap so they reflow to a second row on very narrow screens
	•	Input fields and separators scale down gracefully on small phones (under 360px)
	•	No horizontal overflow — everything stays within the viewport

🟢 Lap Counter (Stopwatch mode)

	•	A Lap button appears when in Stopwatch mode, enabled only while running
	•	Each lap shows: lap number, split time (with centiseconds), and total elapsed
	•	The fastest lap highlights in green, the slowest in amber
	•	A scrollable list holds as many laps as you need, with a Clear button
	•	Laps animate in smoothly when recorded

⏰ Alarm Sound (Countdown)

	•	Uses the Web Audio API — no external files needed, works completely offline
	•	Plays a two-phrase melodic beep sequence (6 tones) when the countdown hits zero
	•	Pairs with the existing toast notification

🔴 Screen Flash (Countdown)

	•	A red overlay pulses across the entire screen 5 times when time’s up
	•	Works alongside the alarm for a satisfying multi-sensory alert

☀️ / 🌙 Theme Toggle

	•	Button in the top-right corner switches between dark and light mode
	•	Every element — card, inputs, laps, buttons, text — adapts cleanly
	•	Light mode uses a soft blue-grey gradient with proper contrast throughout

What you see in fullscreen:

	•	The timer display scales up massively — up to 18rem on a large screen, readable from across a room
	•	The mode label (Stopwatch / Countdown) shown above the digits
	•	A full-width progress bar for countdown mode
	•	All control buttons reproduced at larger size — Start, Stop, Pause/Resume, Lap, Reset — fully functional
	•	The current date and time shown below the controls so you always have context
	•	Both dark and light themes respected

How to exit:

	•	Click the ✕ Exit button (top-right corner)
	•	Press the Escape key
	•	The browser’s native fullscreen toggle (F11 / green button on Mac) also works and syncs correctly

The fullscreen display stays perfectly in sync with the main view — button states, pause/resume labels, countdown progress, and warning pulses all mirror live. 🖖

