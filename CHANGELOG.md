# Changelog

## v0.6.0
* Features
  * Support json-api spec `include` query param. (@green-arrow)
  * Support json-api spec `fields` query param. (@green-arrow)
  * Add meta info support

## v0.5.0
* Features:
  * Support custom ids in relationships. (@green-arrow)
  * Adds error rendering support to Phoenix view.
* Deprecations:
  * Use key `serializer` instead of `include` when defining relationships.
* Dependencies:
  * Ecto is now a required (non-optional) dependency.

## v0.4.0
* Features:
  * Adds support for pagination links w/ Scrivener or via opts. (@vysakh0)
* Bugfixes:
  * Properly serialize empty relationships. (@dmarkow)

## v0.3.1

* Bugfixes
  * Adds optional Ecto dependency to fix compliation issue.

## v0.3.0

* **Breaking**:
  * Raises exception if ecto relationship is not pre-fetched.
* Features:
  * Adds JaSerializer.ErrorSerializer
  * Adds JaSerializer.EctoErrorSerializer
  * Pre-defines formats for Ecto built in types.

## v0.2.0

* Features:
  * Add Phoenix integration w/ JaSerializer.PhoenixView.
  * Infer type from module name.
  * Add `attributes/2` callback w/ default implementation based on `attributes/1` macro.
  * Add JaSerializer.ContentTypeNegotiation plug for setting content type.
  * Add JaSerializer.Deserializer plug for param normalization.
* Deprecations:
  * Remove `serialize` macro in favor of `type/0` callback.

## v0.1.2

* Bugfix
  * Added non-fallback formatters for simple data types to improve out of the box performance.

## v0.1.1

* Bugfixes:
  * Fix issues w/ include chains that resulted in infinite loops.

## v0.1.0

* Features:
  * Add config option for formatting keys as underscored or dasherized.
* Bugfixes:
  * Serialize include chains w/o duplicates.

## v0.0.1

* Initial release.
