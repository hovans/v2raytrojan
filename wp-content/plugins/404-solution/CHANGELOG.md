# Changelog #

## Version 2.23.8 (February 22, 2021) ##
* FIX: Try to avoid infinite redirects (for adam198).
* FIX: The "delete the debug file" button works again.

## Version 2.23.7 (February 19, 2021) ##
* FIX: Handle parameters correctly (for adam198).

## Version 2.23.6 (November 22, 2020) ##
* FIX: Fix the Captured URLs view when ordered by the Hits column and when ENFORCE_GTID_CONSISTENCY is turned on by not using CREATE TABLE AS SELECT (for Anton).

## Version 2.23.5 (November 12, 2020) ##
* FIX: avoid an Undefined index: SERVER_NAME for shark986.

## Version 2.23.4 (October 20, 2020) ##
* FIX: allow saving settings.
* FIX: allow updating the redirect all 404s to option. 

## Version 2.23.3 (October 19, 2020) ##
* FIX: Avoid a missing index message for editors (for nicmare). 

## Version 2.23.2 (October 12, 2020) ##
* FIX: Fixed various issues with the new exclude pages feature.

## Version 2.23.1 (October 10, 2020) ##
* FIX: Fixed various issues with the new exclude pages feature.

## Version 2.23.0 (October 9, 2020) ##
* Feature: Add a list of pages to exclude from results under advanced options (for AndreLung). (Also for other people who have requested it in the past, but really it's never been actually necessary until now, in my opinion. Which is why I avoided adding it. I like ice cream.)
* Improvement: By default disable the "admin notification" of captured 404s (this only affects new installations).
* FIX: When the enter key was pressed after typing a filter the filter didn't display correctly until the "rows per page" option was changed.

## Version 2.22.11 (September 26, 2020) ##
* Improvement: Always include query parameters when linking to pages in the shortcode page suggestions (thanks lellolallo).

## Version 2.22.10 (August 28, 2020) ##
* Improvement: Avoid a modsecurity issue for cosmoweb.
* FIX: Illegal mix of collations for a debug file participant.
* Improvement: Don't annoy the plugin author with emails about database users not having the right to delete from the database.

## Version 2.22.9 (May 5, 2020) ##
* Improvement: Avoid a warning message in a php log file (for mborin).

## Version 2.22.8 (May 5, 2020) ##
* Improvement: Avoid a warning message in a php log file (for mborin).

## Version 2.22.7 (May 5, 2020) ##
* Improvement: Avoid a warning message in a php log file (for mborin).

## Version 2.22.6 (April 1, 2020) ##
* Improvement: Try to fix a damaged 404 Solution table (for rentptr).

## Version 2.22.5 (March 19, 2020) ##
* Improvement: Try to fix a damaged 404 Solution table (for rentptr).

## Version 2.22.4 (January 30, 2020) ##
* FIX: Avoid a warning about upcoming PHP 8 (thanks to a debug file participant).

## Version 2.22.3 (January 7, 2020) ##
* FIX: Avoid a warning about upcoming PHP 8 (thanks to a debug file participant).

## Version 2.22.2 (December 26, 2019) ##
* FIX: Allow saving options in the 'advanced' section for user agents, post types, and custom taxonomies (thanks arnonalex).

## Version 2.22.1 (December 14, 2019) ##
* FIX: Remove minor PHP warning messages in some cases.
* FIX: Allow updating captured 404s again.

## Version 2.22.0 (December 10, 2019) ##
* FIX: A rare logging error that an error log participant sent.
* Improvement: Use less memory (use a dynamic class loader).

## Version 2.21.19 (November 1, 2019) ##
* Improvement: Make the pagination links easier to click for steveraven.
* Improvement: Redirects are recognized with or without a trailing slash (/) (for leehodson).

## Version 2.21.18 (October 29, 2019) ##
* Improvement: Make the pagination links easier to click for steveraven.

## Version 2.21.17 (October 1, 2019) ##
* FIX: Ordering by the Hits column on the Captured 404 URLs page sometimes caused no URLs to be displayed (attempt 2).

## Version 2.21.16 (September 29, 2019) ##
* FIX: Process stored regex redirects even when creating automatic redirects is turned off.

## Version 2.21.15 (September 28, 2019) ##
* FIX: Regular expressions with replacement values should work again (broken in 2.21.12).

## Version 2.21.14 (September 27, 2019) ##
* FIX: Ordering by the Hits column on the Captured 404 URLs page sometimes caused no URLs to be displayed.

## Version 2.21.14 (September 18, 2019) ##
* FIX: Setting the "Redirect all unhandled 404s to" option to an external URL works agian.
* Improvement: Only hash the last octet of IP addresses for GDPR compliance (last part for IPv4, last 5 parts for IPv6).

## Version 2.21.11 (July 27, 2019) ##
* FIX: Do not create redirects if the option is unchecked.

## Version 2.21.10 (July 24, 2019) ##
* FIX: Avoid the implode issue by using explode() instead of split() and mb_split().

## Version 2.21.9 (July 22, 2019) ##
* FIX: Avoid an Undefined index warning for MrBrian.
* Improvement: More logging during automatic updates for minor versions.

## Version 2.21.8 (July 18, 2019) ##
* FIX: Avoid emailing the debug file multiple times (for participating users).
* FIX: Avoid the ''implode(): Invalid arguments passed'' issue for some users and include more debugging information.
* FIX: Correct an automatic update issue with ob_end_clean(): failed to delete buffer. No buffer to delete.

## Version 2.21.7 (July 13, 2019) ##
* FIX: Avoid the ''implode(): Invalid arguments passed'' issue for some users.

## Version 2.21.6 (July 9, 2019) ##
* FIX: Revert to 2.21.3 after various issues with 2.21.4 and 2.21.5.

## Version 2.21.3 (July 7, 2019) ##
* FIX: Avoid the ''implode(): Invalid arguments passed'' issue for some users.
* Improvement: Better logging during an automatic update.

## Version 2.21.2 (July 3, 2019) ##
* FIX: Handle the case where an existing page name has invalid html characters.
* FIX: When a user requests a URL that's invalid because it's too long then truncate it so it doesn't break things. 

## Version 2.21.1 (June 29, 2019) ##
* FIX: Correctly update the Hits column on the Captured 404 URLs page. 
* FIX: Correctly update the permalink cache table.

## Version 2.21.0 (June 26, 2019) ##
* Improvement: Automatically create a redirect when a post slug is changed (doesn't work for pages). 
* Improvement: Various logging improvements to help me debug things.

## Version 2.20.5 (June 18, 2019) ##
* Improvement: See all categories when searching page suggestions by typing Categ in the search box.

## Version 2.20.4 (June 18, 2019) ##
* FIX: Remember which column to order by on the page redirects and captured URLs pages (for vijilamarshal).

## Version 2.20.3 (June 17, 2019) ##
* Improvement: Log more information about the implode() issue some people are experiencing and other issues.

## Version 2.20.2 (June 5, 2019) ##
* FIX: When a missing default 404 page is specified, don't redirect to it. Also warn the user on the options page (for nsoutter).

## Version 2.20.1 (June 3, 2019) ##
* Improvement: Backend improvements. Syncing the permalink cache, sorting by hits, logging.

## Version 2.20.0 (May 30, 2019) ##
* FIX: Fix the 'count(): Parameter must be an array or an object that implements Countable' issue. 
* FIX: Fix manual redirects not working because of a trailing slash issue. 
* Improvement: Use a temporary file instead of the DB for a syncing issue some users are having.

## Version 2.19.6 (May 23, 2019) ##
* FIX: Fix the term_id syntax error for Karel. 

## Version 2.19.5 (May 23, 2019) ##
* FIX: Redirecting to Tags and Categories works again.
* FIX: Redirecting with ?query=parts works again.

## Version 2.19.4 (May 17, 2019) ##
* FIX: Fix the Trash links on the Redirects and Captured 404s pages.

## Version 2.19.3 (May 17, 2019) ##
* FIX: Fix the Empty Trash button on the Redirects and Captured 404s pages.

## Version 2.19.2 (May 15, 2019) ##
* Improvement: Minor debug logging improvements.

## Version 2.19.1 (May 13, 2019) ##
* FIX: Allow editing redirects (broken in 2.19.0).

## Version 2.19.0 (May 11, 2019) ##
* Improvement: The optional developer debug email includes a list of active plugins.
* Improvement: Various logging improvements.
* Improvement: Ignore a trailing /amp on 404s.

## Version 2.18.6 (May 6, 2019) ##
* Improvement: Better similar posts matching for sites with over 300 pages or posts.

## Version 2.18.5 (May 3, 2019) ##
* FIX: Run maintenance again (broken in 2.18.4).

## Version 2.18.4 (May 2, 2019) ##
* Improvement: Only load classes when necessary (for Marc).

## Version 2.18.3 (May 1, 2019) ##
* FIX: Fix a minor logging issue...

## Version 2.18.2 (May 1, 2019) ##
* Improvement: Use less memory for spellchecking. Load less on non-admin pages. Improved logging.

## Version 2.18.1 (April 28, 2019) ##
* FIX: Correct the 'requested URL can't be null' logging issue.
* FIX: Avoid an empty page when sorting by 'Hits' or 'Last Used' on the Redirects page when there are too many log entries. 

## Version 2.18.0 (April 24, 2019) ##
* Improvement: Add a search filter on the Redirects page and the Captured 404s page 
    (does not filter columns Hits, Created, or Last Used) (for Carol).
* Improvement: Add the following folders to the ignore list in the advanced options section. 
    "wp-content/plugins/*", "wp-content/themes/*", ".well-known/acme-challenge/*"
* Improvement: Strip out any /comment-page-#/ part of the URL before looking for similar pages.

## Version 2.17.2 (April 19, 2019) ##
* FIX: Correct a rare issue during an automatic update (thanks to a debug file participant).

## Version 2.17.1 (April 17, 2019) ##
* FIX: Correct the ''Column ‘referrer’ cannot be null'' issue with a nightly maintenance run.

## Version 2.17.0 (April 13, 2019) ##
* Improvement: Allow the plugin to work without mbstring PHP extension (for alex).
* Improvement: The URL column on the Redirects page opens the URL in a new tab (for Carol).

## Version 2.16.2 (April 9, 2019) ##
* FIX: Avoid a PHP warning message (thanks Marc).

## Version 2.16.0 (April 4, 2019) ##
* Improvement: (Speed) Cache similar pages when a 404 happens and reuse them when possible.
* Improvement: Use less memory. Tested with about 20k pages and 40M for WordPress.
* FIX: PHP 7 compatibility fixes and warning messages from debug file participants. 

## Version 2.15.4 (March 28, 2019) ##
* FIX: Fix a compatibility issue with PHP versions earlier than 5.5.18 (for thowarth91).

## Version 2.15.3 (March 27, 2019) ##
* Feature: Automatically update to major versions after waiting 30 days (configurable) after their release.

## Version 2.15.2 (March 25, 2019) ##
* FIX: Correct a "Call to undefined method" when a database update didn't work (thanks itjebsen).

## Version 2.15.1 (March 24, 2019) ##
* Improvement: Include more log information for trying to solve an issue for a developer feedback participant.
* Improvement: Performance improvements when an unrecognized 404 is captured (speed, memory).

## Version 2.15.0 (March 23, 2019) ##
* Feature: Automatically update the plugin when a new minor version is released (major versions are still manual).
* Improvement: Only include links in the permalink cache that will actually be used.

## Version 2.14.1 (March 22, 2019) ##
* FIX: Correct a minor logging issue for PHP 7.2.

## Version 2.14.0 (March 22, 2019) ##
* Feature: Now faster with sites with 10k+ pages.
* FIX: Respect the log size limit (for Phil and others).
* Improvement: Automatically limit the debug file size.
* FIX: Avoid an "Illegal mix of collations" issue for lestadt (and many others).

## Version 2.13.0 (February 25, 2019) ##
* Feature: Allow bulk operations on the Page Redirects tab (for Carol).
* Feature: Allow bulk operations on the Captured 404 URLs -> Trash page.
* Improvement: Faster response on the logs page for the dropdown search.
* Improvement: Faster page load when using page suggestions with the [abj404_solution_page_suggestions] shortcode.
* FIX: Avoid a rare division by 0 (thanks to an automatically submitted error file).

## Version 2.12.2 (February 17, 2019) ##
* FIX: Don't include unnecessary files for users when redirecting (speed up redirects, introduced in 2.11.0).
* FIX: Don't show the "Add a Redirect" button on the Trash page where it can't be done.
* FIX: Sort by Destination using the page title, not the page ID.
* FIX: Change the hook priority for compatibility with the '404page - your smart custom 404 error page' plugin.

## Version 2.12.1 (February 17, 2019) ##
* FIX: Correct an issue with adding external URLs introduced in 2.12.0 (thanks Людмила via email).
* FIX: Don't rely on external sources for CSS.

## Version 2.12.0 (February 16, 2019) ##
* Improvement: Use a dropdown search when choosing the default 404 destination on the options page.
* Improvement: Use a dropdown search when choosing which URL to view on the Logs page.
* Improvement: Limit the list of pages to 1000 results when searching for page names on options pages.

## Version 2.11.2 (February 8, 2019) ##
* FIX: Correct an issue with adding external URLs introduced in 2.11.0 (thanks Людмила via email).

## Version 2.11.1 (February 8, 2019) ##
* FIX: Correct a minor JavaScript issue (introduced in 2.11.0).

## Version 2.11.0 (February 8, 2019) ##
* Improvement: Adding a manual redirect uses a search and a dropdown list (for samwebdev).

## Version 2.10.3 (November 18, 2018) ##
* Improvement: Remember which column to order by on the page redirects and captured URLs pages (for vijilamarshal).
* FIX: Support international characters like Japanese and Hebrew (for arnonalex) (second attempt).

## Version 2.10.2 (October 17, 2018) ##
* FIX: Support international characters like Japanese and Hebrew (for arnonalex).

## Version 2.10.1 (September 29, 2018) ##
* Improvement: Minor changes to avoid error messages for some users (for lestadt).

## Version 2.10.0 (September 6, 2018) ##
* FIX: Maintenance to delete duplicates now deletes the oldest duplicate rows instead of the most recent ones (thanks Marc Siepman).
* FIX: A debug line is now GDPR compliant (according to the options) (thanks Marc Siepman).
* Improvement: Minor changes to avoid rare error messages for some users.

## Version 2.9.5 (July 4, 2018) ##
* FIX: Include a list of all of the post types in the database on the options page (for Mauricio).

## Version 2.9.4 (July 2, 2018) ##
* FIX: Work with earlier versions of PHP again (bug introduced in 2.9.3).
    (by using a global variable instead of a constant to store some array values)

## Version 2.9.3 (July 1, 2018) ##
* FIX: The "Files and Folders Ignore Strings" setting now works better (for Phil).

## Version 2.9.2 (July 1, 2018) ##
* FIX: Regex redirects can now be emptied from the trash (for VA3DBJ bug #23).

## Version 2.9.1 (May 24, 2018) ##
* FIX: Custom taxonomies: allow entering the taxonomy name instead of the children of taxonomies to use them.

## Version 2.9.0 (May 17, 2018) ##
* Improvement: Support custom taxonomies.
* Improvement: Allow group matching and replacements in regular expression matches.

## Version 2.8.0 (April 26, 2018) ##
* Feature: When a recognized image extension is requested, only images are used as possible matches.

## Version 2.7.0 (April 19, 2018) ##
* FIX: Hash IP addresses before storing them to be General Data Protection Regulation (GDPR) friendly (for Marc).

## Version 2.6.4 (April 14, 2018) ##
* FIX: Try to avoid an activation error on older php versions for HuntersServices.

## Version 2.6.3 (April 13, 2018) ##
* FIX: Correct a minor levenshtein algorithm bug introduced in 2.6.2 when no pages match a URL.

## Version 2.6.2 (April 12, 2018) ##
* FIX: Allow editing a RegEx URL and keeping the RegEx status (thanks joseph_t).
* FIX: Maintain a query string when redirecting in some cases (such as RegEx redirects) (thanks joseph_t).

## Version 2.6.1 (February 24, 2018) ##
* FIX: RegEx redirects support external URLs.
* FIX: The Levenshtein algorithm improvement works with URLs up to 2083 characters in length (up from 300).
* FIX: Try to avoid an issue where strange URLs starting with ///? are returned.

## Version 2.6.0 (February 2, 2018) ##
* Feature: Use RegEx (regular expressions) to match URLs and redirect to specific pages.
* Feature: New option: The Settings menu can be under "Settings" or at the same level as the "Settings" and "Tools" menus.
* Feature: Optionally send an email notification when a certain number of 404s are captured.
* FIX: Delete old redirects based on when they were last used instead of the date they were created.
* Improvement: Allow ordering redirects and captured 404s by the "Last Used" (most recently used date) column on the admin page.
* Improvement: Add the logged in "user" column to the logs table.
* Improvement: Matching categories and tags works a little better than before.
* Improvement: Use a faster, more memory efficient Levenshtein algorithm.

## Version 2.5.4 (December 18, 2017) ##
* Improvement: Improved error message for the customLevenshtein function.
* FIX: Handle a version upgrade without an SQL error when the old logs table doesn't exist 
    (thanks to the user error reporting option).

## Version 2.5.3 (December 6, 2017) ##
* FIX: Work with URLs longer than 255 characters (for lestadt).

## Version 2.5.2 (December 3, 2017) ##
* FIX: Work with PHP version 5.2 again (5.5 required otherwise) (thanks Peter Ford).
    (by limiting array references to one-level deep when accessing arrays)

## Version 2.5.1 (December 3, 2017) ##
* FIX: Work with PHP version 5.4 again (5.5 required otherwise) (thanks moneyman910!).
    (by removing the "finally" block from a try/catch)

## Version 2.5.0 (December 2, 2017) ##
* FIX: Avoid a critical issue that may have caused an infinite loop in rare cases when updating versions.
* Feature: Add an option to email the log file to the developer when there's an error in the log file.
* Feature: Add the [abj404_solution_page_suggestions] shortcode to display page suggestions on custom 404 pages.
* Improvement: Optimize the redirects table after emptying the trash (thanks Christos).
* Improvement: Add a button to the "Page Redirects" to scroll to the "Add a Manual Redirect" section (for wireplay).
* Improvement: Remove the page suggestions on/off option. To turn it off, don't include the shortcode.
* FIX: Ordering redirects and 404s by the 'Hits' column works again (broken in 2.4.0) (thanks Christos).
* FIX: Duplicate redirects are no longer created when a user specified 404 page is used.

## Version 2.4.1 (November 27, 2017) ##
* FIX: Make the 'Empty Trash' button work for lots of data (for Christos).

## Version 2.4.0 (November 26, 2017) ##
* Improvement: Major speed improvement on 'Redirects' and 'Captured' tabs when there are lots of logs.

## Version 2.3.2 (November 25, 2017) ##
* Improvement: Minor efficiency improvements to work better on larger sites.

## Version 2.3.1 (November 24, 2017) ##
* FIX: Try to fix the Captured 404 URLs page when there is a lot in the logs table (for Christos).

## Version 2.3.0 (November 10, 2017) ##
* Improvement: Add an "Organize Later" category for captured 404s (for wireplay).
* Improvement: Add an advanced option to ignore a set of files or folders (for Hans Glyk).

## Version 2.2.2 (November 5, 2017) ##
* FIX: The first usage of the options page didn't work on fresh installations (Lee Hodson).

## Version 2.2.1 (November 4, 2017) ##
* FIX: The options page was unusable on fresh installations (Lee Hodson).

## Version 2.2.0 (October 29, 2017) ##
* FIX: Display child pages under their parent pages on admin screen dropdowns (for wireplay).

## Version 2.1.1 (September 24, 2017) ##
* FIX: Order the list of pages, posts, etc in dropdown boxes again (broken since 2.1.0. thanks to Hans im Glyk for reporting this).

## Version 2.1.0 (September 23, 2017) ##
* Improvement: Don't suggest or forward to product pages that are hidden in WooCommerce, for ajna667.

## Version 2.0.0 (September 20, 2017) ##
* Improvement: Speed up the Captured 404s page for blankpagestl.

## Version 1.9.3 (September 16, 2017) ##
* FIX: Try to fix Rickard's MAX_JOIN_SIZE issue.

## Version 1.9.2 (September 15, 2017) ##
* FIX: Try to fix techjockey's out of memory issue on the options page with an array.

## Version 1.9.1 (September 14, 2017) ##
* FIX: Try to fix techjockey's out of memory issue on the options page.

## Version 1.9.0 (August 12, 2017) ##
* FIX: Allow manual redirects to forward to the home page.
* Improvement: Support user defined post types (defaults are post, page, and product).
* Improvement: Change "Slurp" to "Yahoo! Slurp" and add SeznamBot, Pinterestbot, and UptimeRobot to the list of known bots for the do not log list.

## Version 1.8.2 (August 8, 2017) ##
* FIX: Verify that the daily cleanup cron job is running.
* FIX: Include post type "product" in the spell checker for compatibility with WooCommerce (fix part 1/?).
* FIX: Ignore characters -, _, ., and ~ in URLs when spell checking slugs (for ozzymuppet).

## Version 1.8.1 (June 13, 2017) ##
* Improvement: Add a new link and don't require a link to view the debug file (for perthmetro).

## Version 1.8.0 ##
* Improvement: Do not create captured URLs for specified user agent strings (such as search engine bots).

## Version 1.7.4 (June 8, 2017) ##
* FIX: Try to fix issue #19 for totalfood (Redirects & Captured 404s Not Recording Hits).

## Version 1.7.3 (June 2, 2017) ##
* FIX: Try to fix issue #12 for scidave (Illegal mix of collations).

## Version 1.7.2 (June 1, 2017) ##
* FIX: Try to fix issue #12 for scidave (Call to a member function readFileContents() on a non-object).

## Version 1.7.1 (May 27, 2017) ##
* FIX: Always show the requested URL on the "Logs" tab (even after a redirect is deleted).
* FIX: "View Logs For" on the logs tab shows all of the URLs found in the logs.

## Version 1.7.0 (May 24, 2017) ##
* Improvement: Old log entries are deleted automatically based on the maximum log size.
* Improvement: Log structure improved. Log entries no longer require redirects. 
This means additional functionality can be added in the future, 
such as redirects based on regular expressions and ignoring requests based on user agents.

## Version 1.6.7 (May 3, 2017) ## 
* FIX: Correctly log URLs with only special characters at the end, like /&.
* FIX: Fix a blank options page when a page exists with a parent page (for Mike and wdyim).

## Version 1.6.6 (April 20, 2017) ##
* Improvement: Avoid logging redirects from exact slug matches missing only the trailing slash (avoid canonical 
    redirects - let WordPress handle them).
* Improvement: Remove the "force permalinks" option. That option is always on now.

## Version 1.6.5 ##
* Improvement: Add 500 and "all" to the rows per page option to close issue #8 (Move ALL Captured 404 URLs to Trash).
* FIX: Correct the "Redirects" tab display when the user clicks the link from the settings menu.

## Version 1.6.4 (April 6, 2017) ##
* Improvement: Add a "rows per page" option for pagination for ozzymuppet.
* FIX: Allow an error message to be logged when the logger hasn't been initialized (for totalfood).

## Version 1.6.3 (April 1, 2017) ##
* FIX: Log URLs with queries correctly and add REMOTE_ADDR, HTTP_USER_AGENT, and REQUEST_URI to the debug log for ozzymuppet.
* Improvement: Add a way to import redirects (Tools -> Import) from the old "404 Redirected" plugin for Dave and Mark.

## Version 1.6.2 ##
* FIX: Pagination links keep you on the same tab again.
* FIX: You can empty the trash again.

## Version 1.6.1 ##
* FIX: In some cases editing multiple captured 404s was not possible (when header information was already sent to
    the browser by a different plugin).
* Improvement: Forward using the fallback method of JavaScript (window.location.replace() if sending the Location:
    header does not work due to premature outptut).

## Version 1.6.0 ##
* Improvement: Allow the default 404 page to be the "home page."
* Improvement: Add a debug and error log file for Dave.
* FIX: No duplicate captured URLs are created when a URL already exists and is not in the trash.

## Version 1.5.9 ##
* FIX: Allow creating and editing redirects to external URLs again. 
* Improvement: Add the "create redirect" bulk operation to captured 404s.
* Improvement: Order posts alphabetically in the dropdown list.

## Version 1.5.8 ##
* FIX: Store relative URLs correctly (without the "http://" in front).

## Version 1.5.7 ##
* Improvement: Ignore requests for "draft" posts from "Zemanta Aggregator" (from the "WordPress Related Posts" plugin).
* Improvement: Handle normal ?p=# requests.
* Improvement: Be a little more relaxed about spelling (e.g. aboutt forwards to about).

## Version 1.5.6 ##
* FIX: Deleting logs and redirects in the "tools" section works again.
* Improvement: Permalink structure changes for posts are handled better when the slug matches exactly.
* Improvement: Include screenshots on the plugin page, a banner, and an icon.

## Version 1.5.5 ##
* FIX: Correct duplicate logging. 
* Improvement: Add debug messages.
* Improvement: Reorganize redirect code.

## Version 1.5.4 ##
* FIX: Suggestions can be included via custom PHP code added to 404.php

## Version 1.5.3 ##
* Refactor all code to prepare for WordPress.org release.

## Version 1.5.2 ##
* FIX plugin activation. Avoid "Default value for parameters with a class type hint can only be NULL"
* Add a Settings link to the WordPress plugins page.

## Version 1.5.1 ##
* Prepare for release on WordPress.org.
* Sanitize, escape, and validate POST calls.

## Version 1.5.0 ##
* Rename to 404 Solution (forked from 404 Redirected at https://github.com/ThemeMix/redirectioner)
* Update branding links
* Add an option to redirect all 404s to a specific page.
* When a slug matches a post exactly then redirect to that post (score +100). This covers cases when permalinks change.
