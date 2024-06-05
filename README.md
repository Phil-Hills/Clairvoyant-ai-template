# Clairvoyant-ai-template
# Clairvoyant AI Template

This repository contains a template for the Clairvoyant AI project, which includes a Chrome extension, a CRM app, and ClairBot, the flagship product designed for real estate agents. Clairvoyant AI utilizes generative AI and cloud technologies to enhance client relationship management and sales processes.

## Directory Structure

- **chrome-extension/**: Contains the Chrome extension files.
  - `background.js`
  - `content.js`
  - `manifest.json`
  - `popup/`: Contains the popup files (`popup.html`, `popup.css`, `popup.js`).

- **crm-app/**: Contains the CRM app files.
  - `index.html`
  - `styles.css`
  - `app.js`
  - `genai-integration.js`
  - `appsheet-integration.js`
  - `components/`: Contains the component files (`lead-management.js`, `client-communication.js`).

- **clairbot/**: Contains the ClairBot files.
  - `clairbot.html`
  - `clairbot.css`
  - `clairbot.js`
  - `lead-scoring.js`
  - `marketing-suggestions.js`
  - `prospect-engagement.js`

## Setup Instructions

### Prerequisites

- Node.js (v14 or higher)
- npm (v6 or higher)
- A Google Cloud account with Vertex AI and Google Sheets API enabled
- A Google service account with a key file

### Installation

1. **Clone the repository**:
    ```sh
    git clone https://github.com/phil-hills/clairvoyant-ai-template.git
    cd clairvoyant-ai-template
    ```

2. **Install dependencies**:
    ```sh
    npm install
    ```

3. **Set up environment variables**:
    - Create a `.env` file in the root directory and add your API key:
      ```plaintext
      GEMINI_API_KEY=your-gemini-api-key
      ```

4. **Add your Google service account key**:
    - Save your Google service account key file as `service-account-file.json` in the root directory.

5. **Start the server**:
    ```sh
    node server.js
    ```

## Adding the Extension to Chrome

1. **Build the extension**:
    - Ensure the following files are in the `chrome-extension` directory:
      - `background.js`
      - `content.js`
      - `manifest.json`
      - `popup/`: Contains `popup.html`, `popup.css`, `popup.js`.

2. **Load the extension in Chrome**:
    - Open Chrome and go to `chrome://extensions/`.
    - Enable “Developer mode” by toggling the switch in the top right corner.
    - Click on “Load unpacked” and select the `chrome-extension` directory.

## Using ClairBot

1. **Open ClairBot**:
    - Click on the ClairBot icon in your Chrome toolbar to open the chat interface.
    - Interact with ClairBot by typing your queries into the text box and pressing “Send.”

2. **Export chat history to Google Sheets**:
    - Click the “Export to Google Sheets” button to export your chat history.
    - A link to the Google Sheet will be provided once the export is successful.

## Troubleshooting

- **Server errors**:
  - Ensure your environment variables are correctly set in the `.env` file.
  - Verify that your Google service account key file is correctly placed in the root directory.

- **Extension issues**:
  - Ensure all extension files (`popup.html`, `popup.css`, `popup.js`, `manifest.json`) are present and correctly referenced.
  - Check the Chrome console for any errors and address them accordingly.

## Contribution

Feel free to fork this repository and submit pull requests. Contributions that improve the functionality and usability of Clair are welcome.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

---

Clairvoyant AI is designed to make your browsing experience more efficient and productive by providing a powerful AI assistant right at your fingertips. Enjoy seamless interactions and easy data management with Clair!
