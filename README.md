# Node js ocr document reader
It can accept images to be uploaded
Performs the operation of converting image to text using the trained data from `eng.traineddata`.
Returns the text in html format.
## How it works  
After you upload the file, it reads it from request body and saves it under resources. On that saved file we perform the OCR to read over the image pixels.
The result gets returned as http response.  
## How to put it into work  
1. Clone the repo.
2. `npm i` - for installing the packages
3. npm start for starting the application
4. At `http://localhost:8080/upload` make a http post request to  upload the file as formdata with key file
5. Wait for response.
6. You can train the data even more on your needs and for that you have to refer `tesseract.js` documentation.