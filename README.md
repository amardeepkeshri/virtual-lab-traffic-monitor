# Virtual Lab Traffic Monitor

A cloud-based dashboard for monitoring and classifying virtual lab traffic using AWS services.

## Overview

Virtual Lab Traffic Monitor accepts a traffic count, classifies the traffic level, and stores analysis records in Amazon DynamoDB through an AWS Lambda function.

## Features

- Real-time traffic analysis requests
- Traffic classification into Low, Moderate, and High
- AWS Lambda backend integration
- Amazon DynamoDB record storage and history
- Interactive web dashboard
- Dashboard hosted using Amazon S3 static website hosting

## Traffic Classification

| Traffic Count | Classification |
|---|---|
| 0–50 | Low Traffic |
| 51–100 | Moderate Traffic |
| Above 100 | High Traffic |

## Architecture

1. User enters a traffic count in the dashboard.
2. The frontend sends the request to AWS Lambda.
3. Lambda classifies the traffic count.
4. The result is stored in Amazon DynamoDB.
5. The dashboard displays the analysis result.

## Technology Stack

- HTML, CSS, and JavaScript
- AWS Lambda
- Amazon DynamoDB
- Amazon S3
- Git and GitHub

## Project Structure

```text
virtual-lab-traffic-monitor/
├── index.html
├── README.md
└── .gitignore
```

## Getting Started

1. Clone this repository.
2. Open `index.html` in a browser or use VS Code Live Server.
3. Ensure the configured AWS Lambda Function URL is available and its CORS settings permit the frontend origin.
4. Enter a traffic count and click **Analyze Traffic**.

Note: The cloud-connected features require the AWS backend and appropriate permissions to be configured.

## Team

**Team Name:** 404 Error

## Future Improvements

- Connect persistent DynamoDB history to the dashboard.
- Improve traffic analytics and visualizations.
- Add stronger validation and error handling.
- Improve deployment security and documentation.

## License

No license has been specified yet.
