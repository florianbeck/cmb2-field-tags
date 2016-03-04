# CMB2 Field Type: Tags

**Contributors:**      [florianbeck](https://github.com/florianbeck)  
**Donate link:**       [http://florianbeck.de](http://florianbeck.de)  
**Required at least:** 3.8.2  
**Tested up to:**      4.4.2  
**Stable tag:**        1.0.0  
**License:** GPLv3  
**License URI:** [http://www.gnu.org/licenses/gpl-3.0.html](http://www.gnu.org/licenses/gpl-3.0.html)

WorsPress-Tags-like field type for Custom Metaboxes and Fields for WordPress using CMB2.  

## Description
WordPress-Tags-like field type for [CMB2](https://github.com/WebDevStudios/CMB2). Based on [WordPress Tags-Like Meta Box](https://github.com/WebDevStudios/WordPress-tags-like-meta-box).

This plugin gives you two CMB2 field types:

1. The ```tags``` field acts like WordPress's default tags list.
2. The ```tags_sortable```field acts like WordPress's default tags list as well, but adds sorting.

The Entrys will be saved as single string separated with semicolons.

**Note:** This field may not support repetition, repeatable fields/groups is untested.

## Installation
You can install this field type as you would a WordPress plugin: 

1. Download the plugin
2. Place the plugin folder in your ```wp-content/plugins/``` directory
3. Activate the plugin in the Plugin dashboard

Alternatively, you can plate the plugin folder within your theme/plugin. After you call CMB2:

```php
require_once 'init.php';
```

Add another line to include the ```cmb2-field-tags.php``` file. Something like:

```php
require_once 'cmb2-field-type-tags/cmb2-field-type-tags.php';
```

## Usage

See [CMB2's Wiki](https://github.com/WebDevStudios/CMB2/wiki) for general explanations of how to use CMB2.

```tags``` — WordPress-Tags-like input field. Example:

```php
array(
	'name' => 'Related Publications',
	'id'   => $prefix . 'related_publications',
	'desc' => 'Add or remove BibTeX-keys.',
	'type' => 'tags',
),
```

```tags_sortable``` — WordPress-Tags-like input field that allows sorting. Example:

```php
array(
	'name' => 'Tasks',
	'id'   => $prefix . 'tasks',
	'desc' => 'Add or remove tasks, drag and drop to sort.',
	'type' => 'tags_sortable',
),
```

## Screenshots

### Tags box

Adding entry in tags box:
![Adding entry in tags box](screenshot-1.jpg)

Deleting entry in tags box:
![Deleting entry in tags box](screenshot-2.jpg)

### Tags box (sortable)

Adding entry in tags_sortable box:
![Adding entry in tags_sortable box](screenshot-3.jpg)

Sorting entry in tags_sortable box:
![Deleting entry in tags_sortablebox](screenshot-4.jpg)
