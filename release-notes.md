---
description: The history of Ignited's development.
---

# 📔 Release Notes

## <mark style="color:orange;">Ignited 1.8.3</mark>

<mark style="color:orange;">1/11/2024</mark>

#### New

* Added a check for N64 games to disallow mismatched OpenGLES versions
* Added a view in settings to see all games with OpenGLES 3 enabled and remove them
* Added a view in settings to see all games with Invalid VRAM Access enabled and remove them

## <mark style="color:orange;">Ignited 1.8.2</mark>

<mark style="color:orange;">1/10/2024</mark>

#### New

* SNES Invalid VRAM Access
  * Allows text and other sprites to render properly in some emulator-only games
  * Applied per game using the game's context menu

#### Changed

* N64 Graphics replaced with OpenGLES 3 toggle
  * Applied per game using the game's context menu
* Toast notification style updated and the code flow for toasts has been unified/simplified

## <mark style="color:orange;">Ignited 1.8.1</mark>

<mark style="color:orange;">1/8/2024</mark>

#### New

* Microphone can now be toggled on and off, and only allows microphone usage when using the melonDS core
* Create an auto save state any time the app becomes inactive, even when immediately quitting the app from a game
* Adds new icons by LitRitt and Kongolabongo

#### Changed

* Makes the Pro label fancy
* Makes the alternate icon feature free, some icons will remain Pro only
* Removes the Documentation link until it's more complete
* Makes most system titles use full names instead of short names
* Unhides the status bar feature in settings

#### Fixed

* Fixes patrons list after update to Patreon benefits
* Fixes toggling the status bar showing the wrong toast notification
* Fixes setting game preview parameters when feature is disabled

## <mark style="color:orange;">Ignited 1.8</mark>

<mark style="color:orange;">1/6/2024</mark>

#### New

* Ignited Pro
  * Select features and options will now only be available to patrons
* Patreon Integration
  * You can now link your Patreon account within the app to access Ignited Pro

#### Fixed

* Fixes skin debugging being shown when the feature is off
* Fixes game search results overlapping other games
* Makes the transition from Quick Settings to Main Menu create an auto save state
* Fixes animated artwork still animating when the feature is off

## <mark style="color:orange;">Ignited 1.7.2</mark>

<mark style="color:orange;">12/23/2023</mark>

#### New

* Makes the Pause Menu items able to be rearranged in settings
* Adds options for opening the Pause Menu by shaking your device

#### Changed

* Makes the New Game, Pause, and Star icons on artwork able to be disabled
* Makes context menu previews use auto-save states if enabled
* Updated artwork database to include Master System and Game Gear games

#### Fixed

* Makes custom artwork background color support transparency
* Adjusts DS artwork forced aspect ratio

## <mark style="color:orange;">Ignited 1.7.1</mark>

<mark style="color:orange;">12/6/2023</mark>

#### Bugfixes

* Fixes crash when mapping controller inputs
* Makes custom artwork background color support transparency
* Adds missing toggles back into artwork settings

## <mark style="color:orange;">Ignited 1.7</mark> <a href="#id-161---10312023" id="id-161---10312023"></a>

<mark style="color:orange;">12/2/2023</mark>

#### Core Separation

* Cores with support for multiple systems have been made into their own cores to allow for different controller skins and feature sets.
* Gambatte core has been separated into Game Boy (GB) and Game Boy Color (GBC).
* GPGX core has been separated into Genesis / Mega Drive (GEN), Master System (MS), and Game Gear (GG).

#### User Interface

* The app now fully supports a unique UI for both light mode and dark mode.
* You can either match your device dark mode setting or choose from either mode at any time.
* All custom assets have been replaced with SF Symbols for style consistency

#### Games Library

* New menu in the top right to access convenient settings and options without navigating the settings page.
* The import button will now become a menu to resume / play / import games once a game has been imported.
  * Resume or quit your currently playing game.
  * View your recently played games and choose one to play.
  * Choose a random game to play from your library or current collection of games.
* The bottom toolbar has been removed to free up space for your games.
* You can now change collections by tapping the collection title in the navigation bar.
* Unplayed games are now marked with a theme colored dot in the title, similar to updated iOS apps.

#### Game Artwork

* New theme system with 3 built in themes and a fully customizable custom theme.
* New custom made default box art for all 10 systems.
* There's now an option to force all artwork within a given collection to use the same aspect ratio, determined by the default box art.
* A screenshot of your latest save state will now be used as a game's artwork, if available. Can be turned off via the Live Artwork option.
* Currently playing game will be highlighted with a theme colored pause icon.

#### Favorite Games

