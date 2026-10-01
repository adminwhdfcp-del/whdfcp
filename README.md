# WHDFCP WEBSITE — MAINTENANCE GUIDE

This repository contains the website for the **Welwyn Hatfield Dementia Friendly Community Partnership (WHDFCP)**.

The site is a simple, accessible, static website hosted through **Cloudflare Pages** and maintained through **GitHub**.

## 1. HOW THE WEBSITE WORKS

**GitHub is the master copy of the website.** Changes should be made in this repository and committed to the `main` branch unless the website administrator has instructed otherwise.

Cloudflare Pages is connected to the GitHub repository and publishes the committed files to the live website. There is normally no need to upload files manually to Cloudflare.

After committing a change:

1. Check that the commit completed successfully on GitHub.
2. Allow Cloudflare a few minutes to create the new deployment.
3. Check the live website, preferably on both desktop and mobile.
4. If a change does not appear, check the Cloudflare deployment status before making another edit.

## 2. CURRENT FILE STRUCTURE

The main website files are kept in the repository root:

- `index.html` — Home page
- `events.html` — Events page
- `partners.html` — Partner directory
- `updates.html` — News and information updates
- `styles.css` — Shared website styling
- `README.md` — These maintenance instructions

Images and logos are stored in the `images` folder rather than alongside the HTML files.

Current image organisation includes:

- `images/events/` — Event posters, event images and event maps
- `images/logos/` — WHDFCP logos and general site branding
- `images/logos/partners/` — Partner organisation logos
- `images/group-photo-1.jpg` and `images/group-photo-2.jpg` — Existing general/community photographs

Keep new images in the appropriate folder. Do not put new images in the repository root unless there is a specific reason.

## 3. FILE AND IMAGE NAMING

Use simple, descriptive filenames. Prefer:

- lowercase letters
- hyphens or underscores consistently
- no unnecessary spaces
- descriptive names rather than names such as `image1.jpg` or `final-final.png`

For example:

- `cyber-fraud-aware.jpg`
- `carol_service_2026.png`
- `carol_service_map_2026.png`
- `alzheimers-society.png`

**File and folder names are case-sensitive.** The path in the HTML must exactly match the path and filename in GitHub.

Avoid keeping multiple copies of the same image with names such as `logo-new.png`, `logo-final.png` and `logo-final-2.png`. If an existing image is suitable, reuse it.

## 4. MAKING A GENERAL WEBSITE UPDATE

1. Open the GitHub repository.
2. Find the HTML, CSS or image file that needs changing.
3. Edit the file directly on GitHub, or upload a new image into the appropriate `images` subfolder.
4. Check spelling, links, image paths and formatting carefully.
5. Commit the change to `main` unless instructed otherwise.
6. Wait for the Cloudflare deployment.
7. Check the live page on desktop and mobile.

Use a short, useful commit message, for example:

- `Update events page`
- `Add new partner`
- `Add Carol Service poster`
- `Correct contact details`

If you are unsure about a change, do not commit it until it has been checked.

## 5. UPDATING THE EVENTS PAGE

The Events page is designed for people who may not be very confident using websites. Keep the information simple, clear and easy to scan.

### Upcoming events

Upcoming events appear under **Upcoming events** and are presented as large event cards.

On desktop:

- the event title and date appear across the top of the card
- the event image/poster appears on the left side
- the event information appears on the right side
- the layout changes to a single column on smaller screens

Do not redesign an individual event card unless there is a good reason. Keep the established layout consistent between events.

### Information to include

Where the information is available, include:

- event name
- date
- time
- venue/location
- short description
- booking information
- parking information
- contact information
- relevant programme or timetable
- organiser or partner information
- links to further information

Put the most important information first. Avoid long blocks of text when the same information can be presented as short labelled sections.

### Event images

If a suitable poster or event image is supplied:

1. Save it in `images/events/`.
2. Use a descriptive filename.
3. Add it to the event card using the correct relative path, for example:

`images/events/carol_service_2026.png`

4. Add meaningful `alt` text describing what the image contains and, where useful, identifying the event/date/venue.

Do not use a large poster as a background image where important information would become inaccessible. The image should be a normal image element with useful alternative text.

### Maps and parking information

If a separate map or parking image is supplied, keep it in `images/events/` and provide a clear link from the event card, for example **View map & parking information**.

The map should not normally be the main event image. The main event poster should be used where it is more attractive and useful for recognising the event.

### Adding a new upcoming event

When adding an event:

1. Open `events.html`.
2. Copy the structure of an existing upcoming event card rather than creating a completely different design.
3. Replace the title, date, image, description and details with the new event information.
4. Add any supplied poster to `images/events/`.
5. Check every image path and external link.
6. Make sure the event appears in chronological order with the other upcoming events.
7. Check the result on desktop and mobile after deployment.

Do not invent missing event details. If a time, booking arrangement or other detail has not been confirmed, say so clearly, for example **time to be confirmed**.

