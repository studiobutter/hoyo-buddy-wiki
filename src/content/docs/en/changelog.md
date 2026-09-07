---
title: "Changelogs"
---

## v1.16.23

### New Features

- (`/search hsr`) Add Enemy category.
- (`/challenge hsr`) Add Starward mode to Memory of Chaos, Pure Fiction, and Apocalyptic Shadow cards.
- (`/challenge zzz`) Add Hard mode to the Deadly Assault card.
- (`/gacha-log import`) Add one-click import for ZZZ HoYoLAB accounts, no URL needed.
- (`/mimo`) Add point history view.
- (`/accounts`) Show the status and last run time of each auto task for the selected account.
- (`/profile zzz`) Add Sigrid card data.

### Improvements

- (`/search`) Split into `/search genshin` and `/search hsr` subcommands, mirroring `/profile`.
- (`/gacha-log import`) Only fetch new records instead of the full history on every import.
- (`/gacha-log view`) Automatically keep standard banner item lists up to date, so 50/50 win rate stats stay accurate when limited items join the standard pool.
- (`/challenge hsr`) Show the Starward team even when the Starward stage wasn't cleared.
- (`/challenge genshin stygian`) Restore enemy weakness and strength info.
- (`/accompany`) Show the auto accompany toggle in the character view.
- (`/notes`) Remove the HSR expedition column and reminder, as expeditions no longer exist in HSR.
- Stop delivering queued auto task DM notifications after their setting has been turned off, and show the time of the action on each notification.
- Combine up to 10 auto task notifications into a single DM and drop successful ones older than 12 hours.

### Bug Fixes

- (`/gacha-log view`) Fix ZZZ S-ranks pulled during their own rate-up banner being counted as 50/50 losses.

## v1.16.22

### New Features

- (`/accompany`) Add new command to view HoYoLAB accompany characters, set yours, and enable auto check-in.
- (`/settings`) Add new settings related to auto accompany check-in feature.
- (`/profile genshin`) Add Enka style cards for Genshin Impact.
- (`/profile hsr`) Add new HSR character card data, including Himeko SP.
- (`/profile zzz`) Add ZZZ 3.1 character card data.
- (`/profile zzz`) Add support for the Lumiflux element.
- (`/card-settings`) Enable the substat roll display toggle for Enka style cards in Genshin and HSR.

### Improvements

- (`/card-settings`) Redesign image settings and merge them into card settings; the standalone image settings button in `/profile` is removed.
- (`/card-settings`) Allow custom image settings on all templates, with a warning when the selected template doesn't support them.
- (`/card-settings`) Show official art previews based on the actual card art.
- (`/card-settings`) Remove Pixiv support for custom images, as the service it relied on no longer works.
- (`/profile genshin`) Remove the hattvr template; existing settings are migrated to the Enka style template.
- Improve character autocomplete speed and reliability for Genshin and HSR commands.

### Bug Fixes

- (`/profile`) Fix Traveler pre-selection when passed as a parameter.
- (`/profile zzz`) Fix error for W-Engines without a sub-stat.
- (`/profile zzz`) Fix wrong Velina skin ID.
- (`/card-settings`) Fix crash caused by character ID collisions between games.
- (`/card-settings`) Fix image selector not opening on the current image's page.
- (`/characters zzz`) Fix crash when there are more than 25 faction filter options.
- (`/characters genshin`) Fix error when submitting an empty filter selection.
- (`/challenge`) Show history when the current phase has no data.
- (`/challenge genshin`) Fix the Spiral Abyss damage info section disappearing when some ranks have no data.
- (`/events`) Fix error when an event reward has an unknown rarity.
- (`/search`) Fix autocomplete error for beta items.
- Fix documentation links opening in the wrong language.

## v1.16.21

### New Features

- (`/profile hsr`) Add HSR 4.3 character card data.
- (`/profile zzz`) Add ZZZ 3.0 character card data.
- (`/profile`) Add Enka style cards for HSR and ZZZ.
- (`/profile zzz`) Add support for the Wind element.
- (`/characters zzz`) Show W-engine and skill levels.

### Improvements

