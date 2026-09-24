# TBT Generator

A browser-based toolbox talk generator for HIA and DIA permit templates. Select a permit, discussion tasks and toolbox message, add the conductor and attendees, then preview and download the PDF.

## Use

Open the published website or download and open `index.html` in Edge or Chrome. The app is self-contained and requires no build step. See [the user guide](USER-GUIDE.md) for instructions; its offline filename refers to this same app.

Saved names, signature initials/images, messages and drafts stay in the current browser. They do not sync between devices. To transfer your existing local app data to the website, use **Export backup** in the old app and **Import backup** on the website. Keep backups regularly.

The public app includes the supplied permit templates, permit numbers, QR codes and starter lists. User-entered records and signatures are stored locally; generated PDFs download to the user's device.

## Hosting

This is a static GitHub Pages site. In repository Settings > Pages, publish from the `main` branch and the root folder. No backend or package installation is required.

## Updating

Replace `index.html` with the updated self-contained generator and commit the change. Embedded third-party library and font notices are retained in that file. Review the generated PDF and task-specific controls before use.