### Moving an event to past events

When an event has passed, move it from **Upcoming events** to **Past events**. Do not leave an old event in the upcoming section.

Past events use a more compact layout because visitors generally need less practical information once the event has taken place.

## 6. PARTNERS PAGE

The Partners page is a searchable, filterable partner directory.

Current features include:

- alphabetical ordering of partners
- search by organisation name and relevant text
- category filters
- expandable bios
- a **Read more** control only when the bio needs more than the initial visible amount
- partner website links where available

When adding or editing a partner:

1. Keep the partner list alphabetically ordered. The page's filtering/search behaviour should also preserve alphabetical order.
2. Put the organisation in the most appropriate category.
3. Keep the visible bio concise.
4. Only include a **Read more** control when there is additional bio text to reveal.
5. Add the organisation's logo to `images/logos/partners/` when a suitable logo is available.
6. Use meaningful image `alt` text for logos.
7. Do not invent an official bio, service description or website URL. If supplied information is incomplete, use an appropriately cautious placeholder or ask for the missing information.

## 7. UPDATES PAGE

`updates.html` contains local news, useful information, community projects and partnership updates.

Keep updates concise and useful. Use a clear heading, a short description and a link to the original source where appropriate.

External links should open in a new tab and use `rel="noopener noreferrer"` when they use `target="_blank"`.

## 8. LINKS

Before committing an update, check that:

- internal links such as `events.html` and `partners.html` use the correct filenames
- image paths point to the correct `images` subfolder
- external website addresses are current and correctly typed
- email links use `mailto:` correctly
- links to maps or event information point to files that actually exist in GitHub

When changing or moving an image, update every HTML reference to that image. A moved image will otherwise produce a broken image on the website.

Some external organisations block automated link checking. A failed automated check does not necessarily mean that the organisation's website is broken; if in doubt, open the link in a normal browser.

## 9. ACCESSIBILITY

Accessibility is especially important for this website because it serves people living with dementia, families, carers and a wide community audience.

When editing the site:

- keep the skip link
- preserve keyboard focus styles
- use meaningful image `alt` text
- keep text readable and sufficiently large
- use clear headings and labelled sections
- maintain good contrast
- keep buttons and links visually distinct
- make interactive controls usable with a keyboard
- preserve the responsive mobile layout
- do not rely on colour alone to communicate important information
- keep language straightforward and easy to scan

For filter buttons on the Partners page, preserve the existing `aria-pressed` state behaviour.

For expandable partner bios, preserve the existing `aria-expanded` behaviour.

The main navigation uses `aria-current="page"` to identify the current page.

## 10. IMAGES AND LOGOS

Use the existing image folders:

`images/events/` — event posters and maps

`images/logos/` — WHDFCP/general branding

`images/logos/partners/` — partner logos

Do not store sensitive information in image files or upload documents containing personal information unless they are genuinely intended for public publication.

For partner logos, use one consistent logo file per organisation where practical. Avoid accumulating duplicate versions of the same logo.

## 11. CLOUDFLARE AND DEPLOYMENT

The website is published through Cloudflare Pages from the GitHub repository.

After a GitHub commit, Cloudflare should normally create a new deployment. If the deployment remains stuck at **Initializing** for an unusually long time, check the Cloudflare deployment logs rather than repeatedly committing the same change.

Do not manually upload the website as a separate copy to Cloudflare unless the website administrator has specifically decided to change the deployment method.

## 12. SECURITY AND ACCESS

The organisation should control access to:

- the GitHub repository
- the Cloudflare account
- the website domain

Avoid making a volunteer's personal account the sole point of access.

**Never commit passwords, API keys, Cloudflare tokens, private keys or other secrets to this repository.** If a secret is accidentally exposed, revoke/rotate it rather than simply deleting it from the current files.

## 13. BEFORE FINISHING AN UPDATE — CHECKLIST

Before committing:

- [ ] Correct file edited
- [ ] Spelling and dates checked
- [ ] Image paths checked
- [ ] External links checked where practical
- [ ] No personal or confidential information accidentally added
- [ ] Accessibility features preserved
- [ ] Mobile layout considered
- [ ] Event is in the correct Upcoming/Past section
- [ ] Partner remains alphabetically sortable
- [ ] Commit message clearly describes the change

After committing:

- [ ] GitHub commit completed successfully
- [ ] Cloudflare deployment completed
- [ ] Live page checked
- [ ] Desktop layout checked
- [ ] Mobile layout checked
- [ ] New images load correctly
- [ ] Important links work

## 14. CURRENT DESIGN PRINCIPLES

The website should remain:

- simple rather than technically complicated
- welcoming rather than corporate
- easy to navigate for people with limited digital confidence
- readable at larger text sizes
- accessible on phones, tablets and desktop computers
- consistent between pages
- easy for future volunteers to maintain through GitHub

When making a design decision, prioritise **clarity, accessibility and ease of use** over adding unnecessary interactive features.
