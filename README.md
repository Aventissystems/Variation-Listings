# Variation Listings

## How to Convert Spreadsheet to JSON

This guide will walk you through the steps to convert a spreadsheet into JSON format.

---

## Steps:

1. **Download the Spreadsheet as CSV**:
   - Open the spreadsheet that contains the data for all products.
   - From the top navigation bar, go to `File` → `Download`.
   - Select `Comma Separated Values (.csv)` as the download option.

2. **Upload the CSV File for Conversion**:
   - After downloading the CSV file, go to [CSV to JSON Converter](https://www.convertcsv.com/csv-to-json.htm).
   - Under **"Step 1: Select your input"**, click the `Choose File` button and upload the CSV.
   - Once the file is uploaded, scroll to **"Step 5: Generate output"**.
   - Click `Download Result` to download the resulting JSON file.

---

## Setting the JSON File and Validating

1. Open the JSON file using any code/text editor.
2. Remove the first empty object (used for headers) and save the file.
3. Go to [JSONLint](https://jsonlint.com/).
4. Paste your JSON code and click `Validate JSON` to check for correctness.

---

## Understanding the JSON Structure

The structure will consist of an array of objects. Each object corresponds to a row in your spreadsheet.

Example:

```json
[
  {
    "url": "https://www.aventissystems.com/dell-p1424h-14-ips-type-c-lcd-portable-monitor/",
    "options": {
      "Choose Screen Size (inches)": [
        {
          "option": "14-inch",
          "link": "https://www.aventissystems.com/dell-p1424h-14-ips-type-c-lcd-portable-monitor/"
        },
        {
          "option": "24-inch",
          "link": "https://www.aventissystems.com/dell-p2423d-24-ips-qhd-1440p-monitor/"
        },
        {
          "option": "27-inch",
          "link": "https://www.aventissystems.com/dell-p2723d-27-ips-qhd-1440p-monitor/"
        },
        {
          "option": "32-inch",
          "link": "https://www.aventissystems.com/dell-p3223de-32-qhd-usb-c-hub-monitor/"
        },
        {
          "option": "34-inch",
          "link": "https://www.aventissystems.com/dell-p3424we-34-curved-usb-c-hub-monitor/"
        }
      ]
    }
  }
]
```

---

## JSON Fields Explained

- **`url`**  
  - The main product URL.

- **`options`**  
  - Variant options (e.g., screen sizes).
  - Each option includes:
    - **`option`**: The specific choice (e.g., "14-inch").
    - **`link`**: URL pointing to that variant.

---
