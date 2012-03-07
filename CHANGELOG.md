Changelog
=========

Version 2.5 *(in development)*
--------------------------------

Notable changes:

* Database upgrade for better time representation. It may take a few seconds for the database to upgrade.
* Hide individual shows.
* 'Only favorites' option for Upcoming/Recent, also respected by widgets.
* 'Watched all previously aired' option when long-tapping an episode.
* Unified interface across all devices thanks to ActionBarSherlock 4.0.
* Removed middle and large widget on Android 3.0+ devices. Use the new list widget!

Detailed changes:

Since 2.5beta/2.5.1beta (2012-01-13):
 
* Add 'Watched all previously aired' option to episode list of a season.
* Add show posters in Upcoming and Recent.
* Fix to display correct episode title.

Since 2.5.2beta (2012-01-28):

* Better internal representation for time. It may take a while until your shows appear (the database is upgrading in the background). YOU MAY NEED to update all of your shows afterwards. Episodes move now correctly from Upcoming to Recent 1 hour after they aired.

* Hide shows, they will disappear from everywhere except the new 'Hidden' show filter.
* Swipe between episodes on xlarge screens (10 inch tablets) or in landscape, too.
* 'Only favorites' option for Upcoming/Recent, also respected by widget.
* Add menu button to quickly share with last used sharing option.
* Use progress indicators in `AddActivity`.
* Friends layout more similar to Upcoming.
* Use ViewPagerIndicator 2.2.2 release.
* Fixes for the updater.
* Fixes for market reported crashes.
* Cleaner welcome dialog.
* Improvements for descriptions and text everywhere.
* Hide friends tab in Activity if trakt account is not set up.
* Don't use beta icon for stable release (only devices with extra high resolution displays were affected).
* Hide text of some action bar buttons.
* Support for 'Daily' air day.
* Latest translations from crowdin, now with Arabic by mohd55 and Hungarian by devilinside.

Since 2.5.3beta (2012-01-29)

* Updated design towards ICS styles.
* Fix for crash when trying to create a trakt account.
* Use user-specified episode numbers in Upcoming/Recent.
* Fix GetGlue comment box text not wrapping.
* Latest translations from crowdin. Thanks everyone for the big effort!

Since 2.5.4beta (2012-02-17 GMT+1):

* Hide legacy widgets except small size on Android 3.0+ devices.
* Fix incorrect next episodes if two air the same day. The lower numbered one is now assumed to be aired first (though still at the same time).
* Fix sorting and filtering if shows have older episodes listed under next.
* Reduced auto-update interval to at least every 15min.
* New notification icon (finally!).
* Layout tweaks in Upcoming and episode details.
* Hide 'Add to calendar' button if it is useless.
* Use ActionBarSherlock 4.0.
* Display search term, title and search soft button in `SearchActivity`.
* Enabled home button (app icon in the ActionBar) everywhere.
* New welcome and beta dialog.

Since 2.5.5beta (2012-02-20 GMT+1):

* Fix for crash when marking episodes watched.
* Always show the 'Add to calendar' button, if room.
* Fix #53 for episodes list.

Since 2.5.6beta (soon)

* Modify design to be closer to Android Design guidelines.
* Highlight selected item in multi-pane episode view.
* UI for custom upcoming interval (currently 24 hours).
* Posters and no already added shows in Add Show (not for the search screen).
* When adding a show get seen episodes from trakt.
* Download half the data when syncing from trakt via Settings.
* Bigger sized list widget items on xlarge devices. Smaller minimum list widget size, therefore smaller on GoogleTV.
* Fixed stuck progress dialog when checking in with trakt.
* Some other minor improvements.

Version 2.4.2/2.4.3beta *(2012-01-11)*
-------------------------------

* Fix for a crash while updating and fetching trakt activity.
* Fix for wrong show poster displaying in list widget.
* Latest translations from crowdin.

Version 2.4.1 *(2012-01-07)*
-------------------------------

* New list widget for Android 3.0+.
* Remade all widgets sticking to design guidelines, this means they now display 1 (small), 3 (middle) or 7 (large) items and have correct padding.
* Latest translations from crowdin.

Since 2.4.2beta (2012-01-07)

* Tapping list widget items takes you to the respective episode page.
* Tweaked list widget layout a little.
* Made widget backgrounds more transparent.

Since 2.4.1beta (2012-01-06)

* Resizable list widget for Android 3.0+. Uses an alarm to refresh (this needs testing) every 5 mins if the device is awake.
* Remade all widgets sticking to design guidelines, this means they now display 1 (small), 3 (middle) or 7 (large) items and have correct padding.
* Latest translations from crowdin.


Version 2.4 *(2011-12-25)*
--------------------------------

* Check into a show on trakt. After checking in, trakt will automatically display it as watching then switch over to watched status once the runtime of the show has elapsed.
* Recently watched episodes are fetched from trakt on each update: allows easy syncing of devices. After adding a show the initial fetch of watched episodes should still be done via `Settings` >> `Sync with trakt` >> `Sync to SeriesGuide`.
* `Upcoming` renamed `Activity`.

Since 2.3.9beta (2011-12-21):

