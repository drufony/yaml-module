YAML Module
===========

Creates a YAML form element which allows complex configuration to be added in a single
text area.

Example
-------

```php
<?php
  $form['module_settings'] = array(
    '#type' => 'yaml',
    '#title' => t('Settings'),
    '#default_value' => variable_get('module_settings', array(
      'something' => TRUE,
      'another_thing' => 100,
      'something_else' => 'this is a string',
      'list' => array(123, 456, 789),
      'deeper' => array(
        'top' => TRUE,
        'left' => FALSE,
      ),
    )),
  );
```
