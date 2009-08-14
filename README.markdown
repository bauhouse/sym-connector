# Joyent Connector - A Symphony Ensemble

A while ago, Joyent announced their Connector Suite as 
[Free + Open](http://joyeur.com/2007/07/17/joyent-connector-free-open), 
offering free accounts and releasing an open source Ruby on Rails project, 
with the SVN repository at [dev.joyent.net](http://dev.joyent.com/projects/connector/blog). 
So, what happened after that? Very little. Apparently, no one was interested.

In my mind, that was a shame. It is a beautiful interface. If only its functionality as an 
integrated suite of collaboration tools lived up to the promise. A number of issues remain 
as part of the [Maintenance milestone](https://dev.joyent.com/projects/connector/tickets?status=1&milestone=4). 
A [few tickets were closed](https://dev.joyent.com/projects/connector/tickets?status=0&milestone=4), 
but little more has happened with the project since.

Having found that the GPL v2 released Joyent Connector is here on GitHub, 
it would be nice to see this project revived in some way. This repository is my pet project 
to build the Joyent Connector (or parts of it) as a Symphony CMS Ensemble.

I have omitted the Ruby files. The page templates are included for the Login panel, 
the error pages, and the main pages of the interface, with relative URLs pointing to images, 
JavaScript and CSS assets:

- Connect
- Mail
- Calendar
- People
- Files
- Bookmarks
- Lists

**Note**: The complete source files are quite large, so have been omitted from this repository.
The original Joyent Connector repository can be found here: <http://github.com/luke0x/connector/tree/master>.

## Screenshots

### Connect

<a href="http://www.flickr.com/photos/bauhouse/3766449118/" title="joyent-connector-connect by bauhouse, on Flickr"><img src="http://farm3.static.flickr.com/2442/3766449118_6c00af0245_o.png" width="800" height="600" alt="joyent-connector-connect" /></a>

### Mail

<a href="http://www.flickr.com/photos/bauhouse/3765653795/" title="joyent-connector-mail by bauhouse, on Flickr"><img src="http://farm4.static.flickr.com/3435/3765653795_74de08258c_o.png" width="800" height="600" alt="joyent-connector-mail" /></a>

### Calendar

<a href="http://www.flickr.com/photos/bauhouse/3766449222/" title="joyent-connector-calendar by bauhouse, on Flickr"><img src="http://farm3.static.flickr.com/2654/3766449222_277e6dd0eb_o.png" width="800" height="600" alt="joyent-connector-calendar" /></a>

### People

<a href="http://www.flickr.com/photos/bauhouse/3765775699/" title="joyent-connector-people by bauhouse, on Flickr"><img src="http://farm4.static.flickr.com/3483/3765775699_24dcba539c_o.png" width="800" height="600" alt="joyent-connector-people" /></a>

### Files

<a href="http://www.flickr.com/photos/bauhouse/3765654115/" title="joyent-connector-files by bauhouse, on Flickr"><img src="http://farm3.static.flickr.com/2488/3765654115_c2635e5571_o.png" width="800" height="600" alt="joyent-connector-files" /></a>

### Bookmarks

<a href="http://www.flickr.com/photos/bauhouse/3765654223/" title="joyent-connector-bookmarks by bauhouse, on Flickr"><img src="http://farm4.static.flickr.com/3448/3765654223_d903bb51c4_o.png" width="800" height="600" alt="joyent-connector-bookmarks" /></a>

### Lists

<a href="http://www.flickr.com/photos/bauhouse/3765654329/" title="joyent-connector-lists by bauhouse, on Flickr"><img src="http://farm4.static.flickr.com/3444/3765654329_0fa2d8aca7_o.png" width="800" height="600" alt="joyent-connector-lists" /></a>

## Created with Symphony CMS

- Version: 2.0.6
- Date: 4th August 2009
- Github Repository: <http://github.com/symphony/symphony-2/tree/master>


## Synopsis

Symphony is a `PHP` & `MySQL` based CMS that utilises `XML` and `XSLT` as its core 
technologies. This repository represents version 2.0.6 and is considered stable.

Visit the forum at <http://symphony-cms.com/community/>


## Updating

### Important Information

Version `2.0.5` introduced multiple includable elements, in the Data Source Editor, for a single field. After updating from `2.0.5` or lower, the DS editor will seem to "forget" about any `Textarea` fields selected when you are editing existing Data Sources. After updating, you must ensure you re-select them before saving. Note, this will only effect Data Sources that you edit and were created prior to `2.0.5`. Until that point, the field will still be included in any front-end XML

### Via Git

1. Pull from the master branch at `git://github.com/symphony/symphony-2.git`

2. Use the following command to get Extensions up to date:

	git submodule init
	git submodule update

3. If updating from a version less than `2.0.5`, enable [Debug DevKit](http://github.com/symphony/debugdevkit/tree/master) and [Profile DevKit](http://github.com/symphony/profiledevkit/tree/master) extensions.

4. Follow normal updating procedure below from step 2.

### Via the old fashioned way

Follow the instructions below if you are updating from Symphony version 2.0 (non Git)

**Note:** As of 2.0.6, there is no longer a need to backup `/symphony/.htaccess`.

1. Upload `/symphony`, `index.php` & `update.php`, replacing what is already on your server.

2. If you are updating from a version < 2.0.5, download and install the Debug DevKit and Profile DevKit:

	- [Debug DevKit](http://github.com/symphony/debugdevkit/tree/master)
	- [Profile DevKit](http://github.com/symphony/profiledevkit/tree/master)

3. Go to `http://yoursite.com/update.php` to complete the update process.

4. Celebrate by shaving your friend's head for charity!


## INSTALLING

### Via Git

1. Clone the git repository to the location you desire using:

		git clone git://github.com/symphony/symphony-2.git
		
	Should you wish to make contributions back to the project, fork the master tree rather than cloning, and issue pull requests via github.

	The following repositories are included as submodules:

	- [Markdown](http://github.com/pointybeard/markdown)
	- [Maintenance Mode](http://github.com/pointybeard/maintenance_mode)
	- [Select Box Link Field](http://github.com/pointybeard/selectbox_link_field)
	- [JIT Image Manipulation](http://github.com/pointybeard/jit_image_manipulation)
	- [Export Ensemble](http://github.com/pointybeard/export_ensemble)
	- [Debug DevKit](http://github.com/symphony/debugdevkit/tree/master)
	- [Profile DevKit](http://github.com/symphony/profiledevkit/tree/master)

3. Run the following command to ensure the submodules are cloned:

		git submodule update --init

4. _(Optional)_ If you would like the [default theme](http://github.com/symphony/workspace/tree) installed as well, 
you will need to use the following command from within the Symphony 2 folder you just created:

		git clone git://github.com/symphony/workspace.git
		
5. Follow normal installation procedure below from step 2.


### Via the old fashioned way

**Note: You can leave `/workspace` out if you do not want the default theme.**

1. This step assumes you downloaded a zip archive from the [Symphony website](http://symphony-cms.com). 
Upload the following files and directories to the root directory of your website:

	- index.php
	- install.php
	- /symphony
	- /workspace
	- /extensions

2. Point your web browser at <http://yourwebsite.com/install.php> and provide
details for establishing a database connection and about your server environment.

3. Jump with both arms up like you're in a car commercial!


## SECURITY

**Secure Production Sites: Change permissions and remove installer files.**

1. For a smooth install process, change permissions for the `root`, `symphony` and `workspace` directories.

		cd /your/site/root
		chmod 777 symphony .
		chmod -R 777 workspace

2. Once successfully installed, change permissions as per your server preferences:

		chmod 755 symphony .

3. Remove installer files (unless you're fine with revealing all your trade secrets):

		rm install.php install.sql workspace/install.sql update.php

4. Dance like it's 1999!