* Check into a show on trakt. After checking in, trakt will automatically display it as watching then switch over to watched status once the runtime of the show has elapsed.
* Recently watched episodes are fetched from trakt on each update: allows easy syncing of devices. After adding a show the initial fetch of watched episodes should still be done via `Settings` >> `Sync with trakt` >> `Sync to SeriesGuide`. Enabled by default on new installations.
* `Integrate with trakt.tv` now controls the former behaviour. The eye icon does not automatically mark episodes as seen on trakt anymore. Use the check in functionality.
* Auto update enabled by default on new installations (only over WiFi, only on opening the show list, once a day).
* `Upcoming` renamed `Activity`, now includes the latest activity of friends on trakt.
* Optimized for Android 4.0.
* TVDb button in `Overview`.
* Make the backup screen a little more informative.
* Add a welcome dialog to get users started.
* Set auto-update limit to 12 hours (down from 23 hours).
* Use ActionBarSherlock 3.5.0.

Since 2.4beta (2011-12-24):

* Fix text color for notification on Android 2.2 and below.
* Display failed shows in update error message.
* Latest translations from crowdin.net.

Version 2.3 *(2011-11-26)*
--------------------------------

* Revamped updater: shows get outdated after 7 days and get included in the next update
* AutoUpdate: presses the update button on opening the app for you
* Updating now only works on Wi-Fi, this can be disabled in settings
* Revamped adding of shows (incl. more trakt integration)
* Episode pager on phones/small screens
* TVDb buttons

Version 2.2.2 *(2011-11-01)*
--------------------------------

* Fix crash when adding shows on certain HTC devices (Desire HD, Mytouch 4G, ...)

Version 2.2.1 *(2011-10-31)*
--------------------------------

* Fix layouts on small tablet (large screen) devices
* Validate trakt.tv credentials
* Secure the trakt.tv password even better (you will have to reenter it again, sorry)
* Don't rebuild the search table if nothing was updated
* Latest translations from crowdin. Now with Hungarian thanks to devilinside and uw11!

Version 2.2 *(2011-10-18)*
--------------------------------

* Desire HD users: please try updating your phone to the latest firmware
* Filter options for show list (replaces 'Hide watched shows' setting)
* Layout improvements all over the app (spot the differences!), esp. on tablet/Google TV (large+) devices
* Dual pane layout for Upcoming on large+ devices
* Display which show is currently getting updated
* New number format brought to you by dqdb via GitHub
* Latest translations from crowdin
* Many bug fixes, optimizations
* Thanks to everyone who sent in bug reports, suggested improvements or helps translate!

Version 2.1.2 *(2011-10-01)*
--------------------------------

* Use new trakt library release (better error handling)
* New show sorting: favorites by next episode
* Clean up images when deleting a show
* Show first episode of season when using dual-pane layout
* Bugfixes, Improvements

Version 2.1.1 (04.09.2011)
------------------------

* Better user communication when doing delta and full update (now called 'Update All')
* Use TVDB id instead of IMDb id to mark episodes as seen on trakt
* Don't require a touchscreen to use SeriesGuide (upcoming Google TV support)
* Always use a GridLayout for the show list.
* Tidy up settings.
* Change URLs to new website.
* Improvements for DeltaUpdate.
* Latest translations.

Version 2.1 (13.08.2011)
------------------------

* Design updates (incl. usage of ActionBarSherlock)
* Delta-Updates (Full update option remains available)
* Experimental syncing with trakt.tv
* 'Hide watched shows' and 'No special episodes' options brought to you by Jake Wharton (big thanks!)
* Progress bars in season list
* Show trending or your shows on trakt.tv when adding shows
* New 'Favorites first' show sorting, ability to add shows to favorites
* Many other small improvements
* Thanks to all the beta channel users!


Version 2.0.6 (24.07.2011)
--------------------------------

* Fix calculation of air time and day when using time offset (and in general it is now done right)
* Fixes for some crashes reported by Android Market
* If your device is set to GMT-5:00 (US Central) SeriesGuide automagically corrects airtimes by 1 hour


Version 2.0.5 (08.07.2011)
--------------------------------

* using trakt does not require an API key anymore
* Removed languages with little translation (due to user requests)
* Reworded some strings (English only)


Version 2.0.4 (17.06.2011)
--------------------------------

* Fix: Various rare crashes
* Now with two variants of Portuguese


Version 2.0.3 (16.06.2011)
--------------------------------

* Fix: Crash when updating a show failed.
* trakt.tv rating via the share button.
* Latest translations from crowdin.
* Some other rare crash fixes.


Version 2.0.2 (15.06.2011)
--------------------------------

* Fix: Crashes while database ops were running in parallel
* Latest translations from crowdin.


Version 2.0.1 (14.06.2011)
--------------------------------

* Fix: German whats new was missing.


Version 2.0 (14.06.2011)
--------------------------------

* Redesign of UI and backend (try using it in landscape, or on Android 3.0+!).
* New time offset setting.
* Remove single episodes.
* Long-clicking on Back takes you to the show list.
* Dropped support for Android 1.6
* Much more... (see the source changes)
