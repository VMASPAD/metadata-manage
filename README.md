# Image Metadata Extractor

This simple web application allows you to extract metadata from your images using JavaScript. It utilizes the ExifReader library to read the metadata embedded in the image files.

## How to Use

1. Clone or download the repository to your local machine.
2. Install with `npm i`
3. Run `npm run dev`

## Usage Instructions

1. Click on the "Choose File" button to select an image from your device.
2. Once the image is selected, the application will display a preview of the image.
3. The metadata extracted from the image will be displayed in a table below the image preview.
4. Each row in the table represents a metadata entry, showing the type, value, and description.

## Example

Suppose you have an image file named `example.jpg`. After opening the `index.html` file in your web browser, you select `example.jpg` using the file input. The application will then display the metadata extracted from `example.jpg`, such as the camera model, resolution, date taken, etc.

<img src="test.jpg" alt="Imagen de unas nubes" width="200">

Result:
`
{
    "Bits Per Sample": {
        "value": 8,
        "description": "8"
    },
    "Image Height": {
        "value": 768,
        "description": "768px"
    },
    "Image Width": {
        "value": 768,
        "description": "768px"
    },
    "Color Components": {
        "value": 3,
        "description": "3"
    },
    "Subsampling": {
        "value": [
            [
                1,
                34,
                0
            ],
            [
                2,
                17,
                1
            ],
            [
                3,
                17,
                1
            ]
        ],
        "description": "YCbCr4:2:0 (2 2)"
    },
    "JFIF Version": {
        "value": 257,
        "description": "1.1"
    },
    "Resolution Unit": {
        "value": 0,
        "description": "None"
    },
    "XResolution": {
        "value": 1,
        "description": "1"
    },
    "YResolution": {
        "value": 1,
        "description": "1"
    },
    "JFIF Thumbnail Width": {
        "value": 0,
        "description": "0px"
    },
    "JFIF Thumbnail Height": {
        "value": 0,
        "description": "0px"
    },
    "FileType": {
        "value": "jpeg",
        "description": "JPEG"
    }
}
`
The result varies depending on the image, with less or more information available.
## Note

- This application only extracts metadata from image files (JPEG, PNG, etc.).
- If an error occurs during the metadata extraction process, the application will display an error message in the table.

For more details on how the metadata extraction works, please refer to the source code.

