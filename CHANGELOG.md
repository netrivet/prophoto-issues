# Changelog

### 6.21.16

Additional bugfixes related to WordPress 5 (1/17/19)

* Updated content image alignment to work with WordPress 5 image block
* Worked around conflict with Yoast SEO plugin (and possibly others) in editor/customizer
* Fixes classic editor issue when toggling post/page editor containing a gallery between visual/text mode
* Added warning for hitting upload filesize limit when importing a design

### 6.21.15

Another WordPress 5 update (12/6/18)

* Adding compatibility for users on WordPress 5 and using the classic editor plugin

### 6.21.14

WordPress 5 and Gutenberg (12/5/18)

* Adding compatibility for the Gutenberg plugin and WordPress 5

### 6.21.13

Updates (10/1/18)

* Updated background videos to auto-play after browser updates require "mute" parameter 
* Upated Instagram authentication process after change in Instagram API

### 6.21.12

Enhancement (7/31/18)

* Adding a remote JS file to admin pages for easier messaging

### 6.21.11

Bugfixes & enhancements (5/24/18)

* (GDPR compliance) Added opt-in checkbox for cookies in comment form
* Fixed bug causing forms with a Tile submit button containing an image to submit twice

### 6.21.10

Bugfixes & enhancements (5/3/18)

* Changes for compatability with PHP 7.2
* Change in Instagram API requires us to keep requesting images until we have enough
* Improved font rendering in Firefox

### 6.21.9

Bugfixes (2/16/18)

* Fix a bug with thumbnail galleries when closing full-window mode and re-clicking same image
* Prevent slight grid rendering problem caused by CloudFlare injecting script tags into grid markup

### 6.21.8

Bugfixes & enhancements (2/12/18)

* fix rare problem (usually on Dreamhost) with varnish cache and WordPress content not updating
* allow plugin to disable inclusion of Facebook javascript
* support new WooCommerce gallery type
* fix broken appearance of "Customize" button on P6 theme block in "Appearance" > "Themes" page
* add button to manually clear Instagram cache

### 6.21.7

Bugfix

* fix problem with ProPhoto text widget turning same-domain links into relative urls after recent WordPress update

### 6.21.6

Bugfix

* fix bug caused by a recent WordPress update that can prevent customizations from saving correctly

### 6.21.5

Bugfixes & enhancements (12/15/17)

