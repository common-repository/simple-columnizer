=== Simple Columnizer ===

Contributors: Muhammad Babar
Tags: simple columnizer, column, section, responsive column, Box, Bootstrap Columns, Column shortcodes, Column generator
Requires at least: WP 3.5.1 & Bootstrap libraries
Tested up to: 4.1.1
Stable tag: 4.1.1
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

== Description ==

Simple columnizer create "Widget Area" with name "Columnizer Widget Area" in admin section with Drag & Drop "Columnizer" widget. You can generate number of columns. Place short code where you want. Short code available to you after save the widget.


== Installation ==

1. Upload `simple-columnizer` to the `/wp-content/plugins/` directory
1. Activate the plugin through the 'Plugins' menu in WordPress 

== Frequently Asked Questions ==

= How add new style? =

	$style2 = array(
		'style 2' => array(
			'container_wrapper_start' => '<div class="row-example">',
			'container_wrapper_end' => '</div>',
			'icon_wrapper_start' => '<span %s%>',
			'icon_wrapper_end' => '</span>',
			'title_wrapper_start' => '<h3 %s%>',
			'title_wrapper_end' => '</h3>',
			'content_wrapper_start' => '<p %s%>',
			'content_wrapper_end' => '</p>'
		)
	);
		
	apply_filters('responsive_style_filter', $style2);
	
add in functions.php or in plugin file.

= How add new classes? =


	$column_classes = array(
		"Custom Classes" => array(
			'col-lg-1',
			'col-lg-2'
			)
		);
	apply_filters('columnizer_column_classes_filter', $column_classes);

add in functions.php or in plugin file.


== Screenshots ==

1. Drag & Drop Columnizer widget.
2. Add column informations.
3. Example : Preview on the page.