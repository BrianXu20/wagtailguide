# Wagtail Guide
![tests](https://github.com/kevinhowbrook/wagtailguide/workflows/Test/badge.svg)

## What is it?

The Wagtail Guide app adds functionality for creating and editing a guide for editors and publishers to help them create good content.

## Installation

Wagtailguide has a pypi package and can be installed with:

```
pip install wagtail-guide
```

After installing, add it to your settings file along with `wagtail.contrib.settings`, the settings inclusion should be placed with your other wagtail.contrib libraries:

```
INSTALLED_APPS = [
    ...
    'wagtail_guide',
    'wagtail.contrib.settings',
]
```

## Dependencies
Wagtail Guide requires `wagtail>=2.16`

## Usage
To edit the guide, the user needs to be an admin, or have the `Manage editor guide` 'change' value checked in their user group permissions.

### Editing the guide
To edit the guide, from the left hand menu open settings > then click 'Manage editor guide'. Edit your content and then save.

![guide edit](https://i.imgur.com/ZGRlu3I.png)

#### Guide navigation menu
If more than one 'heading' blocks are added to the content, an automatic menu will be displayed at the top of the guide under the heading 'Contents'

### Viewing the guide
Once logged in, a new menu icon towards the bottom of the left hand menu will be visible labeled as 'Editor guide':

![guide view](https://i.imgur.com/HbCVvXy.png)