* Favorite games now have a star icon displayed on the artwork.
* The style of favorite games can be completely customized independent of the main artwork theme.

#### Syncing

* Added automatic conflict resolution for all syncable files
* Whether or not a game is favorited is now synced.
* Auto-syncing (syncing every time you return to the library) can now be disabled. The app will always perform a background sync when the app launches, and this cannot be disabled.
* You can now manually trigger a sync from the library menu.

#### Save States

* Auto-Save states can now be disabled. Disabling Auto-Save states will also disable Auto-Load.
* Enabling Auto-Load states will also enable Auto-Save states.

#### Settings

* Sections have been rearranged. Most used sections will now be at the top.
* Some features have been explicitly made permanent with no option to disable them.
* If a feature can be toggled off, doing so will now completely disable that feature ( e.g. Background Blur).
* Many feature options have been reworked to be easier to understand and use.
* Patrons and contributors now load from a remote source
* Added official project links

#### Pause Menu

* Added new long-press actions to some pause menu items.
  * Long press Save/Load State to quick save/load.
  * Long press Screenshot to have a 3 second countdown before the screenshot is taken.
  * Long press Hold Buttons to reset your currently held inputs and select new inputs to hold. Tapping Hold Buttons now toggles your saved inputs on or off if you've selected inputs to hold. _\*Inputs are currently reset when the app quits. Plan to make these persist in a future update._
  * Long press Fast Forward to change the speed. Tap to toggle.

#### Quick Settings

* Added an option to open the Quick Settings menu via shaking your device
* Added an option to replace the Quick Settings menu on controller skins with a custom input: Quick Save/Load, Screenshot, Fast Forward, or Restart.

#### Device Shaking

* Shake your device to return to your currently playing game from anywhere else in the app.
* If no other "Shake to..." features are enabled, you can shake your device to pause your game.

#### Bugfixes

* Fixes supported controller skins being non-selectable until rotating your device to the orientation of the skin
* Many other small fixes and changes

## <mark style="color:orange;">Ignited 1.6.1</mark> <a href="#id-161---10312023" id="id-161---10312023"></a>

<mark style="color:orange;">10/31/2023</mark>

#### **New Features** <a href="#new-features" id="new-features"></a>

* Adds an option to replace the Quick Settings button on skins with another input
* Adds an option to open Quick Settings by shaking the device
* Adds a new menu to change or reset Override Traits, and to access the pause menu
  * Accessible via shaking the device
* Adds a Power User feature to copy the Google Drive refresh token
  * Allows other applications and services to access your Google Drive Ignited Sync backup files

## <mark style="color:orange;">Ignited 1.6</mark> <a href="#id-16---10302023" id="id-16---10302023"></a>

<mark style="color:orange;">10/30/2023</mark>

#### **New Features** <a href="#new-features-1" id="new-features-1"></a>

* Adds an informative popup after successfully importing controller skins and games
* Adds a setting to show unsupported controller skins
* Adds an All Systems page to settings for controller skin management

## <mark style="color:orange;">Ignited 1.5.6</mark> <a href="#id-156---10282023" id="id-156---10282023"></a>

<mark style="color:orange;">10/28/2023</mark>

#### **New Features** <a href="#new-features-2" id="new-features-2"></a>

* Adds support for dynamic background blur tinting based on device light/dark mode setting
  * The background blur will be darkened in dark mode and lightened in light mode
  * Intensity of the tint can also be adjusted

#### **Updates** <a href="#updates" id="updates"></a>

* Makes DSi support toggle-able
  * User’s won’t be able to add DSi BIOS files until toggling DSi support on first
  * The DSi NAND file will be removed when DSi support is toggled off to remove the DSi Home Screen
* Moves Core Settings below Features in the settings page

## <mark style="color:orange;">Ignited 1.5.5</mark> <a href="#id-155---10272023" id="id-155---10272023"></a>

<mark style="color:orange;">10/27/2023</mark>

#### **Updates** <a href="#updates-1" id="updates-1"></a>

* Changes some toast notifications to be disabled by default

#### **Bugfixes** <a href="#bugfixes" id="bugfixes"></a>

* Fixes a bug with AirPlay display losing transparency after rotating the device
* Fixes a bug with AirPlay not showing the correct DS screens on the external display
* Fixes games losing audio after switching systems

## <mark style="color:orange;">Ignited 1.5.4</mark> <a href="#id-154---10232023" id="id-154---10232023"></a>

<mark style="color:orange;">10/23/2023</mark>

#### **Bugfixes** <a href="#bugfixes-1" id="bugfixes-1"></a>

* Fixes wrong game collection being used for random game button
* Fixes a crash when selecting hold buttons
* Fixes a crash when displaying toasts

