gentoo_cronbits
===============

Various Gentoo-related scripts for cron-based housekeeping

The scripts are:
+cron.daily:
++clean_distfiles - clean out the distfiles and packages dirs
++depclean - remove packages that are no longer needed
++eix_sync - synchronize our Portage tree to the master
++emaint_check - check for and peform routine maintenance
++emerge_check - check if there are any packaged to install/upgrade/downgrade
++emerge_tweet - alert the sys admin about the packages to be installed/upgraded/downgraded
++emerge_world - install/upgrade/downgrade our local packages
++enable_bash_completions - enable any available Bash tab completions
++get_news - report if there is any Gentoo news available
++glsa_check - check for outstanding security alerts on this system
++preserved_rebuild - correct issues created by upgrading shared libraries
++profile_check - check for new Gentoo profiles
++sort_portage_sets - sort our Portage sets files
<br>
+cron.weekly:
++eix_obsolete - ensure we have no stale USE flags

Usage
-----
Simply drop the files in /etc/cron.{daily,weekly}, edit to taste, and enjoy.

Requirements
------------
Gentoo
<br>GNU Bash
<br>app-portage/eix
<br>app-portage/gentoolkit
<br>sys-apps/portage (>= 2.2.x)
<br>app-admin/eselect
<br>GNU Coreutils

Bugs
----
Find a bug? Please create an issue here on GitHub at:
https://github.com/hunleyd/gentoo_cronbits/issues

Twitter
-------
Keep up to date on announcements and more by following Doug on Twitter, <a href="http://twitter.com/hunleyd">@hunleyd</a>

Authors
-------
**Douglas J Hunley**
+ G+: http://goo.gl/sajR3
+ Twitter: http://twitter.com/hunleyd
+ GitHub: http://github.com/hunleyd

Copyright and license
---------------------
Copyright 2012 Douglas J Hunley.

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this work
except in compliance with the License. You may obtain a copy of the License in the
LICENSE file, or at:

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the
License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND,
either express or implied. See the License for the specific language governing
permissions and limitations under the License.
