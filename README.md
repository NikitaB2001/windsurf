# Social Media Listening Dashboard

A comprehensive dashboard for analyzing social media performance across Instagram, TikTok, and YouTube for brands like Marks & Spencer and Next Retail.

## Project Overview

This dashboard provides detailed analytics and insights based on Excel datasets for social media performance. The application includes:

- Multi-step setup wizard for configuring brands and platforms
- Comprehensive dashboard with multiple visualization components
- Filtering capabilities by platform, date range, hashtag, sentiment, and brand
- Dynamic recalculation of metrics based on applied filters

## Features

### Setup Flow
1. **Login Screen** - Simple authentication
2. **Brand Setup** - Configure main brand and hashtags
3. **Competitor Setup** - Add and validate competitor brands
4. **Platform Selection** - Choose which platforms to analyze
5. **Confirmation** - Review and confirm setup choices

### Dashboard Components
1. **Brand Performance** - Overall engagement metrics across platforms
2. **Engagement Insights** - Detailed engagement rate analysis
3. **Hashtag Analysis** - Top performing hashtags visualization
4. **Sentiment Analysis** - Sentiment distribution and trends
5. **Competitor Monitoring** - Comparative analysis with competitors

## Data Sources

The dashboard exclusively uses Excel datasets located in the `data` folder. No external APIs or random data are used.

## Technology Stack

- React for UI components
- Chart.js for data visualization
- XLSX library for parsing Excel files
- CSS for styling

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn

### Installation

1. Clone the repository
2. Install dependencies:
   ```
   npm install
   ```
3. Start the development server:
   ```
   npm start
   ```

### Data Files

Place your Excel data files in the `data` folder with the following naming convention:
- `[BrandName]_[Platform].xlsx` (e.g., `Marks&Spencer_Instagram.xlsx`)

## Usage

1. Log in with any credentials (demo mode)
2. Follow the setup wizard to configure your dashboard
3. Use the filters to refine the data displayed
4. Analyze the visualizations and metrics

## Project Structure

```
/src
  /components
    /Dashboard
      - Dashboard.js         # Main dashboard component
      - BrandPerformance.js  # Brand performance visualization
      - EngagementInsights.js # Engagement rate analysis
      - HashtagAnalysis.js   # Hashtag visualization
      - SentimentAnalysis.js # Sentiment distribution
      - CompetitorMonitoring.js # Competitor comparison
      - Dashboard.css        # Dashboard styling
    /Login
      - Login.js             # Login component
      - Login.css            # Login styling
    /Setup
      - SetupWizard.js       # Setup flow coordinator
      - BrandSetup.js        # Brand configuration
      - CompetitorSetup.js   # Competitor configuration
      - PlatformSelection.js # Platform selection
      - ConfirmationModal.js # Setup confirmation
      - Setup.css            # Setup styling
  /utils
    - dataProcessor.js       # Data processing utilities
  - App.js                   # Main application component
  - index.js                 # Application entry point
/data
  - [Excel files]            # Data source files
```

## Notes

- This is a client-side only application with no backend
- All data processing happens in the browser
- Sentiment analysis uses basic keyword matching
- Time-based visualizations use simplified calculations