## <mark style="color:orange;">Ignited 1.5.3</mark> <a href="#id-153---8202023" id="id-153---8202023"></a>

<mark style="color:orange;">8/20/2023</mark>

#### **New Features** <a href="#new-features-3" id="new-features-3"></a>

* Added Random Game button to load a random game from your collection

#### **Updates** <a href="#updates-2" id="updates-2"></a>

* Improved preset theme color selection screen
* Updated DS default skin to new style
* Updated SNES default skin to new style

## <mark style="color:orange;">Ignited 1.5.2</mark> <a href="#id-152---7192023" id="id-152---7192023"></a>

<mark style="color:orange;">7/19/2023</mark>

#### **Updates** <a href="#updates-3" id="updates-3"></a>

* Adds new “Classic” icon by Kongolabongo
* Changes deep link scheme from delta:// to ignited://

#### **Bugfixes** <a href="#bugfixes-2" id="bugfixes-2"></a>

* Fixes a crash when remapping controller inputs
* Fixes deep links not loading auto save states in some scenarios
* Fixes wrong description for controller deadzone option

## <mark style="color:orange;">Ignited 1.5.1</mark> <a href="#id-151---7162023" id="id-151---7162023"></a>

<mark style="color:orange;">7/16/2023</mark>

#### **Updates** <a href="#updates-4" id="updates-4"></a>

* Different button overlay styles to choose from
* Updated button sounds to play through the audio engine instead of as system sounds
* Button sounds can be played at either their own volume, or the same volume of game audio

#### **Bugfixes** <a href="#bugfixes-3" id="bugfixes-3"></a>

* Fixes launching a game via deep link not respecting the auto load save state setting

## <mark style="color:orange;">Ignited 1.5</mark> <a href="#id-15---7132023" id="id-15---7132023"></a>

<mark style="color:orange;">7/13/2023</mark>

#### **New Features** <a href="#new-features-4" id="new-features-4"></a>

* AirPlay
  * Proper support for streaming games to an external screen
* Trigger Deadzone
  * Adjustable deadzone for trigger inputs on controllers
* Skin Background Color
  * Change the background color of controller skins from black to any other color

#### **Updates** <a href="#updates-5" id="updates-5"></a>

* Fast Forward inputs can now be manually switched between toggle and hold by users
* Improved default button mappings for various Switch controllers
* Updated app icon and other assets to match modified design
* Various syncing improvements in Harmony

#### **Bugfixes** <a href="#bugfixes-4" id="bugfixes-4"></a>

* Make Quick Settings dismissible with controller input
* Fixes DS save states made with JIT enabled not loading when JIT is not enabled
* Fixes crash when loading save states on iOS 17

## <mark style="color:orange;">Ignited 1.4.8</mark> <a href="#id-148---6252023" id="id-148---6252023"></a>

<mark style="color:orange;">6/25/2023</mark>

#### **New Features** <a href="#new-features-5" id="new-features-5"></a>

* Rotation Lock
  * Adds a pause menu button to lock device rotation during gameplay
* Adds an option to play a 3 second countdown between initiating and capturing a game screenshot

#### **Updates** <a href="#updates-6" id="updates-6"></a>

* Default skins with blurred backgrounds have been adjusted to look seamless on all device sizes
* New icon for hold buttons pause menu button
* Speed up importing compressed games in ZIP format by skipping checksum verification

#### **Bugfixes** <a href="#bugfixes-5" id="bugfixes-5"></a>

* Fixes game screenshots being saved to Photos as JPEG instead of PNG

## <mark style="color:orange;">Ignited 1.4.7</mark> <a href="#id-147---6192023" id="id-147---6192023"></a>

<mark style="color:orange;">6/19/2023</mark>

#### **New Features** <a href="#new-features-6" id="new-features-6"></a>

* Classic skins have been added to the Skin Downloads section in settings for users who want to use the old Delta skins

#### **Updates** <a href="#updates-7" id="updates-7"></a>

* Updated NES default skin with new design
* Default skins with new design have been updated to utilize the new backgroundBlur key
* Allows skin preview images to be in either pdf or png format
* Updated logic for when the background blur pause menu button should show

#### **Bugfixes** <a href="#bugfixes-6" id="bugfixes-6"></a>

* Fixes an issue with the default GBA E2E landscape skin image

## <mark style="color:orange;">Ignited 1.4.6</mark> <a href="#id-146---6172023" id="id-146---6172023"></a>

<mark style="color:orange;">6/17/2023</mark>

#### **New Features** <a href="#new-features-7" id="new-features-7"></a>

* Background blur toggle now available in the pause menu
* Background blur options now available in the quick settings menu

