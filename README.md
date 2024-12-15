# Image Padder

Image Padder is a command-line tool to pad and resize images in a folder. It supports jpg, jpeg, png, webp, and avif formats.

## Installation

```sh
pip install image-padder
```

## Usage

```sh
image-padder <input_folder> [options]
```

```
Options:
- `--ratio`: Target aspect ratio (width/height). Default is 1.0 (square).
- `--bg-color`: Background color in hex format (e.g., #FFFFFF). Default is #000000 (black).
- `--output-size`: Output size after padding, specified as WIDTH HEIGHT.

Example:
```

```sh
image-padder /path/to/image/folder --ratio 1.5 --bg-color "#FFFFFF" --output-size 800 600
```


This will process all supported images in the specified folder, pad them to a 3:2 aspect ratio with a white background, and resize them to 800x600 pixels.

## License

This project is licensed under the MIT License.