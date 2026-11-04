=== Roodra Redirection & 404 Manager ===
Tags: redirection, 404, redirects
Requires at least: 5.8
Requires PHP: 7.4
Stable tag: 1.0.0
License: GPLv2 or later
License URI: https://www.gnu.org/licenses/gpl-2.0.html

Manage exact-path redirects and review recent 404 paths from your WordPress dashboard.

== Description ==
Roodra Redirection & 404 Manager lets administrators create redirects and review recent missing URL paths from Tools > Redirection & 404.

* Create and edit exact-path redirects with 301, 302, 307 or 308 status codes.
* Enable or disable individual redirects, and see their hit counts.
* Review aggregated 404 paths and create a redirect from a logged path.
* Delete individual logs or clear the log.

The plugin does not connect to external services. Redirect destinations can be external URLs chosen by an administrator.

== Installation ==
1. Upload and activate the plugin using Plugins > Add New > Upload Plugin.
2. Open Tools > Redirection & 404.
3. Add an exact source path and a destination URL, choose a status code and save.

== Frequently Asked Questions ==
= How are URLs matched? =
Matching is case-sensitive and uses the exact request path, including any site subdirectory. Query strings are ignored for matching and are not forwarded to the destination. You may include a query string in the destination itself.

= What data is logged? =
The plugin stores the requested path, a hit count and the most recent timestamp in UTC. It does not record query strings, IP addresses or referrers. Paths may themselves contain personal information. Review your site's privacy and retention practices. Logging is approximate and the plugin periodically trims the log to the 1,000 most recently seen unique paths.

= Does it work with caching? =
Requests served by a cache, CDN or web server without reaching WordPress cannot be redirected or logged by the plugin. Clear relevant caches after changing redirects.

= What happens when I remove the plugin? =
Deactivation retains redirects and logs. Deleting the plugin through WordPress permanently deletes its database tables. Network-wide activation on multisite is not supported; activate separately on each site.

== Changelog ==
= 1.0.0 =
* Initial release.
