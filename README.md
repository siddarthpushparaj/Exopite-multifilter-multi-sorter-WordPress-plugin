# Exopite Multifilter
## WordPress Plugin

- Author: Joe Szalai
- Version: 1.0.2
- Plugin URL: https://github.com/JoeSz/exopite-multifilter
- Author URL: http://joe.szalai.org
- License: GNU General Public License v3 or later
- License URI: http://www.gnu.org/licenses/gpl-3.0.html

DESCRIPTION
-----------

Exopite multifilter, mutlisortable, multi selectable, multi filterable sortable Wordpress Plugin

AJAX sorter/filter for any page or post types by multiple taxonomies and/or terms. <br />
(like post by categories/tags or any custom post type taxonomies like "portfolio-categories"). <br />
Plugin working with a basic Bootstrap 4 Flex grid. Only enqueued, if style with 'bootstrap' or 'bootstrap-4' slug not already enqueued.

* Working with any Themes and any post types
* Single or multiple filter based on taxonomies and terms. Multi selectable.
* Search in pre-selected taxonomies and terms
* Wordking via shortcode, can be used multiple times on a posts or pages (or custom post types)
* AJAX pagination
* AJAX infinite loading
* AJAX read more loading
* Update browser URL with infintie or read more loading based on page and scroll position
* Store session (page number, selected filters and search). <br />
Useful if visitor is hit back or click on back button (if any) on the sinlge page/post.
* Bootstrap 4 Flex grid
* JavaScript Hooks <br />
https://github.com/carldanley/WP-JS-Hooks
* Translatable via po/mo files. Pot included.
* Multiple hover effects <br />
https://tympanus.net/Development/HoverEffectIdeas/index.html <br />
https://tympanus.net/Development/HoverEffectIdeas/index2.html

Paginated                  |  Title and readmore loading |  Multiple selection  <br />(tags and categories)
:-------------------------:|:---------------------------:|:-------------------------:
![](assets/screenshot-1.png)      |  ![](assets/screenshot-2.png)      |  ![](assets/screenshot-3.png)

USAGE
-----

The plugin working via `[exopite-multifilter]` shortcodes, does not display any admin options. <br />
You can use multiple shortcodes on the same page/post. On posts with 'pretty' permalink, pagination not working well.

Examples:
* `[exopite-multifilter post_type="exopite-portfolio" thumbnail-size-single-row="blog-list-full" thumbnail-size-multi-row="blog-list-multiple" taxonomies_terms="exopite-portfolio-category, exopite-portfolio-tag"]`
* `[exopite-multifilter thumbnail-size-single-row="blog-list-full" thumbnail-size-multi-row="blog-list-multiple"]`

Available options

| Options                            | Values                                                                       | Defaults
| ---------------------------------- | ---------------------------------------------------------------------------- | --------
| `post_type`                        | ['post-type-slug'] as post type slug                                         | post
| `posts_per_page`                   | ['number'] how many post per page per shortcode                              | 4
| `posts_per_row`                    | ['1' - '4'] how many posts per row per shortcode                             | 2
| `display_title`                    | ['true' or 'false'] display post title                                       | false
| `display_pagination`               | ['true' or 'false'] display pagination                                       | true
| `display_filter`                   | ['true' or 'false'] display filter                                           | true
| `blog_layout`                      | ['top', 'left', 'right', 'zigzag' or 'none']                                 | top
| `no-gap`                           | ['true' or 'false'] hide gap between post                                    | false
| `except_lenght`                    | ['number'] the lenght of the exceprt by words, '0' means no exceprt          | 0
| `except_more`                      | ['text'] excerpt more                                                        |
| `pagination`                       | ['pagination', 'readmore' or 'infinite'] the type of the pagination          | pagination
| `multi_selectable`                 | ['true' or 'false'] single or multiselect: true or false                     | true
| `thumbnail-size-single-row`        | ['thumbnail-size-slug'] thumbnail size for single post per row               | full
| `thumbnail-size-multi-row`         | ['thumbnail-size-slug'] thumbnail size for multipe post per row              | large
| `taxonomies_terms`                 | ['category, category(slug&#124;slug)' or 'tag' etc...] the filters                | category
| `update_paged`                     | ['true' or 'false'] Update page in browser URL bar on readmore and infinite loading based on viewport | false
| `display_page_number`              | ['true' or 'false'] Show page number between loads in infinite and readmore  | false
| `paged`                            | ['number'], Set start page number if not already paged                       | 1
| `effect`                           | ['apollo', 'duke', 'goliath', 'julia', 'lexi', 'ming' or 'steve']            | apollo
| `search`                           | ['search'] if set, filter will be disabled                                   |
| `store_session`                    | ['true' or 'false'] Store current session (page number, selected filters and search). Useful if visitor is hit back or click on back button | false

INSTALLATION
------------

1. [x] Upload `exopite-multifilter` to the `/wp-content/plugins/exopite-multifilter/` directory

OR

1. [ ] ~~Install plugin from WordPress repository (not yet)~~

2. [x] Activate the plugin through the 'Plugins' menu in WordPress

REQUIREMENTS
------------

Server

* WordPress 4.0+ (May work with earlier versions too)
* PHP 5.3+ (Required)
* jQuery 1.9.1+

Browsers

* Modern Browsers
* Firefox, Chrome, Safari, Opera, IE 10+
* Tested on Firefox, Chrome, Edge, IE 11

PLANNED
-------

* On mobile 6 page number is too much -> how should be displayed?
* Add widget (only if [CodeStar Framework](http://codestarframework.com/) as plugin installed)
* Display post meta
* AJAX nounce
* Random posts
* Add to WordPress repo.

CHANGELOG
---------

= 1.0.2 - 2017-03-05 =
* Improvement: Automatic script and style versioning for local css and js files based on file time.
https://www.doitwithwp.com/enqueue-scripts-styles-automatic-versioning/

= 1.0.1 - 2017-03-04 =
* Add: restore previous session (localstorage)
* Add: more filters

= 1.0 =
* Initial release.

LICENSE DETAILS
---------------
The GPL license of Exopite Multifilter grants you the right to use, study, share (copy), modify and (re)distribute the software, as long as these license terms are retained.

DISCLAMER
---------

NO WARRANTY OF ANY KIND! USE THIS SOFTWARES AND INFORMATIONS AT YOUR OWN RISK! READ DISCLAMER.TXT!
License: GNU General Public License v3

[![forthebadge](http://forthebadge.com/images/badges/built-by-developers.svg)](http://forthebadge.com) [![forthebadge](http://forthebadge.com/images/badges/for-you.svg)](http://forthebadge.com)