#### **Updates** <a href="#updates-8" id="updates-8"></a>

* Adds support for skin representations with the backgroundBlur key
* Adds an option to override the backgroundBlur setting of a skin
* Disables background blur on GPGX core for the time being
* Reverts and updates pause menu icons

#### **Bugfixes** <a href="#bugfixes-7" id="bugfixes-7"></a>

* Fixes N64 screens going black when toggling background blur

## <mark style="color:orange;">Ignited 1.4.5</mark> <a href="#id-145---6162023" id="id-145---6162023"></a>

<mark style="color:orange;">6/16/2023</mark>

#### **New Features** <a href="#new-features-8" id="new-features-8"></a>

* Blurred game backgrounds for skins
  * Options to enable/disable, change blur strength, and adjust the brightness
* Option to change the N64 graphics rendering API between OpenGL ES 2 and OpenGL ES 3

#### **Updates** <a href="#updates-9" id="updates-9"></a>

* Adds support for skins with .ignitedskin extension to differentiate between legacy Delta skins and new Ignited skins
* Adds more mappable inputs for controllers

#### **Bugfixes** <a href="#bugfixes-8" id="bugfixes-8"></a>

* Fixes overlapping buttons when mapping controller inputs
* Fixes crashes on N64 when opening menu and saving state

## <mark style="color:orange;">Ignited 1.4.4</mark> <a href="#id-144---672023" id="id-144---672023"></a>

<mark style="color:orange;">6/7/2023</mark>

#### **New Features** <a href="#new-features-9" id="new-features-9"></a>

* Adds several new alternate app icons and an interface to change between them
* Adds an option within every feature to reset all options to their default values, and a power user option to reset all options at once
* Adds an option to change the intensity of the favorite games highlight glow

#### **Updates** <a href="#updates-10" id="updates-10"></a>

* Makes the reset artwork feature work with the DS home screen icons
* Makes rewind deleting its states on rewinding or quitting the game a toggleable option
  * Allows the rewind feature to be used as a persistent secondary auto-save method

#### **Bugfixes** <a href="#bugfixes-9" id="bugfixes-9"></a>

* Fixes artwork size setting not applying until swiping to a new page

## <mark style="color:orange;">Ignited 1.4.3</mark> <a href="#id-143---642023" id="id-143---642023"></a>

<mark style="color:orange;">6/4/2023</mark>

#### **Updates** <a href="#updates-11" id="updates-11"></a>

* Adds an option for custom touch overlay color
* Creates a new feature section called Games Collection
* Moves settings previously found in Game Artwork Customization into separate sections within the Games Collection feature set
* Makes Favorites features respect whether the feature is actually enabled

#### **Bugfixes** <a href="#bugfixes-10" id="bugfixes-10"></a>

* Fixes lag when changing settings with animated artwork in the background
* Fixes animated artwork losing transparency when downsampling

## <mark style="color:orange;">Ignited 1.4.2</mark> <a href="#id-142---632023" id="id-142---632023"></a>

<mark style="color:orange;">6/3/2023</mark>

#### **New Features** <a href="#new-features-10" id="new-features-10"></a>

* Quick Settings
  * Quick access to game options and actions: screenshot, save, load, volume, game speed, palettes
  * Accessible from a controller/skin button as well as the pause menu

#### **Updates** <a href="#updates-12" id="updates-12"></a>

* New options for game title size and max lines, available in User Interface Features -> Game Artwork Customization

#### **Bugfixes** <a href="#bugfixes-11" id="bugfixes-11"></a>

* Fixes crash on iPad when resolving sync merge conflicts
* Fixes accidentally deleting Games directory during sync in rare circumstances

## <mark style="color:orange;">Ignited 1.4.1</mark> <a href="#id-141---5142023" id="id-141---5142023"></a>

<mark style="color:orange;">5/14/2023</mark>

#### **New Features** <a href="#new-features-11" id="new-features-11"></a>

* Adds an option to reset game artwork to the one provided by the games database
* Adds a power user option to reset artwork for every game at once

#### **Bugfixes** <a href="#bugfixes-12" id="bugfixes-12"></a>

* Fixes cancelling some pause menu popups causing the game to freeze
* Fixes incorrect checkmarks next to selected palette for sprite 1 and 2
* Fixes preview save state being overwritten by auto save state

## <mark style="color:orange;">Ignited 1.4</mark> <a href="#id-14---5132023" id="id-14---5132023"></a>

<mark style="color:orange;">5/13/2023</mark>

#### **Updates** <a href="#updates-13" id="updates-13"></a>

* Settings page has been completely revamped and reorganized
  * Many existing features received improvements as they were moved

