# Scrollspy

## What is it?

Scrollspy is something that I needed to include in a project that does not use bootstrap.
I still needed the scrollspy functionality that is bundled with bootstrap and after playing around with some alternatives, I found that the best solution was to create my own.
The idea was to create a simple solution that did pretty much everything that bootstraps solution offers.
So this is why I created this plugin.

For those that are not familiar with bootstraps scrollspy, basically this allows you to attach the plugin to a **ul** styled menu on a single page application. When you scroll down the page, the **pages** that you pass through would then mark the **li** children of your menu with an active class.

## Requirements

jQuery

## Demo

I have created a demo which you can find here:
http://codepen.io/r3plica/pen/NqbarV

## Installation

unzip the contents to your desired location and include either library on your page.

## How to use

It's really easy to use, simply initialise the script like this:

```
    $("#nav").scrollspy();
```

To pass options to the plugin, simply pass an object to the call like so:

```
    $("#nav").scrollspy({ offset: -25 });
```

## Available options

Currently there are only a few options:

### activeClass

This allows you to define your own active class that gets added to the **li** element of the menu.
*default: 'active'*

### animate

This tells the plugin whether it should animate the scroll when a link in your menu is click or not.
*default: false*

### offset

This tells the plugin if there is any need to include an offset.
*default: 0*

### onChange

This function is called whenever the document scrolls into a new **page**.

### onExit

In some cercumstances there will be a **page** that is not included in the menu. When scrollspy gets to this area the onExit function is called.