- (`/profile`) Speed up card rendering by caching resized images.
- (`/characters`) Cache rendered pages for faster navigation.
- (`/events`) Show a clear unsupported-feature message for games without an event calendar.
- (`/notes`) Show reminder text in mobile push notifications.

### Bug Fixes

- (`/challenge hsr`) Handle incomplete floor data in Apocalyptic Shadow, Memory of Chaos, and Pure Fiction without erroring.
- (`/profile`) Fix Genshin Impact damage bonus stat incorrectly defaulting to Anemo.
- (`/profile`) Fix Genshin Impact card errors caused by missing stats and costume art data.
- (`/profile zzz`) Fix image positions for ZZZ 3.0 template 2 characters.
- (`/card-settings`) Fix validation error when configuring the Genshin Traveler.
- (`/search`) Fix error when opening the Quotes or Stories pages for characters with no data.
- (`/redeem`) Improve handling of code redemption errors.
- Fix disabling notifications not taking effect, which could cause unwanted auto-redeem DMs.
- Fall back to your Discord client language when no language is set in settings.

## v1.16.20

### New Features

- (`/profile zzz`) Add ZZZ 2.8 character card data.
- (`/profile zzz`) Add Miyabi skin card data.

### Improvements

- (`/profile hsr`) Improve stat display logic in build cards, including Elation damage boost stats.

### Bug Fixes

- (`/profile zzz`) Fix new ZZZ characters missing Mindscape images.
- (`/profile`) Preserve the order of characters passed as parameters.
- (`/gacha-log`) Show a placeholder image for missing gacha item icons.

## v1.16.19

### New Features

- (`/challenge hsr anomaly`) Now fetches the 3 most recent runs.
- (`/mimo`) Add support for completing Genshin video tasks.
- (`/notes`) Add ZZZ Cloud Global option to open game buttons.
- (`/profile hsr`) Show Trailblazer's path instead of element.

### Improvements

- (`/profile`) Add support for new HSR characters and Elation Trailblazers.
- (`/challenge zzz shiyu`) Hide clear time text in newer card layouts.

### Bug Fixes

- (`/challenge hsr anomaly`) Fix icon position for empty character blocks.
- (`/profile zzz`) Fix bad image positions or missing skin images for Aria and Nangong Yu.

## v1.16.18

### New Features

- (`/profile`) Add support for new ZZZ 2.7 and HSR 4.1 characters.

### Bug Fixes

- (`/characters zzz`) Fix performance issue when there are many characters.
- (`/events hsr`) Fix Anomaly Arbitration showing wrong name in dropdown.
- (`/card-settings`) Fix invalid query error for ZZZ.
- (`/notes`) Fix error when switching accounts in the UI.
- (`/search`) Fix error when searching books in HSR.
- (`/profile zzz`) Fix Aria's image appearing incorrectly in team cards.
- (`/profile zzz`) Fix Pan Yinhu skin missing card data.

## v1.16.17a

### Improvements

- Update to "Did you know" tip message - April 1st, 2026

## v1.16.17

### New Features

- (`/profile hsr`) Add support for new characters in HSR 4.0, including the new Elation path.
- (`/challenge zzz shiyu`) Add support for Shiyu Defense v2.
- (`/profile zzz`) Add card data for ZZZ 2.6 characters.

### Bug Fixes

- (`/challenge zzz shiyu`) Fix card rendering issues and handle errors when fetching Shiyu Defense data.
- (`/characters hsr`) Fix filter breaking when path character counts are missing.
- (`/events zzz`) Fix weapon object parsing.
- (`/profile hsr`) Fix rank percentage formatting for top-ranked builds.
- (`/notes`) Fix missing stamina reminder interval for Honkai Impact 3rd.
- Fix localization newline issues in zh-CN and other languages.

## v1.16.16

### New Features

- (`/profile zzz`) Add ZZZ 2.5 character card data, including Jane Doe's skin.
- (`/profile hsr`) Add initial support for the Elation path type.
- (`/gacha-log`) Add support for new ZZZ banner types (official import only).
- (`/build zzz`) Show guide author and last updated date in the overview.