#### **New Features** <a href="#new-features-12" id="new-features-12"></a>

* Game Boy color palettes
  * Several built in palettes and 3 user customizable palettes
  * Both the main and sprite palettes can be changed, allowing for unique palettes never before possible
* Custom Theme Color
  * Choose your own color to use for the app accent color
* Favorite Games
  * Games can be favorited, with options to highlight and sort them to the top of the games list
* Game Sorting
  * You can now sort games A-Z, Z-A, most recently played, and least recently played
* Animated Game Artwork
  * Support for short animated GIFs as your game artwork, with options for animation pause and speed

#### Bugfixes <a href="#bugfixes-13" id="bugfixes-13"></a>

* Burnt a bunch of bugs

## <mark style="color:orange;">Ignited 1.3</mark> <a href="#id-130---4282023" id="id-130---4282023"></a>

<mark style="color:orange;">4/28/2023</mark>

#### **New Features** <a href="#new-features-13" id="new-features-13"></a>

* Skin Debug Device
  * Switch to another device type when debugging a skin, useful for testing skins on devices you don’t own

#### **Updates** <a href="#updates-14" id="updates-14"></a>

* Adds toasts notifications for more actions

#### **Bugfixes** <a href="#bugfixes-14" id="bugfixes-14"></a>

* Now creates an auto save state when saving in-game, fixes old autosaves overwriting game data when loaded
* Fixes the Resume button not working with auto-load save states disabled
* Fixes the pause menu not fully showing in landscape with 2 rows of buttons

## <mark style="color:orange;">Ignited 1.2.10</mark> <a href="#id-1210---4232023" id="id-1210---4232023"></a>

<mark style="color:orange;">4/23/2023</mark>

#### **New Features** <a href="#new-features-14" id="new-features-14"></a>

* New Screenshot options
  * Save to Files, Save to Photos, Image Scale

#### **Updates** <a href="#updates-15" id="updates-15"></a>

* Forced light status bar during gameplay
* Updated licenses page formatting
* Reordered pause menu buttons and adjusted spacing to 4 items per row

#### **Bugfixes** <a href="#bugfixes-15" id="bugfixes-15"></a>

* Adjusted settings slider labels to fit with bold system text
* Removed unimplemented swipable page control

## <mark style="color:orange;">Ignited 1.2.9</mark> <a href="#id-129---4182023" id="id-129---4182023"></a>

<mark style="color:orange;">4/18/2023</mark>

#### **Updates** <a href="#updates-16" id="updates-16"></a>

* Added page for Lit Patrons shoutout
* Changed rewind to be disabled by default

#### **Bugfixes** <a href="#bugfixes-16" id="bugfixes-16"></a>

* Fixed a crash when toggling clicky haptics
* Removed unsupported file extensions on GPGX

## <mark style="color:orange;">Ignited 1.2.8</mark> <a href="#id-128---4162023" id="id-128---4162023"></a>

<mark style="color:orange;">4/16/2023</mark>

#### **New Features** <a href="#new-features-15" id="new-features-15"></a>

* Added toggle to show or hide the status bar while in-game
* Added Resource Links section to settings
* Added Rom Patcher JS and DS Save Converter links

#### **Updates** <a href="#updates-17" id="updates-17"></a>

* Added remaining file extensions for all systems supported by the Genesis Plus GX core

## <mark style="color:orange;">Ignited 1.2.7</mark> <a href="#id-127---4152023" id="id-127---4152023"></a>

<mark style="color:orange;">4/15/2023</mark>

#### **New Features** <a href="#new-features-16" id="new-features-16"></a>

* Added options to toggle game artwork borders, shadows, and rounded corners

#### **Updates** <a href="#updates-18" id="updates-18"></a>

* Added confirmation popup to advanced settings
* Game screenshots are now scaled up by 5x before being saved

## <mark style="color:orange;">Ignited 1.2.6</mark> <a href="#id-126---4142023" id="id-126---4142023"></a>

<mark style="color:orange;">4/14/2023</mark>

#### **New Features** <a href="#new-features-17" id="new-features-17"></a>

* Game Screenshots - save a screenshot of the game screen to your photos with a pause menu item or controller skin button

## <mark style="color:orange;">Ignited 1.2.5</mark> <a href="#id-125---4122023" id="id-125---4122023"></a>

<mark style="color:orange;">4/12/2023</mark>

#### **Bugfixes** <a href="#bugfixes-17" id="bugfixes-17"></a>

* Fixed importing game saves with auto-load save state enabled

#### **New Features** <a href="#new-features-18" id="new-features-18"></a>

* Added advanced setting to clear auto save states from every game

