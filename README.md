WHDFCP WEBSITE — MAINTENANCE NOTES

This version of the site is a simple website designed for hosting via Cloudflare Pages.

FILES
- index.html       Home page
- events.html      Events page
- partners.html    Partner directory
- styles.css       Shared styling

LOGO
The main WHDFCP branding uses WHDFCP_Logo_Large.png. Keep this file in place.

# UPDATING THE SITE

The website is maintained through **GitHub** and automatically published through **Cloudflare Pages**.

**GitHub is the master copy of the website.** Do not maintain a separate master copy of the website on an individual's computer.

## Making an update

1. **Log in to the website's GitHub repository.**

   * Open the website repository on GitHub.
   * Make sure you are working in the correct repository before making any changes.

2. **Find the file you need to change.**

   * HTML files contain the website's text, links and page structure.
   * `styles.css` controls the appearance of the website, including fonts, colours, spacing and layout.
   * Images are stored in the `images` folder.

3. **Edit the file directly on GitHub.**

   * Open the file.
   * Click the **Edit** (pencil) button.
   * Make the required changes.
   * Be careful not to change anything else in the file.

4. **Check your changes carefully before saving.**

   * Check spelling and formatting.
   * Make sure links and image file names are correct.
   * **File and folder names are case-sensitive.** For example, `images/photo.jpg`, `images/Photo.jpg`, and `Images/photo.jpg` are all different.

5. **Save the changes to GitHub.**

   * When you are happy with the changes, use GitHub's **Commit changes** option.
   * Add a short description of what you changed, for example:

     * `Update events page`
     * `Add new partner`
     * `Correct contact details`
   * Commit the changes to the main branch unless the website administrator has instructed you otherwise.

6. **Wait for Cloudflare to update the website.**

   * Cloudflare Pages is connected to the GitHub repository.
   * After a change is committed to GitHub, Cloudflare automatically creates a new website deployment.
   * **There is no need to upload anything manually to Cloudflare.**
   * Allow a few minutes for the changes to appear on the live website.

## After making an update

7. **Check the live website.**

   * Open the website's address.
   * Check the page you changed.
   * It is also good practice to check the other pages to make sure everything seems normal. 

8. **Check the website on both desktop and mobile.**

   * Make sure the layout still looks correct.
   * Pay particular attention to images, menus, buttons and text.

## Important

* **GitHub is the master copy.**
* Do not use a separate copy on a personal computer as the main version of the website.
* Do not manually upload files to Cloudflare Pages.
* Make changes through GitHub so that the website's history and previous versions are recorded.
* Keep GitHub access restricted to people who need permission to edit the website.
* If you are unsure about a change, **do not commit it**. Ask another website administrator to check it first.


DOMAIN AND HOSTING
The organisation should control its Github, Cloudflare account, and .org.uk domain. Avoid making a volunteer's personal account the sole point of access.

ACCESSIBILITY
Keep the skip link, keyboard focus styles, meaningful image alt text, readable text sizes and responsive layout when editing the site.
