# ML-Based Waste Sorting System

# Built for [GreenLexicon](https://github.com/GunaPalanivel/GreenLexicon.git)

## Overview

This repository hosts the code for a machine learning-based waste sorting system that helps in classifying various types of waste into correct categories such as recyclables, non-recyclables, and compostables. The tool is designed to be used via a web interface where users can interact with the system through a webcam feed.

## Features

- **Real-time waste identification**: Users can use their webcam to capture images of waste items which are then automatically classified into categories.
- **Support for multiple waste types**: The system can identify various types of waste, including glass, plastic cups, beverage bottles, and more.
- **Dynamic UI updates**: Based on the classification, the UI updates to show the appropriate disposal instructions.
- **Location-based sorting guidelines**: Sorts waste according to local recycling rules (currently supports Toronto and Hamilton).

## Technical Details

- **TensorFlow.js**: Utilizes TensorFlow.js for running the machine learning model directly in the browser.
- **Teachable Machine**: The model was trained using Teachable Machine with the following specifications:
  - Version: 1.3.1
  - Model Name: tm-my-image-model
  - Image Size: 224x224 pixels
- **Model Labels**: The model can classify the following labels:
  - glass
  - clear_containers
  - food_containers
  - plastic_cups
  - beverage_bottles
  - shampoo_bottles
  - clear_cd_dvd_cases
  - plastic_foil_wrappers
  - hot_drink_cups
  - metal_cans
  - paper_products

## Installation

To run this project locally, follow these steps:

1. **Clone the repository**:
   ```
   git clone https://github.com/GunaPalanivel/gitpod.git
   ```
2. **Navigate to the project directory**:
   ```
   cd gitpod
   ```
3. **Open the HTML file in a web browser**:
   - Ensure you have a working webcam connected.
   - Allow the browser to access your webcam when prompted.

## Usage

1. **Start the application**: Open the `index.html` file in a browser to start the application.
2. **Take a photo**: Click on 'Take Photo' to capture an image of the waste item.
3. **Sort the item**: After the photo is taken, the system will analyze the image and display the classification result. Click 'Sort Item' to see the suggested disposal method.

## Contributing

Contributions to this project are welcome. Please adhere to the following guidelines:
- Fork the repository and create your branch from `main`.
- Write clear and concise commit messages.
- Update the README.md with details of changes to the interface or new environment variables.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Support

For any technical issues or questions, please file an issue in the GitHub repository issue tracker.

---

This project aims to facilitate better waste management and recycling practices through the use of cutting-edge technology directly accessible from web browsers. We appreciate your support and contributions to making this tool more effective and widespread.