## <mark style="color:orange;">Ignited 1.2.4</mark> <a href="#id-124---4112023" id="id-124---4112023"></a>

<mark style="color:orange;">4/11/2023</mark>

#### **Bugfixes** <a href="#bugfixes-18" id="bugfixes-18"></a>

* Disabled auto-load save on DSi Home Screen
* Removed cheats, save, load, and rewind pause menu items from DSi Home Screen
* Removed cheats from DS Home Screen

## <mark style="color:orange;">Ignited 1.2.3</mark> <a href="#id-123---4102023" id="id-123---4102023"></a>

<mark style="color:orange;">4/10/2023</mark>

#### **New Features** <a href="#new-features-19" id="new-features-19"></a>

* Updates screen will now be shown once per update at launch

#### **Updates** <a href="#updates-19" id="updates-19"></a>

* Updates screen now includes dates for all versions

## <mark style="color:orange;">Ignited 1.2.2</mark> <a href="#id-122---492023" id="id-122---492023"></a>

<mark style="color:orange;">4/9/2023</mark>

#### **New Features** <a href="#new-features-20" id="new-features-20"></a>

* Game Volume - Change the game volume relative to your device volume
* Toggle for whether game audio should play when other audio is playing in the background

#### **Updates** <a href="#updates-20" id="updates-20"></a>

* Updated OpenVGDB database

## <mark style="color:orange;">Ignited 1.2.1</mark> <a href="#id-121---492023" id="id-121---492023"></a>

<mark style="color:orange;">4/9/2023</mark>

#### **New Features** <a href="#new-features-21" id="new-features-21"></a>

* Audio Button Feedback - option to play a sound when a controller skin input is pressed

#### **Updates** <a href="#updates-21" id="updates-21"></a>

* Raise minimum iOS to 14.0 - Removed all legacy code

#### **Bugfixes** <a href="#bugfixes-19" id="bugfixes-19"></a>

* Fixed laggy sliders in settings that could crash the app when paused

## <mark style="color:orange;">Ignited 1.2</mark> <a href="#id-120---482023" id="id-120---482023"></a>

<mark style="color:orange;">4/8/2023</mark>

#### **New Features** <a href="#new-features-22" id="new-features-22"></a>

* Touch Overlays - Get visual feedback about what buttons are currently pressed
* Options for size, opacity, and color of touch overlays
* Resume Button added to game collection screen beside the page dots

#### **Bugfixes** <a href="#bugfixes-20" id="bugfixes-20"></a>

* Fixed controller skins losing transparency on device rotation

## <mark style="color:orange;">Ignited 1.1.4</mark> <a href="#id-114---462023" id="id-114---462023"></a>

<mark style="color:orange;">4/6/2023</mark>

#### **New Features** <a href="#new-features-23" id="new-features-23"></a>

* Re-enabled Save State Rewind - Disabled on GBC to prevent crashes with gambette

#### **Updates** <a href="#updates-22" id="updates-22"></a>

* Added new Advanced section to settings - Moved alt skin and debug toggles there
* Custom fast forward speed is now default - Toggle removed

#### **Bugfixes** <a href="#bugfixes-21" id="bugfixes-21"></a>

* Fixed the Show with Controller settings not working on DS

## <mark style="color:orange;">Ignited 1.1.3</mark> <a href="#id-113---452023" id="id-113---452023"></a>

<mark style="color:orange;">4/5/2023</mark>

#### **New Features** <a href="#new-features-24" id="new-features-24"></a>

* Added option for clicky haptic feedback - A more rigid haptic impulse will be sent on both button press and release
* Added slider for haptic feedback strength

## <mark style="color:orange;">Ignited 1.1.2</mark> <a href="#id-112---422023" id="id-112---422023"></a>

<mark style="color:orange;">4/2/2023</mark>

#### **WARNING** <a href="#warning" id="warning"></a>

This update uses a new bundleID with my domain. It will never change again after this point. Installing will not overwrite your old app. You will need to use Sync or manually transfer data to the new app.

#### **New Features** <a href="#new-features-25" id="new-features-25"></a>

* Made auto save states syncable

#### **Updates** <a href="#updates-23" id="updates-23"></a>

* Made the restart game button available to skins and controllers
* Made the current game highlighting stand out more

#### **Bugfixes** <a href="#bugfixes-22" id="bugfixes-22"></a>

* Fixed last unthemed elements buried in settings

## <mark style="color:orange;">Ignited 1.1.1</mark> <a href="#id-111---422023" id="id-111---422023"></a>

<mark style="color:orange;">4/2/2023</mark>

#### **Changes** <a href="#changes" id="changes"></a>

* Updated toast notification logic to prevent multiple toasts being shown at once