* ignore non-public taxonomies (like Yoast's "Prominent SEO words") for template assignments in customizer
* try to prevent some false-positive warnings from security plugins regarding usage of base64_en/decode
* add extra safeguard for extremely rare bug where all text widgets dissappear due to serialized data corruption
* prevent customizer stuck on loading graphic in rare scenarios where WPML has been de-activated
* clarify in customizer that video backgrounds don't work on phones
* fix ios fixed/scroll override on columns
* fix bug that could prevent form validation message font style to not correctly apply
* prevent rare bug caused by plugins or services injecting unexpected script tags inside of grids

### 6.21.4

Bugfix (11/29/17)

* guard against very rare scenario where template assignments get corrupted from `6.21.3` migration

### 6.21.3

Bugfixes & enhancements (11/21/17)

* fix post/page template assignments not accounting for customizing vs. live design
* show more descriptive error messages for registration failures
* allow plugins to prevent ProPhoto from inserting missing content image database records

### 6.21.2

WP 4.9.0 Compat & Bugfix (10/24/17)

* prevent errors from changes introduced by WordPress in `4.9.0`
* fix display bug with slide-up style overlay grids having excerpt text or read-more links

### 6.21.1

Bugfix (10/17/17)

* fix a bug with customization inheritance between templates caused by WordPress security update `4.8.2`

### 6.21.0

New features -- [Blog post](https://pro.photo/blog/prophoto-6-21-0) (10/2/17)

* **New feature:** Customize ProPhoto gallery permalink slug [#798](https://github.com/downshiftorg/prophoto-issues/issues/798)
* **New feature:** Control ProPhoto galleries with arrow keys [#218](https://github.com/downshiftorg/prophoto-issues/issues/218)
* **New feature:** Display post author name & link in post header or footer [#595](https://github.com/downshiftorg/prophoto-issues/issues/595)
* **New feature:** Optionally disable swipe-to-open functionality for mobile menu [#622](https://github.com/downshiftorg/prophoto-issues/issues/622)
* *Enhancement:* Ajax-loaded gallery images now fully support WordPress-driven alt text [#737](https://github.com/downshiftorg/prophoto-issues/issues/737)
* *Enhancement:* Set a unique background color for footer copyright area only [#391](https://github.com/downshiftorg/prophoto-issues/issues/391)
* *Enhancement:* Remove outdated rich structured markup to easily support plugins focused on that domain [#796](https://github.com/downshiftorg/prophoto-issues/issues/796)
* removed confusing fallback horizontal menu used when no menu widgets present [#775](https://github.com/downshiftorg/prophoto-issues/issues/775)
* default is now for ProPhoto page-caching to be _enabled_
* fix bug where page cache did not expire when a new comment was added
* fix bug with WordPress `4.8.2` that can cause fatal error in customizer

### 6.20.6

Bugfixes & support enhancements (7/31/17)

* fix bug with font styles not being correctly applied to form dropdown elements
* fix new Firefox flexbox bug with full-height blocks and aligned rows
* added support helpers for quicker diagnostics and support replies

### 6.20.5

Bugfixes (7/10/17)

* remove babel polyfill to prevent errors from new version of Yoast
* restore support for lists in P6 text widget
* update initial activation welcome video
* allow plugins to prevent P6 javascript from loading

### 6.20.4

Bugfix (6/19/17)

* fix build error in `6.20.3` causing ProPhoto admin Settings page errors and other admin javascript problems

### 6.20.3

Bugfixes (6/16/17)

* fix flexbox rendering bug in Firefox (PC) for full-height blocks
* fix auto-starting slideshows in old versions of Safari

### 6.20.2

WP 4.8 Compat (6/6/17)

* ensure compatibility with WordPress 4.8, due for release soon
* fix graphic selects components overridable when inheriting [#758](https://github.com/downshiftorg/prophoto-issues/issues/758)

### 6.20.1

Bugfix (5/22/17)

* prevent fatal error for proofing plugin users updating to `6.20.x` who haven't recently logged-in

### 6.20.0

New free designs & features -- [Blog post](https://pro.photo/blog/prophoto-6-20-0) (5/18/17)

* **New feature:** [Agency](https://pro.photo/design/agency/demo) -- new free included starter design [#745](https://github.com/downshiftorg/prophoto-issues/issues/745)
* **New feature:** [Creative](https://pro.photo/design/creative/demo) -- new free included starter design [#745](https://github.com/downshiftorg/prophoto-issues/issues/745)
* **New feature:** [New Age](https://pro.photo/design/new-age/demo) -- new free included starter design [#745](https://github.com/downshiftorg/prophoto-issues/issues/745)
* **New feature:** gallery image label overlays _(number or filename)_
* **New feature:** window-height block row alignment _(top, center, bottom, or spread)_
* **New feature:** control auto-updating preference and allow trigging of forced update [#570](https://github.com/downshiftorg/prophoto-issues/issues/570)
* **New feature:** block/row/column scroll-to links can be appended to _home_ and _page_ menu items
* support columns having top/bottom padding greater than 50%
* fix responsive breakpoint inheriting settings not always reflected on site front layout
* fix bug with tile shape layer border-radius
* fix bug with horizontal menu alignment using new _Custom Text_ menu item from `6.19.0`
* fix rendering of Pinterest _pin-any_ call-to-action link text

### 6.19.3

Bugfixes (5/10/17)

* fix gallery sizing problem introduced in recent build
* fix PHP warning with numbered pagination when not enough posts to require pagination
* add safeguards to prevent rare fatal errors running template inheritance repair migration

### 6.19.2

Bugfixes (5/9/17)

* fix php warnings in widgets admin screen introduced in `6.19.0`
* fix inability to edit embedded ProPhoto galleries due to change in TinyMCE in WordPress `4.7.4`
* fix _slide_ style widget transition animations on Safari when also rendering a sticky block
* fix form placeholder selected font style not taking effect
* prevent PHP notice (only visible if `WP_DEBUG` on) when rendering ProPhoto gallery pages

### 6.19.1

Bugfixes (5/5/17)

* fix php warnings from plugin widgets introduced in `6.19.0`
* ensure plugin widgets support new widget animation feature
* don't incorrectly show widget animation options for call-to-action items

### 6.19.0

New features -- [Blog post](https://pro.photo/blog/prophoto-6-19-0) (5/3/17)

* **New feature:** Widget visibility animations [#746](https://github.com/downshiftorg/prophoto-issues/issues/746)
* **New feature:** Featured image background images & widget [#371](https://github.com/downshiftorg/prophoto-issues/issues/371)
* **New feature:** Copy/paste blocks, rows, and columns in the customizer [#474](https://github.com/downshiftorg/prophoto-issues/issues/474)
* **New feature:** Numbered pagination for older/newer posts [#352](https://github.com/downshiftorg/prophoto-issues/issues/352)
* **New feature:** Significantly expanded customization options for ProPhoto forms [#447](https://github.com/downshiftorg/prophoto-issues/issues/447)
* **New feature:** Customizer onboarding wizard [#744](https://github.com/downshiftorg/prophoto-issues/issues/744)
* **New feature:** New "Post header widget" allows for placing post/page header in custom locations
* **New feature:** New "Spacer widget" for fine-grained overrides of widget spacing
* **New feature:** New menu item type: Custom text -- for non-linking menu items and custom containers [#589](https://github.com/downshiftorg/prophoto-issues/issues/589)
* fix bug displaying uploaded Facebook blog posts page preview image
* fix bug with non-inheriting form customization settings & repair broken designs
* fix auto-update logic issue for proofing plugin users
* images inside a sticky block should never be lazy-loaded to prevent sizing issues
* ensure compatibility with Yoast SEO plugin's configurator page
* fix post-separator showing after last post on page [#268](https://github.com/downshiftorg/prophoto-issues/issues/268)
* fix bug with widget blockquote font styles not being applied [#743](https://github.com/downshiftorg/prophoto-issues/issues/743)
* fix rare tile rendering bugs when a plugin strips html comments
* fix sizing bugs with thumbnail galleries having height constraint
* trigger mobile menu to close when clicking a link with a hash
* add some default styling to `<dl>`, `<table>`, and `<address>` tags

### 6.18.2

Bugfixes (4/19/17)

* workaround plugins flushing rewrite rules in a way that results in ProPhoto gallery permalink 404 errors
* add filter for plugins to influence display of excerpts
* remove whitespace in tile text layers to prevent very rare rendering bugs in Edge
* better handle absolute urls with scroll-to hashes

### 6.18.1

Bugfixes (4/12/17)

* fix display problem with carousel galleries due to build error
* prevent ProPhoto from attempting to cache rest api routes
* toggle hamburger toggle button state when swiping to open/close mobile menu
* fix post page gallery creation and rest request errors for users with outdated versions of WordPress

### 6.18.0

New features -- [Blog post](https://pro.photo/blog/prophoto-6-18-0) (4/11/17)

* **New feature:** New gallery style: Carousel [#453](https://github.com/downshiftorg/prophoto-issues/issues/453)
* **New feature:** Video backgrounds for blocks from uploaded mp4s, YouTube, Vimeo [#363](https://github.com/downshiftorg/prophoto-issues/issues/363)
* **New feature:** New video widget - simplifies embedding videos from YouTube/Vimeo responsively
* **New feature:** Built-in page caching for speed improvement [#747](https://github.com/downshiftorg/prophoto-issues/issues/747)
* **New feature:** Customizable widths for ProPhoto form field elements [#580](https://github.com/downshiftorg/prophoto-issues/issues/580)
* fix bug with certain combinations archive excerpts display settings [#751](https://github.com/downshiftorg/prophoto-issues/issues/751)
* switched to composer class-map auto-loading for page load speed improvement
* removed many uneccesary files not used in production for faster/safer auto-updates
* optimize number and timing of requests made by customizer to help hosts that struggle with concurrency
* fix rare bug exporting designs with Call-to-Action items and `WP_DEBUG` enabled
* fix grid retina image functionality for newer devices with very high pixel density ratios
* fix bug with logged contact form submissions displaying fields out of order when > 8 form fields

### 6.17.3

Security fix (3/22/17)

* prevent an unauthorized request from exposing data that should be only visible to admins

### 6.17.2

Bugfixes (3/21/17)

* fix bug with contact form slow submission processing when combined with CloudFlare
* fix Pinterest pin single image tile/image margin customizations not taking effect
* fix occasional bug uploading image for featured image from post/page editor screen
* fix tile bug in Internet Explorer when images are scaled down in size
* workaround issue with Pinterest not accepting dynamic image creation endpoints
* updated tutorial link in ProPhoto settings area
* slightly improve admin performance by being more selective about when to flush rewrite rules
* clear cache from "WP Fastest Cache" when customizations made

### 6.17.1

Bugfixes (3/11/17)

* show users incompatible WordPress message if less than WordPress `4.4.0`
* fix bug causing Call-to-action items to not render on gallery pages
* fix bug with title tags on paged page-types older than first page
* fix bug for proofing users unable to upload images to proofing images
* update outdated url for finding Facebook admin id

### 6.17.0

New features -- [Blog post](https://pro.photo/blog/prophoto-6-17-0) (3/8/17)

* **New feature:** Create ProPhoto galleries from post/page edit screen [#527](https://github.com/downshiftorg/prophoto-issues/issues/527)
* **New feature:** Allow collapsing of blocks in customizer, remembering selection between templates and sessions [#463](https://github.com/downshiftorg/prophoto-issues/issues/463)
* **New feature:** Set image alt attribute text for image widgets [#725](https://github.com/downshiftorg/prophoto-issues/issues/725)
* **New feature:** Image protection attempts to prevent drag/drop of protected images [#594](https://github.com/downshiftorg/prophoto-issues/issues/594)

### 6.16.3

Bugfix (3/3/17)

* work around memory issues causing crashing on mobile safari with large crossfade galleries [#742](https://github.com/downshiftorg/prophoto-issues/issues/742)

### 6.16.2

Bugfix & caching compatibility (3/1/17)

* fix a bug introduced by `6.16.0` where gallery would resize when encountering images with different aspect ratios
* attempt to clear various possible caching layers when the admin is making customizations
* prevent caching of password-protected posts
* workaround issue with WP Super Cache sending template css with incorrect content-type

### 6.16.1

Performance enhancement (2/27/17)

* improved gallery perfomance on mobile devices

### 6.16.0

New features, enhancements, & bugfixes -- [Blog post](https://pro.photo/blog/prophoto-6-16-0) (2/24/17)

* **New feature:** WooCommerce support [#723](https://github.com/downshiftorg/prophoto-issues/issues/723)
* **New feature:** Significantly updated versions of free included designs [Sunny](https://pro.photo/design/sunny/demo) and [Square](https://pro.photo/design/sunny/square), with more templates & leveraging more recent ProPhoto features
* **New feature:** Allow constraining gallery vertical height to percentage of window height [#627](https://github.com/downshiftorg/prophoto-issues/issues/627)
* **New feature:** Allow inserting of gallery as ordered full-size images into posts & pages [#715](https://github.com/downshiftorg/prophoto-issues/issues/715)
* **New feature:** Custom upload for Facebook blog posts page preview image [#566](https://github.com/downshiftorg/prophoto-issues/issues/566)
* **New feature:** Optionally disable all ProPhoto Facebook preview `og:meta`	to allow plugin override without duplicate meta tags [#724](https://github.com/downshiftorg/prophoto-issues/issues/724)
* _Enhancement:_ Add support for Facebook `og:image:width` and `og:image:height` for better first-time sharing previews
* fix animation jitter in galleries during lazy gallery page loading
* fix problem with letterspacing in font-styles for tiles [#562](https://github.com/downshiftorg/prophoto-issues/issues/562)
* fix rare possibility of CSS being generated for wrong design caused by caching layers [#738](https://github.com/downshiftorg/prophoto-issues/issues/738)
* fix intermittent sizing issues in galleries on Safari [#513](https://github.com/downshiftorg/prophoto-issues/issues/513)
* fix font-style _word-spacing_ attribute not applying on site front
* prevent rare Safari tile rendering problems caused by uneccessary trailing `<br />` tags in tile text layers
* add safegaurd against extremetly rare problem with corrupt text widget strings causing loss of all text widget data
* fix lack of styling for logged-out commenting explanatory text
* optimize image lazy-load counting to prevent rare problems with element sizing near site header
* fix rare bug for users on outdated PHP builds missing PHP multi-byte string support
* prevent tile rendering problems in Firefox and older IE versions when text overflows tile before scaling
* fix error preventing admin deleting ProPhoto downsized/modified images from settings area
* fix bug causing full-window galleries to display _behind_ sticky blocks

### 6.15.7

Bugfix (2/10/17)

* fix additional problem with clicking menu items in sticky blocks caused by new version of Chrome (56)

### 6.15.6

Bugfix (2/9/17)

* workaround bug in new version of Chrome (56) causing problems with sticky blocks

### 6.15.5

Bugfixes (2/6/17)

* fix error loading customizer for rare users missing PHP multi-byte string functions, introduced in `6.15.4`
* fix creation of "Recent posts from category" grid when first category never changed

### 6.15.4

Bugfixes (2/1/17)

* fix 2 bugs that cause newly added premium designs or newly copied designs from being immediately visible
* fix a problem with corrupted strings when lower-casing Cyrillic and other UTF-8 strings
* fix error copying widgets between templates when target template has no widget of same type
* fix bug exporting designs with `.woff` custom fonts that could cause import and customization problems
* prevent rare scenarios where users could delete active design
* attempt to recover from scenario where the active design could not be loaded
* add "Cache-safe CSS" mode to help with poorly implemented caching layers
* fix rare bug with sticky blocks and window resize events
* don't use position:sticky for sticky blocks when within an iframe because of Safari bug

### 6.15.3

Bugfixes (1/18/17)

* fix bug that could cause galleries inserted into posts to be deleted in some circumstances while editing post/page
* fix bug with sticky-block menus falling behind tiles in Safari
* added support tooling enhancements

### 6.15.2

Bugfixes (1/13/17)

* change session token storage to work around buggy host/plugin code and caching strategies which caused repeated "Let me customize - session detected" warnings in the ProPhoto customizer
* fixed bug causing Call to Action items to render on static home page when not set to in some cases

### 6.15.1

Bugfixes (1/5/17)

* fix gallery images wrongly inheriting post image margins since `6.14.7` [#733](https://github.com/downshiftorg/prophoto-issues/issues/733)
* fix non-working pinterest default pinit style since `6.15.0` [#732](https://github.com/downshiftorg/prophoto-issues/issues/732)

### 6.15.0

Domain change (12/27/16)

* compatibility with new pro.photo domain and API infrastructure

### 6.14.8

Bugfix (12/22/16)

* fix Safari rendering bug caused by MS Edge flexbox bugfix from `6.14.7`

### 6.14.7

Bugfixes (12/16/16)

* fix bug where pinit overlay tile images were inheriting post image border and margin [#730](https://github.com/downshiftorg/prophoto-issues/issues/730)
* add filter to allow plugins to bypass url prefixing
* fix minor rendering bug in tiles within grids
* fix bug causing menu drop-downs in non-stuck sticky block to fall behind other items
* fix sizing bug for pinterest overlay when html attributes constraining image size
* fix MS Edge flexbox rendering bug for latest build of Edge
* fix some PHP notices from PHP 7.1 in strict error reporting mode
* prevent fatal errors caused by deleted pinterest button graphics
* fix form email time rendering when using UTC offsets [#728](https://github.com/downshiftorg/prophoto-issues/issues/728)

### 6.14.6

Bugfix & new videos (11/21/16)

* fix padding bug for gallery thumbnail strips on iPads
* replace post-registration welcome video with updated version
* embed ProPhoto bar video in ProPhoto bar notification about itself

### 6.14.5

Bugfixes (11/9/16)

* fix pinterest pin overlay not rendered for images with no `class` attribute [#727](https://github.com/downshiftorg/prophoto-issues/issues/727)
* fix pinit overlay sizing problems for small or right/left aligned images [#726](https://github.com/downshiftorg/prophoto-issues/issues/726)
* fix layout bug in new version of Chrome causing content to spill below footer

### 6.14.4

Bugfixes (11/4/16)

* enhancement - add classes to rendered form and form elements for custom styling
* clarify language regarding Facebook comments in customizer
* fix some HTML validation errors
* don't show ProPhoto techs ProPhoto bar notifications

### 6.14.3

Bugfixes (10/31/16)

* fix bug causing srcset not to choose most optimal image size
* fix iOS longpress to save image prevented when image protection off [#721](https://github.com/downshiftorg/prophoto-issues/issues/721)
* fix duplicated data in Sunny free design that can cause customization problems
* add support/tech tooling for diagnosing duplicate customization data

### 6.14.2

Bugfixes (10/27/16)

* fix prophoto bar notifications not staying dismissed for web hosts not supporting http `DELETE` [#719](https://github.com/downshiftorg/prophoto-issues/issues/719)
* fix post content image margin incorrectly applying to gallery thumbnails [#720](https://github.com/downshiftorg/prophoto-issues/issues/720)
* fix design setup wizard not always on-boarding correct design

### 6.14.1

Bugfixes (10/20/16)

* fix problem causing fatal error for a percentage of users updating to `6.14.0`
* directly link to customizer template assignments from post/page template assignment override metabox
* fix grid widget admin labels being cleared when creating a new grid widget

### 6.14.0

New features (10/19/16)

* **New feature:** Preview and customize non-live designs -- show one design to visitors while you work on another [#542](https://github.com/downshiftorg/prophoto-issues/issues/542)
* **New feature:** New "Coming Soon/Maintenance Mode" free design to be used while customizing a different design [#553](https://github.com/downshiftorg/prophoto-issues/issues/553)
* **New feature:** Embedded gallery shortcodes now displayed as interactive visual graphic element in post editor [#642](https://github.com/downshiftorg/prophoto-issues/issues/642)
* **New feature:** Control visibility of gallery permalink page titles and dates [#365](https://github.com/downshiftorg/prophoto-issues/issues/365)
* **New feature:** Customizing design switcher in customizer and front-end ProPhoto bar
* *Enhancement:* totally re-designed _Manage Designs_ screen with better design, usability & support for customizing non-live designs


### 6.13.2

Bugfix (10/6/16)

* fix another bug related to new WPML functionality - menu item dynamic children strings continually re-registered

### 6.13.1

Bugfixes (10/6/16)

* prevent some problems with WPML's latest update and string auto-registration [#713](https://github.com/downshiftorg/prophoto-issues/issues/713)
* prevent multiple customizer sessions from same browser, different tabs [#711](https://github.com/downshiftorg/prophoto-issues/issues/711)
* fix harmless but invalid css being generated [#710](https://github.com/downshiftorg/prophoto-issues/issues/710)
* fix copied tiles sharing WPML text layer translation [#708](https://github.com/downshiftorg/prophoto-issues/issues/708)
* increase possible max-width for column borders
* allow viewing pages without all user-supplied custom CSS

### 6.13.0

Instagram grid type and bugfixes -- [Blog post](https://www.prophoto.com/blog/prophoto-6-13-0/) (9/27/16)

* **New feature:** New grid type: Instagram feed [#241](https://github.com/downshiftorg/prophoto-issues/issues/241)
* fix extra spacing for non-overlaid gallery thumbstrips on small devices [#654](https://github.com/downshiftorg/prophoto-issues/issues/654)
* fix output of telephone `tel:xxx...` links in graphics widgets [#706](https://github.com/downshiftorg/prophoto-issues/issues/706)
* prevent very rare fatal error for hosts without `php-exif` support [#707](https://github.com/downshiftorg/prophoto-issues/issues/707)
* fix appearance of "Remove custom font" button on narrow screens [#698](https://github.com/downshiftorg/prophoto-issues/issues/698)
* fix appearance of special characters in menu titles [#699](https://github.com/downshiftorg/prophoto-issues/issues/699)
* added some tooling for ProPhoto support techs for faster diagnosis of issues

### 6.12.2

Bugfix

* fix errors copying or saving edits to tiles made previous to `6.12.0` [#703](https://github.com/downshiftorg/prophoto-issues/issues/703)

### 6.12.1

Bugfixes

* fix slightly incorrect alignment of vertically centered rollover grid text
* prevent design on-boarder from hanging when bad menu item data encountered

### 6.12.0

Features, enhancements and bugfixes -- [Blog post](https://www.prophoto.com/blog/prophoto-6-12-0/) (9/14/16)

* **New feature:** Mobile menu toggle can now be a ProPhoto tile with customizeable "active" state [#357](https://github.com/downshiftorg/prophoto-issues/issues/357)
* **New feature:** Optional background images for grid items & background color/image for whole grids [#677](https://github.com/downshiftorg/prophoto-issues/issues/677)
* *Enhancement:* overlay grid text vertical alignment control [#676](https://github.com/downshiftorg/prophoto-issues/issues/676)
* *Enhancement:* control text length of post grid item excerpt text [#678](https://github.com/downshiftorg/prophoto-issues/issues/678)
* *Enhancement:* allow uploading of "featured" images for categories, for use in category grids [#592](https://github.com/downshiftorg/prophoto-issues/issues/592)
* *Enhancement:* allow uploading of grid item fallback images [#354](https://github.com/downshiftorg/prophoto-issues/issues/354)
* fix overlay grid overlays not always perfectly matching size of underlying image [#162](https://github.com/downshiftorg/prophoto-issues/issues/162)
* fix WP RSS feed request not redirecting to Feedburner when valid Feedburner url set [#569](https://github.com/downshiftorg/prophoto-issues/issues/569)
* fix background color for light-color font-style previews [#696](https://github.com/downshiftorg/prophoto-issues/issues/696)
* fix custom grid items set to open link in new page not working for clicks on rollover overlay [#697](https://github.com/downshiftorg/prophoto-issues/issues/697)

### 6.11.1

Enhancement & bugfix (9/8/16)

* *Enhancement:* re-enable Pinterest "pin site image" Call to Action item now that it should be working reliably
* fix php notice from `6.11.0` that breaks tile display only when `WP_DEBUG` turned on

### 6.11.0

Features, enhancements and bugfixes -- [Blog post](https://www.prophoto.com/blog/prophoto-6-11-0/) (9/7/16)

* **New feature:** Pinterest pinning of individual content images [#229](https://github.com/downshiftorg/prophoto-issues/issues/229)
* **New feature:** Toggle visibility of nested items in mobile/vertical menu [#282](https://github.com/downshiftorg/prophoto-issues/issues/282)
* *Enhancement:* allow aligning mobile menu and hamburger icon on site right side
* *Enhancement:* allow translating of menu item and graphic widget urls for WPML [#695](https://github.com/downshiftorg/prophoto-issues/issues/REPLACE)
* fix problem with phantom image attachments being generated when downsizing threshold set very low [#690](https://github.com/downshiftorg/prophoto-issues/issues/690)
* fix failure to show customization group "locked" state when jumping between levels with breadcrumbs [#691](https://github.com/downshiftorg/prophoto-issues/issues/691)
* fix galleries that hang because of missing thumbnail sizes [#688](https://github.com/downshiftorg/prophoto-issues/issues/REPLACE)
* fix grid display bug when sizing constraints set extremely narrow [#692](https://github.com/downshiftorg/prophoto-issues/issues/692)
* fix problem importing remote design assets from `us-east-1` Amazon S3 region
* fix display of form submission email subjects to honor timezone setting [#694](https://github.com/downshiftorg/prophoto-issues/issues/694)

### 6.10.2

Bugfix (9/1/16)

* fix galleries showing up empty in non-primary lanugage when using WPML
* fix incorrect front page displaying when using WMPL string translation
* fix overlay grid background color not displaying after 6.10 update

### 6.10.1

Bugfix (8/31/16)

* fix empty space below grid in certain scenarios (introduced in 6.10.0)

### 6.10.0

New features, enhancements, and bugfixes -- [Blog post](https://www.prophoto.com/blog/prophoto-6-10-0/) (8/31/16)

* **New feature:** Use tile or image for custom form _submit_ button [#550](https://github.com/downshiftorg/prophoto-issues/issues/550)
* **New feature:** Support opacity option for every customizable color [#430](https://github.com/downshiftorg/prophoto-issues/issues/430)
* **New feature:** Column border customizations [#314](https://github.com/downshiftorg/prophoto-issues/issues/314)
* *Enhancement:* Clarify customization UI when customizations inheriting from parent template [#521](https://github.com/downshiftorg/prophoto-issues/issues/521)
* *Enhancement:* Allow toggling of grid item optional text in every situation [#674](https://github.com/downshiftorg/prophoto-issues/issues/674)
* *Enhancement:* Allow clicking directly to where inherited customization is coming from in tooltip [#225](https://github.com/downshiftorg/prophoto-issues/issues/225)
* *Enhancement:* Add clickable breadcrumbs for template/block/row/column items
* *Enhancement:* Use image from embedded gallery as post excerpt image when no other image present [#438](https://github.com/downshiftorg/prophoto-issues/issues/438)
* *Enhancement:* Ensure grids that don't take up full width of context are centered [#333](https://github.com/downshiftorg/prophoto-issues/issues/333)
* *Enhancement:* Only permit renaming blocks at highest template level to prevent the illusion of upward inheritance
* fix cropped grids not keeping rows even when differing amounts of text [#421](https://github.com/downshiftorg/prophoto-issues/issues/421)
* fix password protected galleries not showing password form [#682](https://github.com/downshiftorg/prophoto-issues/issues/682)
* fix problem with translated `page for posts` in WPML [#681](https://github.com/downshiftorg/prophoto-issues/issues/681)
* ensure custom grid item opens in new window/tab when set to [#673](https://github.com/downshiftorg/prophoto-issues/issues/673)
* fix a few fringe problems with form remote email sending [#672](https://github.com/downshiftorg/prophoto-issues/issues/672)
* improve handling of timezone for form submissions [#667](https://github.com/downshiftorg/prophoto-issues/issues/667)
* fix application of template-specific watermarking settings [#670](https://github.com/downshiftorg/prophoto-issues/issues/670)
* fix rare circumstance where ProPhoto bar would not be shown if theme file editing disabled


### 6.9.1

Bugfix (8/16/2016)

* fix custom grid items showing title twice instead of title and text

### 6.9.0

New features -- [Blog post](https://www.prophoto.com/blog/prophoto-6-9-0/) (8/15/16)

* **New feature:** Support for WPML multi-language plugin [#235](https://github.com/downshiftorg/prophoto-issues/issues/235)
* **New feature:** Forms now offer multiple-choice (radio) and select dropdown field options [#577](https://github.com/downshiftorg/prophoto-issues/issues/577)

### 6.8.0

Features, enhancements, & bugfixes -- [Blog post](https://www.prophoto.com/blog/prophoto-6-8-0/) (8/10/16)

* **New feature:** Image lazyloading (currently disabled by default) [#410](https://github.com/downshiftorg/prophoto-issues/issues/410)
* *Enhancement:* Design onboarding menu-item step for connecting content menu items [#639](https://github.com/downshiftorg/prophoto-issues/issues/639)
* *Enhancement:* Improve usability of included "Morgan" design with simpler templates and better inheritance
* *Enhancement:* Add a "blog" menu item type that always links to blog posts page
* fix thumbnail gallery and grid images not being included in right-click image protection [#665](https://github.com/downshiftorg/prophoto-issues/issues/665)
* add widget labels for grid widgets replaced by text placeholders
* remove embedded help widget (every admin page still has help link for contacting us)

### 6.7.3

Bugfix (8/5/16)

* fix error that caused proofing plugin users to not see their orders

### 6.7.2

Bugfixes (8/4/16)

* fix wrong layout rendered when returning to layout component after switching templates
* fix tooltip alignment for add-row elements
* fix bug that can cause very small tile borders to be invisible

### 6.7.1

Bugfix (8/3/16)

* fix inability to load Call-to-Action appearance & assignments areas in customizer since `6.7.0`

### 6.7.0

Features, enhancements, & bugfixes -- [Blog post](https://www.prophoto.com/blog/prophoto-6-7-0/) (8/2/16)

* **New feature:** Design _on-boarding_ wizard to guide through front page & template assignments [#638](https://github.com/downshiftorg/prophoto-issues/issues/638)
* **New feature:** Customizable form submission email subject & body [#551](https://github.com/downshiftorg/prophoto-issues/issues/551)
* **New feature:** Find all template background images from site front toolbar & click to edit [#637](https://github.com/downshiftorg/prophoto-issues/issues/637)
* **New feature:** Front-end ProPhoto bar inspect mode inspects and links to blocks, rows, columns, & widgets [#636](https://github.com/downshiftorg/prophoto-issues/issues/636)
* **New feature:** Form submission success & error redirect urls [#599](https://github.com/downshiftorg/prophoto-issues/issues/599)
* *Enhancement:* Add domain-based email `sendfrom` and remote email sending to improve email delivery rates [#641](https://github.com/downshiftorg/prophoto-issues/issues/641)
* *Enhancement:* Override form notification email recipeient on a per-form basis
* *Enhancement:* Don't close customization modals when clicking "save" [#465](https://github.com/downshiftorg/prophoto-issues/issues/465)
* *Enhancement:* Add toggle for excerpt "read more" link [#575](https://github.com/downshiftorg/prophoto-issues/issues/575)
* *Enhancement:* Add default "read more" link font styles to included designs
* *Enhancement:* Power customizer state through url route to allow direct linking to any state
* fix google/statcounter analytics wrongly counting admin visits [#656](https://github.com/downshiftorg/prophoto-issues/issues/656)
* fix incorrect sizing of sticky-block placeholder [#655](https://github.com/downshiftorg/prophoto-issues/issues/655)
* fix major javascript error when trying to render gallery with zero images [#652](https://github.com/downshiftorg/prophoto-issues/issues/652)
* isolate javascript modules to prevent error in one from bringing down others [#653](https://github.com/downshiftorg/prophoto-issues/issues/653)
* fix error loading image in customizer if filename contained comma [#648](https://github.com/downshiftorg/prophoto-issues/issues/648)

### 6.6.5

Bugfixes (7/28/16)

* prevent & fix problems with non-working front-page and call-to-action settings [#650](https://github.com/downshiftorg/prophoto-issues/issues/650)
* fix bug causing galleries to hang on very small images [#651](https://github.com/downshiftorg/prophoto-issues/issues/651)
* fix occasional weird display of long decimal values in tile height field [#649](https://github.com/downshiftorg/prophoto-issues/issues/649)

### 6.6.4

Enhancement/bugfix (7/26/16)

* import selected P5/4 settings [#619](https://github.com/downshiftorg/prophoto-issues/issues/619)

### 6.6.3

Bugfixes (7/22/16)

* fix bug resolving page for posts if WordPress option never existed [#647](https://github.com/downshiftorg/prophoto-issues/issues/647)
* fix email reply-to address header [#646](https://github.com/downshiftorg/prophoto-issues/issues/646)
* fix slashes being added to saved ProPhoto site settings [#645](https://github.com/downshiftorg/prophoto-issues/issues/645)
* hide P3 gallery placeholders on site front [#644](https://github.com/downshiftorg/prophoto-issues/issues/644)

### 6.6.2

Bugfix (7/20/16)

* fix bug affecting a few updaters to `6.6.x` causing static home page setting not to be obeyed

### 6.6.1

Bugfixes (7/20/16)

* fix rare error from archives menu item when zero published posts [#632](https://github.com/downshiftorg/prophoto-issues/issues/632)
* fix front-end widget link hash broken in `6.6.0`

### 6.6.0

Features & enhancements -- [Blog post](https://www.prophoto.com/blog/prophoto-6-6-0/) (7/20/16)

* Front-page settings now controlled in customizer on a per-design basis
* Reorganize customizer to clearly distinguish between _design_ and _template_ areas [#196](https://github.com/downshiftorg/prophoto-issues/issues/196)
* Fix problems saving site settings in very rare circumstances [#629](https://github.com/downshiftorg/prophoto-issues/issues/629)
* Fix deleting menu item from library pops up two modals [#630](https://github.com/downshiftorg/prophoto-issues/issues/630)

### 6.5.1

Bugfix (7/13/16)

* fix bug causing mobile menu hamburger icon click to not work [#623](https://github.com/downshiftorg/prophoto-issues/issues/623)

### 6.5.0

Features & enhancements -- [Blog post](https://www.prophoto.com/blog/prophoto-6-5-0/) (7/12/16)

* Add "ProPhoto bar" on front for admins with inspecting and direct links to edit widgets
* Allow max-height constraint based on window size for content images [#395](https://github.com/downshiftorg/prophoto-issues/issues/395)
* Use form submitted email address as notification reply-to address [#552](https://github.com/downshiftorg/prophoto-issues/issues/552)
* Cross-browser compatible form required field validation with customizable messages [#587](https://github.com/downshiftorg/prophoto-issues/issues/587)

### 6.4.7

Hotfix (7/11/16)

* disables caching of front-end query because we didn't consider how templates are resolved ¯\\\_(ツ)_/¯ [#621](https://github.com/downshiftorg/prophoto-issues/issues/621)

### 6.4.6

Performance enhancement (7/11/16)

* cache main front-end query for faster page loads

### 6.4.5

Bugfixes (7/8/16)

* fix fatal error from Seo class on pages where `$post` can't be found [#618](https://github.com/downshiftorg/prophoto-issues/issues/618)
* fix fatal errors on `PHP 5.3.6` [#617](https://github.com/downshiftorg/prophoto-issues/issues/617)
* fix errors related to call-to-action from designs exported at `6.4.0`

### 6.4.4

Bugfixes & performance improvements (7/7/16)

* optimize main design database query for faster page loads
* fix errors copying certain templates & inability to create copies of broken copies [#611](https://github.com/downshiftorg/prophoto-issues/issues/611)
* fix inability to import P3-era galleries if source post can't be found [#614](https://github.com/downshiftorg/prophoto-issues/issues/614)
* fix column vertical padding not applied on MS Edge [#612](https://github.com/downshiftorg/prophoto-issues/issues/612)
* fix inability to delete images in certain scenarios in customizer [#613](https://github.com/downshiftorg/prophoto-issues/issues/613)
* fix content images broken due to failure to correct for previous site url locations [#609](https://github.com/downshiftorg/prophoto-issues/issues/609)
* fix password-protected post translation settings not applying [#616](https://github.com/downshiftorg/prophoto-issues/issues/616)
* fix unintuitive reordering of blocks [#590](https://github.com/downshiftorg/prophoto-issues/issues/590)
* fix problems with SEO and Facebook meta fields [#529](https://github.com/downshiftorg/prophoto-issues/issues/529)

### 6.4.3

Bugfix (7/1/16)

* Minor release adding some internal tooling for troubleshooting "undeletable" widgets

### 6.4.2

Bugfixes (6/30/16)

* fixes bug where tile selector would not scroll in a modal window
* fixes bug where exported form widgets would not render on front [#606](https://github.com/downshiftorg/prophoto-issues/issues/606)
* fixes bug with call to action groups on multi-post pages [#605](https://github.com/downshiftorg/prophoto-issues/issues/605)
* fixes inheritance issue with "Nav & Logo" block in "About" and "Info" templates in bundled design "Morgan"

### 6.4.1

Bugfix (6/29/16)

* fix fatal errors resulting from call to action database changes

### 6.4.0

Thumbnail galleries, Call to Action, and more -- [Blog post](https://www.prophoto.com/blog/prophoto-6-4-0/) (6/29/16)

* **New feature:** Thumbnail-style galleries [#351](https://github.com/downshiftorg/prophoto-issues/issues/351)
* **New feature:** Responsive call-to-action items [#223](https://github.com/downshiftorg/prophoto-issues/issues/223)
* **New feature:** Gallery "full-window" mode: an alternative to "fullscreen" and a great fallback for devices that don't support HTML5 fullscreen api (iPhones, iPads, IE10)
* fix bug deleting widgets caused by possibility of using duplicate widget ids from simultaneous customizer tabs [#603](https://github.com/downshiftorg/prophoto-issues/issues/603)
* fix non-taxonomy custom post type (like uncategorized proofing galleries) template assignments not applying [#602](https://github.com/downshiftorg/prophoto-issues/issues/602)
* fix auto-update failures on certain servers caused by too-long temp filename [#601](https://github.com/downshiftorg/prophoto-issues/issues/601)

### 6.3.1

Bugfixes (6/23/16)

* fix crossfading galleries occasionally going blank when images slow to load [#598](https://github.com/downshiftorg/prophoto-issues/issues/598)
* fix fatal error caused if plugin widget deactivated before deleting widget from P6 [#596](https://github.com/downshiftorg/prophoto-issues/issues/596)
* improve display of small-sized image dropzone upload areas

### 6.3.0

New features, enhancements, and bugfixes --  [Blog post](https://www.prophoto.com/blog/prophoto-6-3-0/) (6/22/16)

* **New feature:** Custom grids [#220](https://github.com/downshiftorg/prophoto-issues/issues/220)
* *Enhancement:* Newly added block or row will now _always_ appear in all child templates, regardless of inheritance state
* *Enhancement:* Many more template assignment controls, including 404, post categories, custom post types, proofing galleries, individual posts, individual galleries [#439](https://github.com/downshiftorg/prophoto-issues/issues/439)
* *Enhancement:* Hardware acceleration for better tile transitions and border behavior [#501](https://github.com/downshiftorg/prophoto-issues/issues/510)
* *Enhancement:* Tile text layer alignment options [#459](https://github.com/downshiftorg/prophoto-issues/issues/459)
* *Enhancement:* Allow linebreaks in tile text layers [#458](https://github.com/downshiftorg/prophoto-issues/issues/458)
* Fix bug causing script/slanted fonts to be partially cut off in tile text layers [#582](https://github.com/downshiftorg/prophoto-issues/issues/582)
* Guard against non-standard plugin widgets that can't be rendered [#588](https://github.com/downshiftorg/prophoto-issues/issues/588)
* Fix hiding of sticky block at responsive breakpoints [#591](https://github.com/downshiftorg/prophoto-issues/issues/591)

### 6.2.4

Bugfixes & experimental PHP7 support (6/14/16)

* *Enhancement:* PHP7 support (tested, but considered _experimental_ for a few weeks) [#563](https://github.com/downshiftorg/prophoto-issues/issues/563)
* Fix bug with tiles showing unexpected space below [#567](https://github.com/downshiftorg/prophoto-issues/issues/567)
* Fix non-working Facebook comments design settings [#568](https://github.com/downshiftorg/prophoto-issues/issues/568)
* Fix misleading display of inheriting image settings in customizer [#490](https://github.com/downshiftorg/prophoto-issues/issues/490)
* Fix sticky block mobile menu problem in IE11 [#558](https://github.com/downshiftorg/prophoto-issues/issues/558)
* Ensure only admin-level logged in users can access ProPhoto customizer

### 6.2.3

Bugfix (6/7/16)

* Fix bug that caused javascript errors for IE10 and older browers without ES6 support

### 6.2.2

Bugfixes (6/7/16)

* Fix inheritance bug with adding new entities from parent templates
[#561](https://github.com/downshiftorg/prophoto-issues/issues/561)
* Fix bug with excerpt images not being found - (affects things like og:image for Facebook)
[#564](https://github.com/downshiftorg/prophoto-issues/issues/564)

### 6.2.0

New features & bugfixes -- [Blog post](https://www.prophoto.com/blog/prophoto-6-2-0/) (6/7/16)

* **New feature:** Copy/pasting widgets
* **New feature:** Customizable text/tile/image "Read more" excerpt links for grids and standard excerpts [#297](https://github.com/downshiftorg/prophoto-issues/issues/297)
* **New feature:** Upload favicon and apple-touch-icon for site identity [#281](https://github.com/downshiftorg/prophoto-issues/issues/281)
* **Enhancement:** Select multiple gallery images and reorder them as a group [#543](https://github.com/downshiftorg/prophoto-issues/issues/543)
* Fix inability to drag/drop upload images on galleries admin screens [#548](https://github.com/downshiftorg/prophoto-issues/issues/548)
* Fix bug that caused mobile menu top/bottom padding customization to not apply [#560](https://github.com/downshiftorg/prophoto-issues/issues/560)
* Fix bug with positioning of stuck sticky block when mobile menu open [#557](https://github.com/downshiftorg/prophoto-issues/issues/557)
* Fix bug editing existing embedded grid in post/page [#556](https://github.com/downshiftorg/prophoto-issues/issues/556)

### 6.1.2

Bugfixes (6/2/16)

* Hopefully fix problem copying _Morgan_ free design on 1and1 and other servers [#555](https://github.com/downshiftorg/prophoto-issues/issues/555)
* Resolve a few scroll-to link problems [#549](https://github.com/downshiftorg/prophoto-issues/issues/549)
* Fix improperly rendered Mac command character for Safari 9 [#544](https://github.com/downshiftorg/prophoto-issues/issues/544)

### 6.1.1

Bugfixes (5/31/16)

* Fix bug that could cause Facebook `<og:image>` image data to not update when featured image changed [#547](https://github.com/downshiftorg/prophoto-issues/issues/547)
* Fix bug with Proofing plugin auto-updating when WordPress not in English [#546](https://github.com/downshiftorg/prophoto-issues/issues/546)
* Fix bug extracting uploaded design zips on Windows servers [#545](https://github.com/downshiftorg/prophoto-issues/issues/545)
* Support extensible grids for Proofing grid types

### 6.1.0

Scroll-to links, usability enhancements, more -- [Blog post](https://www.prophoto.com/blog/prophoto-6-1-0/) (5/27/16)

* **New feature:** Easily create links that smoothly scroll to blocks & rows [#163](https://github.com/downshiftorg/prophoto-issues/issues/163)
* *Enhancement:* Numerous usability and workflow improvements for managing gallery images
* Minification of generated css for performance
* Add infrastructure for support diagnostics
* Fix bug causing menu re-ordering problems with lengthy menus [#533](https://github.com/downshiftorg/prophoto-issues/issues/533)

### 6.0.1

Bugfixes (5/25/16)

* Fix bug that caused last form element to be deleted instead of chosen element [#539](https://github.com/downshiftorg/prophoto-issues/issues/539)
* Fix problem with block-height overrides in Safari [#540](https://github.com/downshiftorg/prophoto-issues/issues/540)
* Fix bug that could cause unexpected gallery appearance on mobile devices [#538](https://github.com/downshiftorg/prophoto-issues/issues/538)
* Prevent error messages when saving a widget without changing widget data [#537](https://github.com/downshiftorg/prophoto-issues/issues/537)
* Fix gallery images not visible in admin if any gallery images deleted [#536](https://github.com/downshiftorg/prophoto-issues/issues/536)

### 6.0.0

Release, enhancements, & bugfixes (5/24/16)

* Remove beta label
* *Enhancement:* Add user-interface for easily embedding ProPhoto forms in posts/pages
* *Enhancement:* Show template in front-end WordPress admin bar as link to edit that template
* *Enhancement:* Show ProPhoto responsive screensize in front-end WordPress admin bar
* *Enhancement:* Add default spacing for graphic widget label [#464](https://github.com/downshiftorg/prophoto-issues/issues/464)
* *Enhancement:* Add new tile square should always be first, and scroll to copied tile
* Improve appearance of test-drive and other admin notices on form log page [#535](https://github.com/downshiftorg/prophoto-issues/issues/535)
* Clear tile image upload dropzone for multiple image layers [#502](https://github.com/downshiftorg/prophoto-issues/issues/502)
* Fix widget body `h1` font-style overriding widget headline font-style [#511](https://github.com/downshiftorg/prophoto-issues/issues/511)
* Prevent gallery fullscreen button from appearing on devices that don't support html5 fullscreen api [#516](https://github.com/downshiftorg/prophoto-issues/issues/516)
* Fix aspect ratio of uploaded design images in Safari [#525](https://github.com/downshiftorg/prophoto-issues/issues/525)
* Don't force prev/next gallery controls on mobile for auto-starting galleries [#528](https://github.com/downshiftorg/prophoto-issues/issues/528)
* Fix gallery prev/next arrow alignment when control bar outside of gallery [#531](https://github.com/downshiftorg/prophoto-issues/issues/531)
* Fix Facebook comments not respecting language setting [#534](https://github.com/downshiftorg/prophoto-issues/issues/534)
* Remove javascript popup prompt for Zendesk help widget email address
* Don't display input box explanatory help for boxes without help text

### Beta Changelog:

_For the pre-release beta changelog, [go here](https://github.com/downshiftorg/prophoto-issues/blob/master/CHANGELOG-BETA.md)._
