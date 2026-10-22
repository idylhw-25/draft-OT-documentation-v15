OT Documentation Updated — 22 October 2026

OPEN THE APP
For a single-file app, open OT-documentation-webapp-standalone.html in your browser. Its styles, scripts and icons are embedded; keep this filename when replacing an older standalone copy.

For the hosted/installable app, use index.html with app.js, phraseBank.js, style.css, sw.js, manifest.webmanifest and the icons folder together. Serve the folder over HTTPS or localhost for offline installation. The service-worker cache is version v115. Reload the app after deploying the replacement files.

CHANGES
• Bathing: Stand appears even when no bathing facility is selected.
• Home Help Service includes Exercise with a remarks field wherever the shared Social History form is used.
• Home O2 Assessment includes an editable, copyable Green Box in Summary, linked to Oxygen regime and Treatment plan. It retains the existing 250-character warning and does not truncate the note.
• Emergency Medicine is available in the assessment selector with nine sections based on ADL Initial.
• Emergency Medicine Premorbid Cognitive Function offers Good, Fair, Poor and Unremarkable, with one rating at a time. Others can be selected alongside a rating and opens a free-text remarks box. Saved legacy remarks are preserved. Behavioral Problem has Unremarkable/Yes and conditional details. Saved Nil selections are updated to Unremarkable in the form and Summary.
• AMT and Clock Drawing Test are always displayed in Emergency Medicine, with Not test in the form, Summary and linked cognitive comments. MoCA opens through Done.
• Emergency Medicine AMT retains its item cards and adds direct total-score buttons from 0 to 10. Direct scoring clears individual answers and omits item scores from Summary. Selecting an item returns to item scoring; pending AMT remains pending until all items are answered or a total is selected.
• Emergency Medicine Lawton has a Not test option. Its item controls are hidden and the entire Lawton section is omitted from Summary when selected, including linked IADL comments and remarks. Previously entered scores remain available if Not test is deselected.
• A completed Emergency Medicine Lawton adds IADL: Lawton xx/27 and an IADL remarks box to OT Comment. The linked score and remarks appear in Summary only while Lawton is complete and tested.
• Emergency Medicine Treatment includes the options visible in its Treatment Plan except Further assessment if stable. The ADL trio occupies the first row and the cognitive trio the second row. Home Safety Recommendation is shortened and only one Others option is shown. Relevant remarks and training-program selections appear in Summary. Treatment Plan retains its existing choices.
• Mood supports one primary choice plus Others and free text. Performed opens the 15 GDS questions and automatic scoring.
• GDS question 4 is “你常常感到生活沉悶嗎？”, as confirmed. Question wording, score keys and summary cutoff text otherwise follow the supplied specification.
• Chinese Lawton IADL includes nine items scored 0–3, a total out of 27, optional explanations, and item scores in Summary. NA means not assessed.
• Each GDS and Lawton item occupies its own full-width row. GDS response buttons sit alongside the item on wider screens and below it on smaller screens.
• Lawton follows the MBI card format: item title and a Not assessed / score pill above a full-width row of NA, 0, 1, 2 and 3 buttons. NA is highlighted when no score is recorded; optional item explanations appear below the buttons.
• Unfinished Lawton assessments show “>= xx/27, pending further assessment” in the form and Summary, where xx is the sum of assessed items. Completed assessments show their final score out of 27.
• When GDS is marked Performed, a reminder in the form and Summary asks the therapist to answer all 15 questions. The total score appears only when all questions are answered.
• Unfinished AMT summaries show “AMT: pending”, including linked OT comments and the Green Box. Unfinished summaries omit answered-count and subtotal brackets. Blank answers are not treated as zero.
• In Fall Assessment, Others appears before Functional Balance Assessment. Functional Balance Assessment has its own heading and separate block in Summary when results are entered. The entire Functional Balance section is omitted from Summary when Not applicable is selected.
• Emergency Medicine fall history supports multiple incidents and multiple reasons per incident.
• Fall frequency appears in Summary whenever Yes is selected and a frequency is entered in ADL Initial, Emergency Medicine, Fall Assessment and Palliative Care. The dedicated Fall Assessment summary omission has been fixed.
• Emergency Medicine uses “Continue 1-2 days ward-based training”. Other assessment forms retain their existing recommendation wording.

SAVED CASES
The existing local browser autosave and seven-day retention behavior remain in place. New fields are added when older saved records load. Case data belongs to the browser/site (or local file location); it is not included in these application files. A different browser, website address or local file location may use separate storage.

VERIFICATION
JavaScript syntax checks and 18 automated behavior checks passed, covering every form’s rendering, scoring and text fields, conditional controls, summary output, Home O2 Green Box synchronization and saved-case compatibility. New checks cover direct AMT totals including 0 and 10, switching scoring methods, Not test states, premorbid choices and legacy remarks, conditional Lawton OT comments, omission of untested Lawton from Summary (including after saved-case reload), and expanded Treatment options and details. The fall-frequency check covers all four assessments with fall history, including updates, saved-case reloads, blank entries and No fall history. Browser checks confirmed the premorbid remarks, direct AMT score and omission of subscores, CDT Not test summaries, completed Lawton 9/27 with IADL remarks, the grouped Treatment rows, and Treatment details in Summary, with no browser console errors. The standalone build uses the same scripts and styles as the folder version.
