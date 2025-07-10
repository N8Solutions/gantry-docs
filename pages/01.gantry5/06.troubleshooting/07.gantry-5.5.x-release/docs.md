---
title: Gantry 5.5.x Release - Important notes before you update!
date: 2021-10-20
taxonomy:
    category: docs
    tag: [gantry5, joomla4, rockettheme]
---

**TL;DR:**  
Don’t update to Gantry 5.5.x until you have updated your RocketTheme (RT) theme to a compatible version first.  
If you already updated to G5.5 and are stuck with it, G5.5.x has many significant bug fixes, so you should update to the latest version.

Today sees the release of the long-awaited Gantry 5.5.x.  
This major update brings significant improvements, including:

- Support for Joomla 4 (Joomla 3.10.x also supported)
- WP5.8.x blocks support
- PHP8 support

Before you update, please read the following important notes:

1. **Study the changelog** for Gantry 5.5.0 through to the current version of 5.5.x — there are big changes you should be aware of:  
   [https://gantry.org/downloads](https://gantry.org/downloads)

2. **Upgrade on a test environment first** to make sure everything works as you expect.

3. **Backup, backup, backup!**  
   Before you do anything, make sure you can restore if something goes wrong. The update to Gantry 5.5.x is a one-way process — you cannot downgrade back to Gantry 5.x without using your restore.

4. **Menu system migration:**  
   Gantry 5.5.x introduces significant redevelopment of the menu system. Immediately after updating, go to the Gantry 5 menu editor and save each of your menus. This migrates your existing menus from the old YAML method (flat files) to the CMS database.

5. **Clear browser and server cache** after updating.

6. **Template support:**  
   Alongside Gantry 5.5.x, compatible versions of the Helium and Hydrogen themes have been released. Other RT themes will also need updates (many have already been released — 27 of 45 for Joomla, WordPress, and GRAV). If you use an RT theme, wait for its update.  
   There are manual methods to update an RT theme to work with Joomla 4, but it’s better to wait for the official RT theme update (see the changelog; it involves copying folders from Helium and checking/reapplying theme overrides).

7. **Joomla 4 & Gantry 5.5:**  
   Gantry 5.5.x now supports Joomla 4, but Joomla 4 introduces Bootstrap 5, which can change your site’s look (RT is working to minimize this). Joomla 4 also changes some of the HTML structure, which may require changes to your `custom.scss` selectors.  
   Note: Old RT extensions do **not** work with Joomla 4 (and won’t be made to do so). Consider this before migrating to Joomla 4 (which requires Gantry 5.5.x).

8. **Internal code updates:**  
   There are significant updates to third-party code Gantry 5 uses (such as the SCSS compiler). This may require changes to your custom code (like `custom.scss`), as the new SCSS compiler is stricter. RT themes are also affected, so they need updates too.

9. **Cosmetic/layout changes:**  
   Some things may look different after migrating, which may require you to write or amend your `custom.scss`.

10. **Further reading:**  
   - [Gantry 5 Dev team notes, GitHub Issue #2789](https://github.com/gantry/gantry5/issues/2789#issuecomment-947948729)
   - [Gantry 5.5 Upgrade Notes, GitHub](https://github.com/gantry/gantry5/blob/develop/UPGRADE-5.5.md)

---

*Document created from an Evernote web clip of the original RocketTheme forum post by Mark (aka MrT).*
