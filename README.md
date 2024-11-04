# Python-Flask---Image-Background-Removal-API
Background Removal API is a Flask-based web server that provides an API endpoint to remove the background from an image. By sending a local image path via an HTTP POST request, users can retrieve the same image with a transparent background, ideal for applications requiring object isolation.

## Features
- Background Removal: Automatically removes the background from an image, leaving only the foreground with a transparent background.
- Easy Integration: Simple API endpoint for seamless integration with other applications or services.
- Returns PNG with Transparency: The processed image is returned in PNG format, preserving transparency.

## Usage
### Endpoint
POST /removebg

### Request
- Content-Type: application/json
- JSON Payload:
  {
    "image_path": "path/to/your/image.jpg"
  }
- image_path: Local path to the image file you want to process.

## Response
- 200 OK: Processed image with background removed, in PNG format.
- 400 Bad Request: Error if image_path is not provided in the request.
- 404 Not Found: Error if the specified image file is not found.

## Technologies Used
- Python
- Flask
- OpenCV

## Contributing
Contributions are welcome! If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request.

For any questions, feel free to reach me at sahyogshetty12@gmail.com
