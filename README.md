
# Belly Button Biodiversity Dashboard

This project creates an interactive dashboard to explore the Belly Button Biodiversity dataset. The dataset catalogs the bacteria found in the human belly button. Users can select test subjects from a dropdown menu and view dynamic visualizations of the top 10 bacterial species found in their navels, as well as additional metadata and a bubble chart representing bacterial distribution.

## Table of Contents
- [Overview](#overview)
- [Technologies Used](#technologies-used)
- [Features](#features)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Data Source](#data-source)
- [Deployment](#deployment)
- [Acknowledgments](#acknowledgments)

## Overview
The dashboard allows users to:
- Select a test subject ID from a dropdown menu.
- View a horizontal bar chart displaying the top 10 bacterial species (OTUs) found in the test subject.
- View a bubble chart that represents the relative abundance of bacteria.
- Display metadata information such as gender, age, and ethnicity of the selected test subject.
- Dynamically update the visualizations when a new test subject is selected.

## Technologies Used
- **HTML/CSS/Bootstrap**: For structuring and styling the dashboard.
- **JavaScript (ES6)**: For interactivity and rendering the data.
- **D3.js**: To fetch data and manipulate the DOM.
- **Plotly.js**: For creating responsive charts and visualizations.
- **GitHub Pages**: For deploying the dashboard.

## Features
1. **Dynamic Dropdown Menu**: Users can select a test subject from a dropdown menu that updates the charts and metadata panel.
2. **Top 10 OTUs Bar Chart**: Displays the top 10 bacterial species (OTUs) with sample values for each test subject.
3. **Bubble Chart**: Each marker on the bubble chart represents an OTU, with marker size indicating the sample value and marker color representing different OTUs.
4. **Metadata Panel**: Displays demographic information about the selected test subject.
5. **Responsive Design**: The dashboard is mobile-friendly and adjusts to different screen sizes using Bootstrap.

## Getting Started
### Prerequisites
- Basic knowledge of web development (HTML, CSS, JavaScript).
- Git installed on your local machine.

### Steps
1. **Clone the Repository**:
   - Clone this repository to your local machine:
     \`\`\`bash
     git clone https://github.com/your-username/belly-button-challenge.git
     \`\`\`
2. **Open the Project**:
   - Navigate to the project folder and open \`index.html\` in your browser.

3. **View the Dashboard**:
   - The dashboard will be loaded with an interactive dropdown menu to explore different test subjects.

### Optional: Deploying the App to GitHub Pages
1. After completing your changes, commit them to the repository:
   \`\`\`bash
   git add .
   git commit -m "Initial commit"
   git push origin main
   \`\`\`
2. Deploy the project to GitHub Pages by enabling the GitHub Pages feature in your repository settings.

## Project Structure
\`\`\`
belly-button-challenge/
│
├── static/
│   └── js/
│       └── app.js         # Contains D3.js and Plotly.js logic
├── samples.json            # Contains the dataset of bacterial species and metadata
├── index.html              # The main dashboard page
└── README.md               # This file
\`\`\`

### app.js Breakdown
- **buildMetadata()**: Fetches and displays metadata about the selected test subject.
- **buildCharts()**: Builds the bar chart and bubble chart using data filtered by the selected test subject.
- **init()**: Initializes the dashboard, populating the dropdown with sample names and loading the first subject's data.
- **optionChanged()**: Event listener for the dropdown menu that updates the dashboard when a new test subject is selected.

## Data Source
The dataset is hosted on a remote server and is loaded using D3.js. It contains information about different bacterial species (OTUs) and demographic metadata for multiple test subjects. The data file \`samples.json\` is provided for reference but does not need to be accessed locally.

- **URL**: [Belly Button Biodiversity Data](https://static.bc-edx.com/data/dl-1-2/m14/lms/starter/samples.json)

## Deployment
This dashboard is deployed on GitHub Pages and can be accessed [here](https://your-username.github.io/belly-button-challenge).

## Acknowledgments
- This project was completed as part of the Module 14 Challenge at the University of Toronto Boot Camp.
- Special thanks to the instructors and TAs for their support.
