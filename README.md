# Measurement form test (Angular)

A minimal, single-page Angular experience (loaded directly from CDN builds) to try the
`/api/MeasurementForm/UploadImage` endpoint on `http://localhost:5233`.

## Running the page

Because the page uses ES modules and an import map, open it from a simple local web server
instead of the `file://` scheme. For example:

```bash
python -m http.server 4200
```

Then visit [http://localhost:4200](http://localhost:4200) in your browser.

## Using the tester

1. Drag and drop an image into the drop zone or click **Choose file** to browse.
2. (Optional) Enter a value for the `t` form field.
3. Click **Upload** to POST the file to `http://localhost:5233/api/MeasurementForm/UploadImage`.
4. The JSON response is shown in the read-only text area. Use **Copy** to copy it or **Clear** to
   reset the output.

Ensure your API allows cross-origin requests from the host serving this page if you are testing
from a different origin.
