---
wrapper_template: _layouts/docs.html
context:
  title: Radio panel | Design Guidelines
  status: draft
---
# Overview

A Radio Panel is a large, visually-striking version of the traditional radio button controls. Instead of small, browser-native controls, the Radio Panel features large, clickable panels with additional information on each. They are, like radio buttons, mutually exclusive - only 1 can be selected per panel group at a given time. 

# General Usage

## When to Use

Use a Radio Panel when you want the user to pick from a few mutually exclusive options - great examples of this are during a product selection process - where these options are few in number and important to the user. 

An important difference between Radio buttons and the Radio Panel is the initial state:

* Radio Panels can have 1 item selected by default on load, or no selection by default

  * Once a selection is made, it’s not possible to “go back” to the “no selection” state without a page reload
* Radio buttons should always have 1 item in the button group selected by default

![Wireframe of a panel of three radio buttons](/vanilla/templates/static/images/image8.png)

In this example above, the user is picking an important part of the product - and the visual preview of paint colours works well in a Radio Panel. 

This pattern is also useful for logos or other media elements, to aid recognition and recall and make the form feel more intuitive to users:

![Panel of four radio buttons for MicroK8s, AWS, Google Cloud and Azure](/vanilla/templates/static/images/image7.png)

A case for not using Radio Panels and instead using regular radio buttons, would be - for example - options like delivery methods, or other configuration options in a settings view:

![List of three stacked default radio buttons](/vanilla/templates/static/images/image3.png)

In the case above, the choice isn’t very visual or core to the experience of purchasing - so a radio group makes sense. 

## When not to use

Don’t use Radio Panels;

1. If the choice isn’t particularly visual or significant to the core experience
2. If the item descriptions are particularly long you may find a standard radio group works better
3. If you already have a lot of Radio Panels - by adding more, you decrease the significance of the Panels in the view and reduce the impact

# Anatomy

Radio Panels can be thought of as large, styled radio buttons in a button group. Their behaviour is identical to browser-native radio buttons. 

![The radio button should have an icon, multiline copy, or both. It is wrapped in a rectangular panel with border and background colour](/vanilla/templates/static/images/image2.png)

Upon load, one may be selected - or no Radio Panel may be selected. 

There is a visual indication that one Panel is currently selected.

# Variants Overview

(This section is for internal usage)

Variants should be differentiated on usage level - they are best practices for users to achieve a specific goal, but will be used in different context.

<table>
  <tr>
   <td>Variants
   </td>
   <td>Description
   </td>
   <td>Use cases on our products
   </td>
  </tr>
  <tr>
   <td rowspan="3" >A name
   </td>
   <td rowspan="3" >Radio Panels (Desktop viewport)
   </td>
   <td rowspan="2" >
<ul>

<li>Ubuntu Pro Product Selector (+ Blender)
</li>
</ul>
   </td>
  </tr>
  <tr>
  </tr>
  <tr>
   <td>
<ul>

<li>JUJU “Brew with K8s” \

</li>
</ul>
   </td>
  </tr>
  <tr>
   <td>B name
   </td>
   <td>Radio Panels (Mobile viewport)
   </td>
   <td>
<ul>

<li>UA Product Selector (+ Blender)
</li>
</ul>
   </td>
  </tr>
  <tr>
   <td>
   </td>
   <td>
   </td>
   <td>
   </td>
  </tr>
</table>

# Radio Panels (Desktop viewport)

## Definition

A group of styled Radio Panels in a group where selecting one is mutually exclusive and deselects the currently selected item (if selected). 

## The look

![Wireframe of a radio panel with three buttons](/vanilla/templates/static/images/image1.png "image_tooltip")

## Usage

Radio Panels are not intended to replace simple radio button groups, and care should be taken to not overuse them - which will just slow users down and complicate views. 

They are best used sparingly when you want to draw attention to a selection.  \

* Present users with a Radio Panel to add impact or improve the experience of selecting between different choices
* Use when there is a visual example, a logo or a colour to be highlighted
* Use the space for copy to explain why this option is different from the others
* Decide if the group should have an initial selection or not 

## Behaviours

The Radio Panel is selected by a click or a tap. On selection, the Panel changes appearance and any other selected item is deselected. 

### Initial state on load

On load the Panels in the group can be in one of the following states:

1. Selected (up to 1 Panel)
2. Not selected

### Interaction states

The states are as follows:

Enabled

1. Default
2. Hover
3. Selected

Disabled

1. Un-selected
2. Selected \

If the Radio Panel is in a disabled state, then it cannot be interacted with, but up to 1 Panel can be selected.

## Examples

Radio Panels are in use in our products as listed below:

[Ubuntu Advantage product selector](https://ubuntu.com/pro/subscribe):

<p id="gdcalert6" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image6.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert7">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image6.png "image_tooltip")

[Coffee by Juju promotional page](https://juju.is/brew):

<p id="gdcalert7" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image7.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert8">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image7.png "image_tooltip")

# Radio Panels (Mobile viewport)

In a mobile viewport, the Radio Panel behaviour is unchanged, but the developer has a couple of options for how to display the panels:

## Option 1 - 2-column:

<p id="gdcalert8" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image8.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert9">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image8.png "image_tooltip")

Panels are arranged side-by-side in 2 columns. When controls don’t contain much copy, this is ideal. Individual panels are still large enough to be easily tapped without forcing the user to scroll too much to see all the options. 

## Option 2 - 1-column full-width:

<p id="gdcalert9" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image9.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert10">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>

![alt_text](images/image9.png "image_tooltip")

Panels are arranged in one full-width column. Depending on the viewport size and the amount of copy in each panel, this may be the best option for your users.