### Improvements

- (`/build zzz`) Improved spacing and readability of guide sections.

### Bug Fixes

- (`/gacha-log upload`) Fix UIGF v4.1 import not working.
- (`/notes`) Allow setting reminder notify time to 0 hours before.
- (`/mimo`) Disable auto draw for Genshin Traveling Mimo.
- (`/mimo`) Handle -510001 error when fetching Genshin Mimo tasks.

## v1.16.15

### New Features

- (`/build zzz`) Added a command for showing character builds for ZZZ.
- (`/profile hsr`) Added The Dahlia card data.
- (`/mimo`) Re-enabled Genshin Impact support for Traveling Mimo.
- (`/mimo`) Added support for new Genshin Impact Traveling Mimo task types.
- Improved font detection to better handle Arabic and other non-Latin scripts.

### Improvements

- (`/profile hsr`) Improved The Dahlia's card color.
- Implemented zero-downtime updates - the bot will no longer go offline during code updates.

### Bug Fixes

- (`/profile genshin`) Fixed KeyError when converting HoYoLAB Genshin Impact characters.
- (`/gacha-log view`) Fixed missing item icons for HSR and ZZZ gacha logs.
- (`/gacha-log view`) Fixed UI issues on small screen devices.
- Fixed toggle switches not properly returning `False` for disabled options.
- Fixed several internal deployment and scheduling issues.

## v1.16.14

### New Features

- (`/profile`) Add support for new ZZZ characters.
- (`/exploration`) Add new regions.
- (`/events`) Add support for ZZZ.

### Improvements

- (`/characters`) Sort characters by level by default.
- (`/characters`) Add subtle glow of character rarities to card backgrounds.
- (`/about`) Use Discord protocol URLs for users links.
- Add fake settings buttons to guide users to use `/settings`.

### Bug Fixes

- (`/challenge genshin`) Fix text overflow for Stygian Onslaught and Imaginarium Theater cards.
- (`/challenge genshin theater`) Fix Arcana Challenges not showing up when language is Vietnamese.
- (`/challenge hsr anomaly`) Fix text overflow in season name.
- (`/settings`) Fix not being able to select accounts for Traveling Mimo settings.
- (`/settings`) Fix TOT accounts being able to access reminder settings.
- (`/profile hsr`) Fix trace positions in build cards.
- (`/profile hsr`) Fix missing stat icons for certain characters.
- (`/search`, `/profile zzz`) Fix missing characters like Ellen, Soldier 11 in autocomplete.
- (`/settings`) Fix wrong setting being changed when clicking on redeem notification toggles.
- (`/profile zzz`) Fix Rina's image not aligned to the center in team cards.
- Change UID masking character from '*' to 'x' to avoid markdown issues.

## v1.16.13

### New Features

- (`/profile`) Add support for new HSR and ZZZ characters.
- (`/challenge genshin theater`) Add support for Arcana Challenges.
- (`/profile hsr`) Add light cone stats for HoYoLAB/Miyoushe characters.
- (`/challenge hsr anomaly`) Add support for Anomaly Arbitration.
- (`/profile genshin`) Add support for Manekin and Manekina.
- (`/gacha-log`) Add support for Miliastra Wonderland.
- (`/settings`) Revamped settings command UI.

### Improvements

- (`/gacha-log view`) Improve performance of gacha log viewer.
- Improve performance of auto check-in, auto redeem, and auto Traveling Mimo tasks.
- Improve overall performance of the bot.

### Bug Fixes

