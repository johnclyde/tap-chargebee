# Changelog

## 1.3.0
  * Added comments stream [#52](https://github.com/singer-io/tap-chargebee/pull/52)
  * Added include_deleted configuration [#58](https://github.com/singer-io/tap-chargebee/pull/58)
  * Added undocumented fields [#69](https://github.com/singer-io/tap-chargebee/pull/69)

## 1.2.2
  * Update the schema glob so that we include all schemas in the package distribution [#73](https://github.com/singer-io/tap-chargebee/pull/73)

## 1.2.1
  * Add a `MANIFEST.in` file to include schema files in the `tap-chargebee` package [#72](https://github.com/singer-io/tap-chargebee/pull/72)

## 1.2.0

  * Remove all minimum/maximum and minLength/maxLength [#45][#45]
  * Fix JSONDecodeError in Invoices and Transactions streams [#51][#51]
  * Add Tiersprice attribute [#53][#53]
  * Updated integration test to cover product catalog v1 and v2 [#63][#63]
  * Add additional fields from API [#64][#64]
  * Upgraded event stream schema [#57][#57]
  * Updated Bookmark handling, date without tz will updated in UTC tz format [#54][#54]

[#45]: https://github.com/singer-io/tap-chargebee/pull/45
[#51]: https://github.com/singer-io/tap-chargebee/pull/51
[#53]: https://github.com/singer-io/tap-chargebee/pull/53
[#63]: https://github.com/singer-io/tap-chargebee/pull/63
[#64]: https://github.com/singer-io/tap-chargebee/pull/64
[#57]: https://github.com/singer-io/tap-chargebee/pull/57
[#54]: https://github.com/singer-io/tap-chargebee/pull/54

## 1.1.2
  * Fix domain name comparison bug [#67](https://github.com/singer-io/tap-chargebee/pull/67)

## 1.1.1
  * Add an error message when we get an unexpected response from the Configurations API [#62](https://github.com/singer-io/tap-chargebee/pull/62)

## 1.1.0
  *  Adds support for Item Model, Multi-decimal (for Plan Model), and Account hierarchy (for Plan Model) [#56](https://github.com/singer-io/tap-chargebee/pull/56)
  * Organized the folder structure:
      a. common(common schemas to both plan model and item model)
      b. item_model
      c. plan_model
  * Introduces two new streams: ITEM_MODEL_AVAILABLE_STREAMS, PLAN_MODEL_AVAILABLE_STREAMS

## 1.0.3
  * Fix invalid JSON from #44

## 1.0.2
  * Remove `maxLength` from `payment_sources` schema to address certain integrations having IDs of greater length than specified, and make the schema more flexible as the API evolves [#44](https://github.com/singer-io/tap-chargebee/pull/44)

## 1.0.0
  * No change from 0.0.12

## 0.0.12
  * Add `custom_fields` to plans, addons, customers, and subscriptions [#9](https://github.com/singer-io/tap-chargebee/pull/9)

## 0.0.3
  * Add `credit_notes` stream [#2](https://github.com/singer-io/tap-chargebee/pull/2)