## <mark style="color:orange;">Ignited 1.1</mark> <a href="#id-110---412023" id="id-110---412023"></a>

<mark style="color:orange;">4/1/2023</mark>

#### **New Features** <a href="#new-features-26" id="new-features-26"></a>

* Added a toggle to automatically load the last auto save when launching a game
* Added toggle to enabled/disabled in-game toast notifications

#### **Updates** <a href="#updates-24" id="updates-24"></a>

* Removed the Resume Game prompt from the game selection screen
* Added a Restart Game pause menu button

## <mark style="color:orange;">Ignited 1.0.2</mark> <a href="#id-102---412023" id="id-102---412023"></a>

<mark style="color:orange;">4/1/2023</mark>

#### **New Features** <a href="#new-features-27" id="new-features-27"></a>

* Added theme colored highlighting to currently running game’s artwork

#### **Updates** <a href="#updates-25" id="updates-25"></a>

* Make artwork spacing dynamic like size

#### **Bugfixes** <a href="#bugfixes-23" id="bugfixes-23"></a>

* Fixed some artwork bugs caused by resizing

## <mark style="color:orange;">Ignited 1.0.1</mark> <a href="#id-101---3302023" id="id-101---3302023"></a>

<mark style="color:orange;">3/30/2023</mark>

#### **Bugfixes** <a href="#bugfixes-24" id="bugfixes-24"></a>

* Fixed link in settings

## <mark style="color:orange;">Ignited 1.0</mark> <a href="#id-100---3302023" id="id-100---3302023"></a>

<mark style="color:orange;">3/30/2023</mark>

#### **New Features** <a href="#new-features-28" id="new-features-28"></a>

* Theming - Choose from a variety of colors to change the tint and app icon of Ignited. Emulate in your own style!

#### **UI Updates** <a href="#ui-updates" id="ui-updates"></a>

* Album artwork now has rounded corners, contrasting borders, and a drop shadow
* Can now change the artwork size between small, medium, and large
* Default box-art now features the cartridge of their respective system

#### **Changes** <a href="#changes-1" id="changes-1"></a>

* Custom fast-forward is enabled by default
* Default speed changed to 4x
* Removed 4x from unsafe speeds

## <mark style="color:orange;">Ignited 0.7.1</mark> <a href="#id-071---3192023" id="id-071---3192023"></a>

<mark style="color:orange;">3/19/2023</mark>

#### **Changes** <a href="#changes-2" id="changes-2"></a>

* Alternate Skin pause menu item now only shows is the current skin supports it
* Debug Mode pause menu item now only shows if the current skin’s debug property is set to true, or debug mode is manually enabled in settings
* Reordered save state menu sections. General at the top and Quick/Auto at the bottom
* Rebrand to from Delta Ignited to just Ignited

## <mark style="color:orange;">Ignited 0.7</mark> <a href="#id-070---3182023" id="id-070---3182023"></a>

<mark style="color:orange;">3/18/2023</mark>

#### **New Features** <a href="#new-features-29" id="new-features-29"></a>

* Alt Skins - An alternate skin appearance that can be swapped to from a skin or menu item. Allows for a wide range of implementations. Any feature that boils down to switching something on a skin can be achieved using this new feature, including: DS screen swapping, toggle-able screen filters, cosmetics like a power/charging light, and more.
* Toast Notifications - You will now receive short in-game popups when you save, load, or toggle something. Play with confidence knowing Ignited did what you asked it to.
* Always Show Skin Toggle - You now have the option to always show the skin image, even when a controller connected
* In-App Debug Toggle - You no longer have to edit the debug setting in a controller skin, the option is now available in both the settings and the pause menu

#### **Changes** <a href="#changes-3" id="changes-3"></a>

* Updated footer descriptions for `Controller Skin Options` and `Fast Forward` sections in settings
* Added `Alternate Skin` and `Debug Mode` pause menu items

#### **Bugfixes** <a href="#bugfixes-25" id="bugfixes-25"></a>

* Fixed a bug where the user preferred DS core was changed to MelonDS every time the app started

## <mark style="color:orange;">Ignited 0.6.3</mark> <a href="#id-063---3112023" id="id-063---3112023"></a>

<mark style="color:orange;">3/11/2023</mark>

#### **New Features** <a href="#new-features-30" id="new-features-30"></a>

* Access custom fast forward speeds from in-game menu and skin buttons

#### **Updates** <a href="#updates-26" id="updates-26"></a>

* Make users accept a warning prompt to access 4x and faster speeds
* Add 150% speed setting
* Game will auto-save on every fast forward activation
* Number of auto-saves increased from 2 to 4

