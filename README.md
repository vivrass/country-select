# Country-Select

Provides a simple helper to get an HTML select list of countries.  The list of countries comes from the ISO 3166 standard.  While it is a relatively neutral source of country names, it will still offend some users.

Users are strongly advised to evaluate the suitability of this list given their user base.

## Latest Changes

As of version 1.0.5 a runtime error will be raised if any of the user-supplied priority countries do not correlate with those in the main country list.

**Note:** this may cause existing applications using country-select to fail, but such failures will highlight incorrect usage, enabling the implementation to be corrected so that correct and accurate data may be gathered.

Thanks to Steve Purcell (http://github.com/purcell) for this addition.

## Installation

Install as a gem using

    gem install country-select

Or put the following in your Gemfile

    gem 'country-select'

## Example

Simple use supplying model and attribute as parameters:

    country_select("user", "country_name")

Supplying priority countries to be placed at the top of the list:

    country_select("user", "country_name", [ "United Kingdom", "France", "Germany" ])

## Changelist

 - **1.0.5** - runtime error raised if any priority countries do not match those in the main country list
 - **1.0.4** - updated the country list to match the latest ISO 3166 specification
 - **1.0.3** - changed gem name from 'iso-3166-country-select' to just 'country-select'
 - **1.0.2** - forked the plugin and made it into a gem

Copyright (c) 2008 Michael Koziarski, released under the MIT license
