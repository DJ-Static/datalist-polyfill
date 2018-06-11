# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [Unreleased]
### Added
- #GH-16 correction as an enhancement to the current functionality

## [1.13.2] - 2018-06-11
### Changed
- Focusing the input[list] after selecting a suggestion, as in #GH-18

## [1.13.1] - 2018-06-04
### Changed
- Some code refactoring, nothing really serious
By the way, it was polyfills 1st birthday one month ago. Yeah !!!

## [1.13.0] - 2018-05-28
### Added
- Thanks to @eddr and @Kravimir for inspiring me via #GH-5 that there should be another possibility on defining value and label for the suggestions. As the browser vendors (GC vs. the others) don't seem to be aligned on this topic, I've decided to enable the label-attribute to serve as the definitive label being displayed, even if a value is being defined differing from the label. Check out the „Different ways of defining an option“ section on the demo page regarding this topic.

### Changed
- The docs. And changed (dependencies) and added (jsdelivr) badges. I like badges.
- As well as extracted the CHANGELOG to an external file.

## [1.12.3] - 2018-05-04
### Fixed
- @wlekin thankfully mentioned (extracted to #GH-15) that the polyfilling `select` gets positioned incorrectly underneath the `input[list]` element on iOS.

## [1.12.2] - 2018-05-01
### Fixed
- Thank you @IceCreamYou for fixing the case sensitive focusOut -> focusout event name

## [1.12.1] - 2018-04-07
### Changed
- simple (code) style changes (plus added editorconfig to keep it that way) and typo 

## [1.12.0] - 2018-03-18
### Added
- @ottoville thankfully contributed by mentioning and implementing the feature of emitting an event when item in datalist is selected

## [1.11.2] - 2018-03-17
### Changed
- @mertenhanisch has styled the code according to more „standard“ formatting and also improved the wording of the documentation, which is awesome.
- And @mitchhentges thankfully supports on reviewing your great community support and ensures to the keep the wheels turning on the development of this projects.
Many kudos to the both of you !!!

## [1.11.1] - 2017-11-24
### Fixed
- @hryamzik thankfully mentioned by #GH-7 that the polyfilling `select` gets positioned incorrectly in case of the `input[list]` element being styled as a block-level element.

## [1.11.0] - 2017-10-08
### Changed
- I'm very thankful for @ailintom mentioning the missing IE9 support with #GH-2, which is still relevant (at least and maybe foremost) for the Windows Vista users.
- Additionally @Kravimir thankfully brought to my attention, that IE9 handles the `option` subelements quite restricted - so I've added a section regarding IE9 support to the demo page with the additional two lines of HTML, that you'll need to add in case you also need / want to still support IE9 in your projects, as well as changed the JavaScript code to even also support IE9.

## [1.10.3] - 2017-10-07
### Changed
- Added a comment regarding IE9 - and some simple code styling.

## [1.10.2] - 2017-09-26
### Fixed
- Simple corrections.

## [1.10.1] - 2017-09-25
### Fixed
- Simple bugfix, that came up through the latest implementation on the up and down arrow keys.

## [1.10.0] - 2017-08-16
### Changed
- Added the ability to open the datalist on the up and down keys even in case that no value has been provided - this seems to be intentionally and even also adapts the behavior by supporting browsers.

## [1.9.0] - 2017-07-20
### Changed
Regarding the changes out of release version 1.6.0 to emulate the expected UI quite nicely, I was still struggling with using that hacky solution (`multiple` attribute) and even also of how to prevent multiple selections on the polyfilling select.
- Actually the attribute `size` came to my attention, which much better fits the requirements and behaves as designed quite perfectly. Chapeau!

## [1.8.1] - 2017-07-18
### Fixed
- Bugfix regarding the handling of the label values.

## [1.8.0] - 2017-07-24
### Changed
- Restricted the polyfill to only work with relevant input types; we’d like to exclude the ones that even already need another polyfill to „work“ correctly or have a meaningful UI, like e.g. color or date-related ones, as those polyfills should handle the support of the datalist themselves depending on their own functionality.

## [1.7.0] - 2017-06-29
### Added
- As mentioned by @aFarkas [within his review](https://github.com/h5bp/html5please/issues/18), `option` elements could be of some different formats. This release especially follows [the spec](https://www.w3.org/TR/html5/forms.html#the-datalist-element) regarding the aspect that „Each suggestion has a value and a label.“.

## [1.6.2] - 2017-06-28
### Changed
- Optimized the behavior to select the entries within the polyfilling `select[multiple]` on using the up and down arrow keys from the polyfilled `input[list]`.

## [1.6.1] - 2017-06-16
### Changed
- Introduced speaking variables for the different keycodes.
- And implemented some feedback by flow.
- As well as additional code simplifications.

## [1.6.0] - 2017-06-16
### Changed
This is so far the biggest and greatest update !
- Depending of the feedback by Michael the visual appearance has changed and will better emulate the expected layout as in other browsers (on non-touch interactions). That for the script is creating the polyfilling select as a multiple-selection type, which emulates the expected „form“ better.
- And better positioning as well as styling the polyfilling select according to the input field, like e.g. even also set the polyfilling selects border-radius equally as the one by the polyfilled input.

## [1.5.0] - 2017-06-10
### Changed
- Simplified the styling and got rid of the external CSS files / dependency. You could remove that one now. Yeah!

## [1.4.0] - 2017-06-09
### Added
- Added RTL text-direction support

## [1.3.0] - 2017-05-30
### Added
- Added support for multiple email addresses, separated by comma.

### Changed
- And again, updated documentation slightly. And demo accordingly.

## [1.2.1] - 2017-05-29
### Changed
- Simple code style modifications. Because style matters.

## [1.2.0] - 2017-05-29
### Added
- Added .options (for `datalist` elements) and .list (for `input` elements) properties according to the specs.

## [1.1.2] - 2017-05-22
### Changed
- Further simplified the code, so that we could even skip the `.matches()` polyfill. Yeah.
- And documentation updates.

## [1.1.1] - 2017-05-10
### Fixed
- fixed another simple bug that lead to an incorrect index being selected - let's skip this, as it's not even the standard behaviour

## [1.1.0] - 2017-05-09
### Fixed
- some small corrections

## [1.0.3] - 2017-05-09
### Changed
- better preselection on entries within the dropdown depending on the inputs value

## [1.0.2] - 2017-05-08
### Added
- added a `package.json` file

## [1.0.1] - 2017-05-08
### Fixed
- Small, but important typo. :-) Thanks @Fyrd for mentioning this.

## [1.0.0] - 2017-05-04
### Added
- First release.