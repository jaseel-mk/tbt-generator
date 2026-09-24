# TBT Generator

## Open

Double-click **TBT Generator.html** and open it in Microsoft Edge or Google Chrome. Keep this file in a stable folder. It is self-contained, works offline, and requires no installation or login.

## Prepare a daily record

1. Choose `0-HIA#143972 HIA`, `0-HIA#143973 HIA`, or `0-DIA#143919 DIA`.
2. Check the date/time (taken from your computer) and select or type a toolbox message.
3. Tick the relevant tasks. Expand each selected task to review/edit its hazards, controls and responsibility, Controls in place defaults to **Yes**; change it when needed. Selecting a task keeps its details collapsed.
4. Enter the conductor and select attendees. Use **Add attendee** for new names. Include the conductor in the attendee list if they will sign. Up to 19 attendees are supported; bottom blank rows are removed only when needed to fit the discussion content.
5. Enter observations and review **Action required?**, which defaults to **No**. If any controls are marked No, record the required action.
6. Click **Update PDF preview**, review every page, and click **Download PDF**. The preview draws the actual PDF pages directly, without a browser PDF plug-in.
7. Enter signature initials beside each attendee's name, or use **Add signature** to upload a PNG/JPG image (up to 3 MB, preferably cropped closely). Signature images are resized and saved in this browser for future TBTs and included in exported backups. **Change signature** replaces an image; **Remove image** returns to the initials. An uploaded image takes priority over initials. Jaseel M starts with `JM`; edit it as needed. Other initials start blank. Entered initials are printed in the signature cells; leave them blank for handwritten signing. Typed initials and signature images are not certificate-based digital signatures.

The filename uses `TBT <permit number> DDMMYYYY HHMM.pdf`, for example `TBT 0-HIA#143972 25092026 1520.pdf`. Time is 24-hour. The filename uses `1520`; the PDF uses `15:20`. Your browser controls the save folder; use its download settings if you want a fixed folder or to be asked where to save each file. The generator does not attach the PDF to a permit system automatically.

## Reuse and backup

- **New daily TBT** clears daily entries and selections, and defaults controls to Yes and action required to No while retaining saved task wording, names, signature initials, signature images and messages.
- **Copy previous downloaded TBT**, under **Saved lists and backups**, copies the last downloaded record's tasks and message. It resets the date/time to now and clears attendees, conductor, observations for fresh review. Controls default to Yes and action required to No.
- Task wording edits are saved automatically. Use **Save message to list** to keep a new toolbox message.
- **Export backup** saves your lists, current draft and previous downloaded record as JSON. **Import backup** restores them after confirmation.
- Browser storage is local to that browser/device and may be cleared by private mode, browser cleanup or moving the HTML file. Export backups regularly. PDFs already downloaded are separate files.

## Format and limits

- The first page uses your original PDF template, retaining its logo, QR code, printed instructions and column structure. The discussion table ends at its last content row. Blank attendance rows are retained where they fit, up to the original 19 spaces; only the bottom rows needed to fit the content are removed. Old entries are removed. New task row separators are added for readability, and the footer uses the TBT date/time and current page count.
- Each template retains its supplied permit number: `0-HIA#143972`, `0-HIA#143973` or `0-DIA#143919`. Changing the TBT selection changes the permit. Renewed permits with different numbers/QR codes require updated source templates.
- The supplied DIA template also says Hamad International Airport; this heading is retained.
- All tasks stay in one discussion table on one page. The approved 11-task list fits with three attendees at the default wording. Text is fitted between 8 and 9 points; unused attendance rows provide extra space. If the content cannot fit legibly, the generator asks you to shorten the descriptions or select fewer tasks.
- Long messages, attendee names or observations that cannot fit are rejected with an explanation rather than clipped. Shorten the text and generate again. No task content is silently removed and no continuation page is generated.
- This version supports English/Latin text. Unsupported characters are reported instead of silently removed.
- Responsibility roles are starting values; assign the actual responsible people and verify the content for the day's work.

## Verification

PDF generation was checked for all three permits, all 11 tasks with three attendees, three tasks with 19 attendees, signature initials, and oversized input. Generated pages were visually inspected. The PDF.js preview renderer was also checked on all three permits, including the compact one-page layout. Interactive browser testing was unavailable because the app's browser security policy blocked local-file navigation.

## Included software

PDF creation uses pdf-lib 1.x (MIT license). The preview uses Mozilla PDF.js with bundled fonts; the libraries and their license notices are embedded in the HTML. The original PDFs and all data stay on the device; no external network services are used.
