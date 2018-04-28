<?php

function test_custom_menu() {
  $items = array();

  $items['examples/form-example'] = array( //this creates a URL that will call this form at "examples/form-example"
    'title' => 'Example Form', //page title
    'description' => 'A form to mess around with.',
    'page callback' => 'drupal_get_form', //this is the function that will be called when the page is accessed.  for a form, use drupal_get_form
    'page arguments' => array('test_custom_form'), //put the name of the form here
    'access callback' => TRUE
  );

  return $items;
}

function test_custom_form($form, &$form_state) {
  
 $form['price'] = array(
    '#type' => 'textfield', //you can find a list of available types in the form api
    '#title' => 'What is Your Price?',
    '#size' => 10,
    '#maxlength' => 10,
    '#required' => TRUE, //make this field required 
  );

  $form['submit_button'] = array(
    '#type' => 'submit',
    '#value' => t('Click Here!'),
  );
  
  return $form;
}

function test_custom_form_validate($form, &$form_state) {
}

function test_custom_form_submit($form, &$form_state) {
}
?>