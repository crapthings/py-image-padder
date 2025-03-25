# Changelog

## [0.1.1] - 2025-03-25

### Fixed

- Resolved an issue where the output folder was incorrectly created as a subdirectory when the input folder path ended with a slash ("/").
  - The input folder path is now stripped of trailing slashes before processing.
  - This ensures that the output folder is always created at the same level as the input folder.

- Addressed image orientation problems by implementing automatic EXIF orientation correction.
  - Added use of `ImageOps.exif_transpose()` to correct image orientation before processing.
  - This fix ensures that all images are processed and saved with the correct orientation, regardless of their original EXIF orientation.

### Changed

- Updated the `process_images()` function to handle input paths more robustly.
- Improved image processing to maintain correct orientation across various input image formats.