Too many to list, see the [full changelog](https://github.com/seriaati/hoyo-buddy/releases/tag/v1.16.13).

## v1.16.12

Note: This version disables Traveling Mimo for Genshin Impact due to removal from HoYoLAB. The feature will be re-enabled once it is back.

### New Features

- (`/profile`) Add support for new HSR and ZZZ characters.
- (`/gacha-log import`) Use our [own script](https://github.com/studiobutter/gacha-stuff) for importing gacha logs.
- (`/challenge zzz shiyu`) Replace fastest clear time with total clear time.
- (`/challenge genshin stygian`) Add enemy weakness and strength info.
- Add support for Nod-Krai city.

### Improvements

- (`/profile`) Add more robust error handling for Enka Network API requests.
- (`/profile`) Add error handling for Enka Network build API requests.
- (`/profile`) Add error handling for third party card generation APIs.
- (`/accounts`) Handle Discord OAuth2 API errors.
- (`/notes`) Add descriptions for different inputs in the reminder settings modal.
- Due to a Discord bug, WEBP images can't be copied, so we now send infographics as PNGs instead.

### Bug Fixes

- (`/gacha-log view`) Fix Custom Celestial Invitation characters not being counted as 50/50 losses.
- (`/gacha-log view`) Fix wrong item rarity for some ZZZ items.
- (`/search`) Fix unreleased ZZZ characters sometimes shown in autocomplete.
- (`/challenge zzz shiyu`) Handle cases where there are no total clear time.
- (`/upload`) Fix image upload issues.
- (`/challenge genshin stygian`) Fix text overflow for some enemies.
- (`/challenge zzz assault`) Fix issues with accessing bangboo icons for past challenges.
- (`/gacha-log view`) Handle invalid banner type input.
- (`/challenge`) Fix issues with challenge phase dropdown when there are more than 25 phases.

## v1.16.11

### New Features

- (`/search`) Add Ice Trailblazer.
- (`/accounts`) Add device identifier for email logins, so you can see Hoyo Buddy's device on Hoyoverse account center.

### Bug Fixes

- (`/profile zzz`) Update enka.py to match new API format.
- (`/profile`) Fix Enka results always returned in English.
- (`/exploration`) Fix tribe level text overflow.
- Fix translations issues with en-GB locale.

## v1.16.10

### New Features

- (`/profile hsr`) Support new characters: Hysilens & Cerydra.
- (`/gacha-log upload`) Show error when account game and imported game are different.

### Improvements

- (`/gacha-log import`) Improve import performance.
- Cache frequently used data like settings and card settings to improve performance.
- Blur 5 digits of UID instead of 3.

### Bug Fixes

- (`/profile zzz`) Fix missing costume images for team cards.
- (`/profile zzz`) Fix missing data for Alice's summer costume.
- (`/profile zzz`) Fix error caused by costume data.
- (`/profile zzz`) Fix Enka Network builds not being shown sometimes.
- (`/search`) Fix unreleased content being shown in normal search autocomplete.

## v1.16.9

### New Features

- (`/profile zzz`) Add support for Enka Network.
- (`/about`) Add more links to the command.
- Add `/changelog`, `/invite`, and `/help` commands.
- Add documentation support for Simplified Chinese and Spanish.
- Add [status page](https://status.seria.moe/?category=Hoyo%20Buddy) to check the bot's status.

### Improvements

- (`/settings`) This command now responds with ephemeral messages.

### Bug Fixes

- (`/accounts`) Fix account login issues.
- (`/gacha-log manage`) Fix wrong item rarity for ZZZ export.
- (`/gacha-log view`) Fix item name being "???" for HSR collaboration banner characters and light cones.
- (`/profile genshin`) Fix no player embed being shown when data source is HoYoLAB.

## v1.16.8

### New Features

- (`/challenge zzz shiyu`) Add clear time.
- (`/challenge hsr`) Hide quick clears.
- (`/challenge hsr`) Add "Show UID" option.
- (`/gacha-log`) Support HSR collaboration banners.
- (`/profile zzz`) Add support for new characters: Alice and Yuzuha.
- (`/profile zzz`) Add support for agent outfits.
- The bot won't be offline during code updates now.

### Improvements

- (`/profile hsr`) Improve text position for template 2.
- (`/events`) Improve color contrast in light mode.
- (`/gacha-log view`) Change web app link when banner type is changed.
- (`/search`) HSR character story is now shown in a clearer way.
- Improve image generation performance with better caching.
- Save images as webp instead of png to reduce file size.

### Bug Fixes

- (`/redeem`) Fix lowercase codes not counting as redeemed.
- (`/characters genshin`) Fix text position issues.
- (`/characters genshin`) Fix images of some characters being in different styles.
- (`/profile hsr`) Fix font issues in light cone names in template 2.

## v1.16.7

### New Features

- Add Arabic support.
- (`/challenge genshin`) Add Stygian Onslaught card generation.
- (`/profile zzz`) Add acronym for "Automatic Adrenaline Accumulation" for template 4.

### Improvements

- (`/accounts`) Show a page while fetching accounts.
- (`/accounts`) Update APK file URL for Miyoushe logins.
- (`/accounts`) Add input field for aaid when adding Miyoushe accounts.
- Faster image generation by utilizing multiple CPU cores.
- More precise text positions in images.

### Bug Fixes

- (`/profile zzz`) Fix Yixuan's image position in template 1.
- (`/profile zzz`) Fix PEN stat not being translated in template 4.
- (`/search`) Disable spiral abyss category.
- (`/search`) Fix no autocomplete choices for drive disc category.

## v1.16.6

### New Features

- (`/profile zzz`) Add ZZZ 2.0 new characters card data.
- (`/profile zzz`) Add support for Rupture agents and Sheer Force stat.
- (`/gacha-log import`) Handle authkey exceptions.
- Add anniversary dismissible.

### Improvements

- (`/profile zzz`) Remove spaces in background agent names.

### Bug Fixes

- (`/characters genshin`) Handle no-element characters.
- (`/challenge genshin theater`) Handle invalid character IDs.

## v1.16.5

### New Features

- (`/profile hsr`) Add v3.3 new characters card data.
- (`/profile hsr`) Add support for Remembrance path characters to use StarRailCard templates.
- (`/profile`) Handle Enka Network API request timeout error.
- (`/search`) Enable unreleased content category.

### Bug Fixes

- (`/redeem`) Remove 'user' parameter from the command.
- (`/mimo`) Remove UID blur in auto mimo task embeds.
- (`/upload`) Handle image files that are too large.
- (`/search`) Fix incorrect calculation formula for character & light cone stats.
- (`/accounts`) Fix 'next page' option not working when user has more than 25 accounts.

## v1.16.4

### New Features

- (`/profile genshin`) Support no element traveler.
- Add Hindi fonts.

### Improvements

- (`/profile`) Removed character data cache
- Added constraints to gacha-log filters.

### Bug Fixes

- (`/events`) Fixed not finding banner announcements
- (`/challenge genshin theater`) Fixed Imaginarium Theater data not showing.
- (`/profile`) Fixed compatibility issues with Enka Network builds.
- (`/mimo`) Fixed Miyoushe users being able to access the command.
- (`/notes`) Ignore game maintenance errors when doing real-time notes check.
- (`/lb view`) Removed Honkai Impact 3rd achievement leaderboard.
- (`/farm reminder`) Fixed item names being "..."

## v1.16.3

### New Features

- (`/profile zzz`) Added Vivian & Hugo's card data.
- Added Portuguese (Brazil) translation.
- Added Japanese translation.

### Improvements

- (`/profile zzz`) Adjusted the image positions of some characters.
- (`/profile zzz`) Improved image layers for card templates.

### Bug Fixes

- (`/notes`) Fixed parametric transformer notifier not working.
- (`/gacha-log upload`) Fixed wrong item rarity for some ZZZ import methods.

## v1.16.2

### New Features

- (`/profile hsr`) Added Castorice & Anaxa's card data.

### Bug Fixes

- (`/profile zzz`) Fixed Pulchra's image position in card template 2.
- (`/build genshin`) Fixed artifact position emojis not being shown properly for user apps.

## v1.16.1

### New Features

- (`/gacha-log upload`) Added support for importing from [Starward](https://github.com/Scighost/Starward) for ZZZ.
- (`/redeem`) Added notification settings.
- (`/accounts`) Added instructions for gettings aaid for adding Miyoushe accounts.
- Added "Hide UI" button for commands that have many buttons.

### Improvements

- (`/search`) Removed "unreleased content" category, see [this message](https://discord.com/channels/1000727526194298910/1042428379120545873/1346411349999357973) for why.
- (`/characters`) Allow selecting nothing for the filters.
- Increased performance for auto tasks.

### Bug Fixes

Various bug fixes, see the [full changelog](https://github.com/seriaati/hoyo-buddy/releases/tag/v1.16.1) for more details.

## v1.16.0

[For the nerds](https://github.com/seriaati/hoyo-buddy/releases/tag/v1.16.0)

### New Features

- (`/profile`) Added template previews in card settings.
- (`/profile`) Show custom image availability in card template dropdown.
- (`/notes`) Increased trailblaze power limit to 300.
- (`/notes`) Added open game buttons.
- (`/search zzz`) Added core skill level dropdown.
- (`/gacha-log import`) Compare UID of incoming logs with the UID of the account being imported to.
- Automatically set new user's language based on their Discord client's language.

### Improvements

- (`/redeem`) Improved UX by fixing no response when redeeming a redeemed code.
- (`/gacha-log`) Made account parameter required to avoid confusion.
- Show better error messages for "Missing Permissions" and "Message Blocked by AutoMod" errors.
- Simplified texts shown in account set up process.

### Bug Fixes

Various bug fixes and improvements.

## v1.15.7

### New Features

- (`/web-events`) Added a new command to view on-going web events and set notifier to remind you when there is a new event.
- (`/notes`) Added bounty commission and Ridu weekly points notifiers for ZZZ.
- (`/about`) Added changelog button.

### Improvements

- (`/gacha-log view`) Improved gacha log page performance by fixing cache issues.
- (`/about`) Removed latest git changes.
- (`/mimo`) Sort Traveling Mimo shop items from most expensive to least expensive when auto buying.
- Improves localization for other languages.
  
### Bug Fixes

- (`/characters genshin`) Fixed KeyError caused by no-element travelers.
- (`/characters genshin`) Fixed incorrect talent level for Kamisato Ayaka.
- (`/stats`) Fixed "Record card not found for ..." error for ZZZ.
- (`/build genshin`) Fixed "No block lists to draw" error.
- (`/gacha-log view`) Fixed incorrect 50/50 win rate.
- (`/gacha-log view`) Fixed 422 validation error on web app.
- (`/gacha-log view`) Handle invalid size input.
- (`/gacha-log import`) Handle invalid banner types when importing gacha logs.
- (`/gacha-log import`) Fixed UIGF import.
- (`/mimo`) Confirm task finish status before sending notifications.
- (`/mimo`) Added sleep intervals between task completions to avoid being rate limited.
- (`/mimo`) Remove HTML tags from task names.
- (`/mimo`) Fixed error after buying an item.
- (`/profile`) Fixed card settings from different games being mixed up.
- (`/profile genshin`) Fixed extra talents being shown in team cards.
- (`/profile genshin`) Fixed validation error with Mavuika.
- (`/search`) Fixed W-engine refinement selector not updating selected value.
- (`/notes`) Fixed validation error for Honkai Impact 3rd.
- (`/challenge zzz assault`) Fixed buff icons not being shown.

## v1.15.6

### New Features

- (`/mimo`) Added support for Genshin's Traveling Mimo (event has already ended by the time of writing).
- (`/mimo`) Added auto prize draw feature.
- (`/challenge zzz`) Added support for the Deadly Assault game mode.
- (`/profile hsr`) Added template 2.
- (`/notes`) Added bounty commission and Ridu weekly points information for ZZZ.

## Improvements

- (`/check-in`) Reduce duplicate check-in API requests.

## Bug Fixes

- (`/mimo`) Fixed notifications being sent when no tasks are completed and no points are claimed.
- (`/mimo`) Fixed how valuable items are being determined.
- (`/mimo`) Handle -510001 error.
- (`/mimo`) Fixed an issue where valuable items are being counted as decorations for HSR.
- (`/mimo`) Disable lottery draw button when the limit is reached.
- (`/challenge zzz`) Fixed wrong bangboo icons in cards.
- (`/events`) Fixed wrong Spiral Abyss progress.
- (`/gacha-log view`) Fixed wrong number of pulls from last rarity.
- Fixed static image folder creation logic.

## v1.15.5

### New Features

- (`/mimo`) Automatically finish tasks that require commenting on a post.
- (`/mimo`) Automatically finish tasks that require following a topic.
- (`/mimo`) Added lottery feature.
- (`/mimo`) Added notification settings.
- (`/profile zzz`) Added an image setting to use Mindscape 3 arts for build cards.
- (`/profile zzz`) Added Harumasa and Miyabi card data.
- (`/search`) Hide "unreleased content" category in certain guilds.

### Improvements

- (`/mimo`) Show task progress for certain tasks.
- (`/mimo`) Show names of completed tasks in the notification.
- (`/mimo`) Improved performance of auto tasks.
- (`/challenge zzz shiyu`) Updated card layout.
- (`/challenge zzz shiyu`) Avoid fetching agent data twice.
- Show Discord server invite link in error embed footers.
- Unset item loading state upon error.
- Added on/off labels to toggle buttons.
- Improved proxy API request logic.
- Improved auto tasks error handling logic.

### Bug Fixes

- (`/mimo`) Added a sleep interval after redeeming a mimo reward gift code.
- (`/mimo`) Fixed tasks missing in task list.
- (`/mimo`) Fixed comment tasks not being completed.
- (`/mimo`) Fixed notifications being sent when no tasks are completed.
- (`/mimo`) Only show HoYoLAB accounts in the account autocomplete.
- (`/mimo`) Fixed `QuerySetError` in auto tasks.
- (`/mimo`) Fixed post comments not being deleted.
- (`/mimo`) Handle cases where Traveling Mimo is not available for a game.
- (`/profile zzz`) Fixed substat highlights not being added to the card.
- (`/profile zzz`) Fixed agents being identified as cached when they are not.
- (`/characters zzz`) Fixed wrong total agent count.
- (`/gacha-log upload`) Fixed issues with zzz.rng.moe imports.
- (`/redeem`) Fixed Miyoushe accounts being shown in account autocomplete.
- (`/build genshin`) Handle missing usage rates for some characters.
- (`/events`) Fixed future HSR warps not being shown as "not available yet".
- Adapt to new ZenlessData keys.
- Fixed issues with Hakushin API.
- Capture general exceptions in `dm_user` method.

## v1.15.4

### New Features

- (`/build genshin`) Show information about the synergies of a character.
- (`/mimo`) Added a new command to manage Traveling Mimo.

### Improvements

- (`/build genshin`) Improved the card designs.
- (`/notes`) Use the event calendar API to check for planar fissure events.

### Bug Fixes

- (`/build genshin`) Fixed some UI issues.
- (`/events`) Fixed some issues causing the command to be inaccessible.
- (`/gacha-log upload`) Fixed `ValidationError` with UIGF data.
- (`/gacha-log upload`) Fixed `KeyError` with UIGF versions older than 3.0.
- (`/search`) Fixed duplicated autocomplete choices.

## v1.15.3

Bad code in the previous versions caused some users to see the "too many requests" error while logging in, please see
[this article](./too-many-requests.md) for more information.

### New Features

- (`/profile zzz`) Added a selector to select substats that you want to highlight.
- (`/profile hsr`) Added Fugue and Sunday card data.

### Improvements

- (`/redeem`) Mask redeem code links with the code itself.
- (`/challenge genshin theater`, `/challenge genshin abyss`) Show traveler's element in the cards.
- (`/accounts`) Show custom error message for "Too many requests" error.

### Bug Fixes

- Fixed an issue where commands are not being translated to other languages.
- Fixed an issue where timed out modals are not being closed properly.
- Fixed API retry logic and error handling logic.
- Fixed `ValueError` in some commands.
- Fixed modal timeout time being too short.
- Handle `KeyError` in web server redirect endpoint.
- (`/profile`) Handle `EnkaAPIError` when fetching data from Enka Network API.
- (`/profile`) Handle Enka Network API gateway timeout errors gracefully.
- (`/profile`) Fixed `BadRequestError` when generating AI images.
- (`/upload`) Fixed `BadRequestError` when uploading images.

## v1.15.2 and below

Previous changelogs were written in the #updates channel in our [Discord server](https://link.seria.moe/hb-dc).
