# Angular DateParser

A simple parser that converts date and time strings into JavaScript Date objects.

[Demo](http://dnasir.github.io/angular-dateParser/demo.html)

## Prerequisites

1. Angular 1.0.1+

## Usage

Simply include the parser file, add it as a dependency and call it like so:

    $dateParser(string, format)

The first parameter is the date and time string you wish to convert to a Date object, and the second parameter is the format you're using. The format is optional, so if you're using the RFC2822 or ISO 8601 date formats, you're more or less safe, as the parser will simply pass the string to the Date constructor.

Expected return value is a JavaScript Date object, be it valid or otherwise.

## Date formats

All Date formats specified in the Date filter documentation can be used, as well as custom formats. See the demo for examples.

## Localisation

This parser depends on the $locale service to provide it with the list of formats, as well as names of months and days. To use this feature, include the locale file included in the Angular bundle.
