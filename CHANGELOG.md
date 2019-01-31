# CHANGELOG.md

## 3.0.1

- Removed the option to *not* show a grid of files when setting `multiple` on the input. The logic messiness wasn't worth it considering we don't really need the option now that we have a grid view for multiple images.

- Cleaned up logic flow.

- *Added* buttons for deleting indivudual files in the grid view. Also includes the option to disable this feature.

- Added a deletion event that gets triggered when a file is deleted.

- Updated the README accordingly with this changes.

## 3.0.0

- Rewrite of the library code. Made the handling of multiple images a bit more clear. Tried to clean up the logic and set properties only a single time when needed. Should all be a bit more clear now.
- Showing the grid of images in the case of multiple is now the default setting. To stop that, pass
`{showMultiple: false}` when initializing the class.
- All further options are now set up to be passed in a single `options` object during initialization. This will be good for any further additions.
- Restructured how the `imageSelected` event is done as to make it a bit easier to use - see updated documentation on how to use that event.
- `custom-file-container__image-preview__active` was changed to `custom-file-container__image-preview--active` to be inline with BEM style.
- Added overflow to multiple image pane, so when there's a ton of images it doesn't just keep growing in height.

## 2.1.2 (2018-09-21)

Merged in #12 from @firstor - support for .gifs in both single and multiple previews.