---
layout: default
active: changelog
---
# Release notes

## 4.4.0 

* This is the first release under the new package name podio-community/podio-php. It contains several fixes and minor improvements and should generally be backwards compatible to podio/podio-php v4.3.0.
* Several fixes and improvements: [See in repository](https://github.com/podio-community/podio-php/compare/4.3.0...v4.4.0)

## 4.3.0

* Add support for [Flows](https://developers.podio.com/doc/flows)

## 4.2.0

* Add `update_reference` and `count` to `PodioTask`
* Create `PodioVoting`
* Add low memory file fetch
* Verify TLS certificates
* Minor bug fixes

## 4.1.0

* Fix `PodioFile` `get_raw` concatenation
* Fix user model `mail` return value
* Add votes property and support for options when getting item
* Add missing properties to Comment model
* Add description to space model
* Make upload function compatible with `PHP 5.6`
* Add activation method for platform
* Add search method for platform
* Add method for org bootstrap for platform

## 4.0.2

* Minor bugfixes

## 4.0.1

* Minor bugfixes
* Make `authenticate_with_password` actually work
* Support image downloads at different sizes

## 4.0.0

* Introduced PodioCollection to make it easier to work with collections. Removed `field` and related methods from `PodioItem` and `PodioApp` objects. Use the new array access interface instead. [See details]({{site.baseurl}}/objects).
* [Made Podio\*Itemfield objects more intuitive to work with]({{site.baseurl}}/items)
* Unit tests added for `PodioCollection` (and subclasses), `PodioObject` and `Podio*ItemField` classes
* Improved debugging options and added Kint for debugging
* Bug fixed: [Handle GET/DELETE urls with options properly.](https://github.com/podio/podio-php/commit/f1f81c0c8ff4584827bf63b5f023f659e536de5c)
* Made `__attributes` and `__properties` private properties of `PodioObject` instances to underline that they shouldn't be used
