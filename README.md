<img width="1200" height="525" alt="jt_social_bar" src="https://github.com/user-attachments/assets/9e391676-efbb-4740-8dbe-30041be05aa6" />


# Joomtheme Social Share Bars Updates

This repository contains the Joomla update server files for **Joomtheme Social Share Bars**.

It is used to publish update metadata for the plugin, including the update XML feed and changelog XML, so Joomla can detect and deliver new versions through the Joomla Update System.

## Repository Purpose

This repository is dedicated to update delivery only.

It does **not** contain the full plugin source code.  
The plugin package itself is distributed separately through Joomtheme.

## Files

### `updates/socialsharebars.xml`
Main Joomla update server file.

This file provides:
- extension name
- version
- Joomla target platform
- direct package download URL
- changelog URL
- optional SHA256 checksum

### `updates/changelog_socialsharebars.xml`
Changelog file used by Joomla to display release notes in the update interface.

## Extension Information

- **Extension Name:** Social Share Bars
- **Type:** Joomla Content Plugin
- **Element:** `socialsharebars`
- **Folder:** `content`
- **Client:** `site`

## Compatibility

- **Joomla:** 6.x
- **PHP:** 8.3+

## Update Flow

1. Build a new plugin release package
2. Upload the ZIP package to the Joomtheme download location
3. Update the version number in `updates/socialsharebars.xml`
4. Update the direct ZIP download URL
5. Add or update the SHA256 checksum if used
6. Update `updates/changelog_socialsharebars.xml`
7. Commit and publish changes

Once published, Joomla sites using the plugin can detect the new version through the configured update server.

## Important Notes

- The `downloadurl` value in the update XML must point to the **direct ZIP package**
- Do **not** use a product page or shop page as the package download URL
- The update XML should match the plugin manifest values exactly
- This repository is intended only for update metadata distribution

## Maintainer

**Joomtheme**  
Website: https://joomtheme.com/