## <mark style="color:orange;">Ignited 0.6.2</mark> <a href="#id-062---352023" id="id-062---352023"></a>

<mark style="color:orange;">3/5/2023</mark>

#### **New Features** <a href="#new-features-31" id="new-features-31"></a>

* Allow patrons to install and update the app from safari

#### **Updates** <a href="#updates-27" id="updates-27"></a>

* Fix controller skin previews not showing for standard size iPhones

## <mark style="color:orange;">Ignited 0.6.1</mark> <a href="#id-061---342023" id="id-061---342023"></a>

<mark style="color:orange;">3/4/2023</mark>

#### **Updates** <a href="#updates-28" id="updates-28"></a>

* Change formatting of updates screen
* Move updates to its own section in settings

## <mark style="color:orange;">Ignited 0.6</mark> <a href="#id-060---332023" id="id-060---332023"></a>

<mark style="color:orange;">3/3/2023</mark>

#### **New Features** <a href="#new-features-32" id="new-features-32"></a>

* Add in-app updates changelog

## <mark style="color:orange;">Ignited 0.5.3</mark> <a href="#id-053---332023" id="id-053---332023"></a>

<mark style="color:orange;">3/3/2023</mark>

#### **Updates** <a href="#updates-29" id="updates-29"></a>

* Update local multiplayer controller settings logic
* Remove rewind feature due to crashes

## <mark style="color:orange;">Ignited 0.5.2</mark> <a href="#id-052---2262023" id="id-052---2262023"></a>

<mark style="color:orange;">2/26/2023</mark>

#### **Updates** <a href="#updates-30" id="updates-30"></a>

* Added new GBC skin with matching style and previews

## <mark style="color:orange;">Ignited 0.5.1</mark> <a href="#id-051---2252023" id="id-051---2252023"></a>

<mark style="color:orange;">2/25/2023</mark>

#### **Updates** <a href="#updates-31" id="updates-31"></a>

* Implemented new preview feature in default GBA skin

## <mark style="color:orange;">Ignited 0.5</mark> <a href="#id-050---2252023" id="id-050---2252023"></a>

<mark style="color:orange;">2/25/2023</mark>

#### **New Features** <a href="#new-features-33" id="new-features-33"></a>

* Controller skin previews in settings

## <mark style="color:orange;">Ignited 0.4.1</mark> <a href="#id-041---2252023" id="id-041---2252023"></a>

<mark style="color:orange;">2/25/2023</mark>

#### **Updates** <a href="#updates-32" id="updates-32"></a>

* Made the custom fast forward speed popup pretty and informative
* Fixed crashes on iPad related to popups
* Fixed a crash in P2-P4 controller settings pages

## <mark style="color:orange;">Ignited 0.4</mark> <a href="#id-040---2242023" id="id-040---2242023"></a>

<mark style="color:orange;">2/24/2023</mark>

#### **New Features** <a href="#new-features-34" id="new-features-34"></a>

* Custom fast forward speed setting and toggle

## <mark style="color:orange;">Ignited 0.3</mark> <a href="#id-030---2232023" id="id-030---2232023"></a>

<mark style="color:orange;">2/23/2023</mark>

#### **New Features** <a href="#new-features-35" id="new-features-35"></a>

* Links to skin download sites added to settings
* Inset and rounded settings tables

#### **Updates** <a href="#updates-33" id="updates-33"></a>

* Ensured all settings sections have a descriptive footer

## <mark style="color:orange;">Ignited 0.2.1</mark> <a href="#id-021---2212023" id="id-021---2212023"></a>

<mark style="color:orange;">2/21/2023</mark>

#### **New Features** <a href="#new-features-36" id="new-features-36"></a>

* Genesis core made available

#### **Updates** <a href="#updates-34" id="updates-34"></a>

* Genesis file extension fix
* Remove all beta checks
* Contributors page updated

## <mark style="color:orange;">Ignited 0.2</mark> <a href="#id-020---2202023" id="id-020---2202023"></a>

<mark style="color:orange;">2/20/2023</mark>

#### **New Features** <a href="#new-features-37" id="new-features-37"></a>

* Extended MFi Controller Support
* Save State Rewind
* Local Multiplayer

#### **Updates** <a href="#updates-35" id="updates-35"></a>

* Contributors page updated
* Update links in settings

## <mark style="color:orange;">Ignited 0.1</mark> <a href="#id-010---2192023" id="id-010---2192023"></a>

<mark style="color:orange;">2/19/2023</mark>

#### **New Assets** <a href="#new-assets" id="new-assets"></a>

* App Icon
* Box Art
* DS Home Icon
* Launch Screen
* GBA Controller Skin
