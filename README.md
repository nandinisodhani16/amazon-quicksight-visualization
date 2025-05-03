# Amazon Bestsellers Analysis using AWS QuickSight

This project demonstrates how to analyze and visualize data using *AWS S3* and *Amazon QuickSight*.

## Features

- Dataset stored in Amazon S3
- Manifest file used to load data into QuickSightV
- Dashboard and visuals created in QuickSight

## Technologies Used

- AWS S3
- Amazon QuickSight
- JSON (Manifest)
- CSV (Dataset)
- GitHub

## Dashboard Screenshots

### Dashboard 1
![Dashboard](https://github.com/nandinisodhani16/amazon-quicksight-visualization/blob/main/Screenshot%202025-05-03%20170811.png)
 
 ### Dashboard 2
 ![Dashboard](https://github.com/nandinisodhani16/amazon-quicksight-visualization/blob/main/Screenshot%202025-05-03%20171057.png)

## Setup Steps

1. Upload your dataset to Amazon S3.
2. Create a manifest.json like this:
```json
{
  "fileLocations": [
    {
      "URIs": [
        "s3://nandini-amazon-project/Amazon-Bestseller-Dataset.csv"
      ]
    }
  ],
  "globalUploadSettings": {
    "format": "csv",
    "delimiter": ",",
    "textqualifier": "\"",
    "containsHeader": "true"
  }
}