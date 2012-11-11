# BodyClass for ProcessWire

## Description
***

A ProcessWire module to add some classes to your body tag. That will give you a better control of your CSS.

## Basic usage
***

Add this code into the class of your body tag:

	<?php echo $modules->get("BodyClass")->bodyclass() ?>
	
So your body tag should look like this:

	<body class="<?php echo $modules->get("BodyClass")->bodyclass() ?>">

## Custom usage
***

	<?php echo $modules->get("BodyClass")->bodyclass(array('page_id' => false, 'template_name_prefix' => 'templatename-')) ?>

## Default options
***

	array(
		'page_id' => true,
		// bool (default true) return the page id
		
		'page_id_prefix' => 'page-id-',
		// string (default 'page-id-') prefix for page_id
		
		'parent_page_id' => true,
		// bool (default true) return the page id of of parents
		
		'parent_page_id_prefix' => 'parent-page-id-',
		// string (default 'parent-page-id-') prefix for parent_page_id
		
		'template_name' => true,
		// bool (default true) return the template name
		
		'template_name_prefix' => 'template-',
		// string (default 'template-') prefix for template_name
		
		'browser_info' => true
		// bool (default true) return some browser informations (os, browser, browserversion)
	);
	
## Installation
***

1. Copy the BodyClass.module file into site/modules
2. In the admin interface, navigate to the modules page and hit the “Check for new modules” button
3. Click on “BodyClass” in the new module message or scroll down until you locate it
4. Click the “Install” button