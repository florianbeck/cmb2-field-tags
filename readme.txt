=== CMB2 Field Type: Tags ===

Contributors: florianbeck  
Donate link: http://florianbeck.de
Tags: metabox
Requires at least: 3.8.2  
Tested up to: 4.4.2  
Stable tag: 1.0.0  
License: GPLv3  
License URI: http://www.gnu.org/licenses/gpl-3.0.html

WorsPress-Tags-like field type for Custom Metaboxes and Fields for WordPress using CMB2. 

== Description ==

WordPress-Tags-like field type for [CMB2](https://wordpress.org/plugins/cmb2). Based on [WordPress Tags-Like Meta Box](https://github.com/WebDevStudios/WordPress-tags-like-meta-box).

This plugin gives you two CMB2 field types:

1. The `tags` field acts like WordPress's default tags list.
2. The `tags_sortable`field acts like WordPress's default tags list as well, but adds sorting.

The Entrys will be saved as single string separated with semicolons.

**Note:** This field may not support repetition, repeatable fields/groups is untested.

== Installation ==

You can install this field type as you would a WordPress plugin: 

1. Download the plugin
2. Place the plugin folder in your `wp-content/plugins/` directory
3. Activate the plugin in the Plugin dashboard

= Usage =

`tags` — WordPress-Tags-like input field. Example:

```
array(
	'name' => 'Related Publications',
	'id'   => $prefix . 'related_publications',
	'desc' => 'Add or remove BibTeX-keys.',
	'type' => 'tags',
),
```

`tags_sortable` — WordPress-Tags-like input field that allows sorting. Example:

```
array(
	'name' => 'Tasks',
	'id'   => $prefix . 'tasks',
	'desc' => 'Add or remove tasks, drag and drop to sort.',
	'type' => 'tags_sortable',
),
```

== Screenshots ==

1. Adding entry in tags box.
2. Deleting entry in tags box.
3. Adding entry in tags_sortable box.
4. Sorting entry in tags_sortable box.