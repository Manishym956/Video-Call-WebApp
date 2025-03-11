# Video-Call-WebApp

A simple and interactive video-calling web application built using WebRTC. This app allows users to connect with others via video calls directly in their browser. You can also connect to the call using your mobile phone by exposing your local server to the internet using `ngrok`.

---

## Features
- **Real-time video calls**: Connect with others using WebRTC.
- **Multi-tab support**: Test the app by opening multiple tabs in your browser.
- **Mobile support**: Share the call link with your mobile phone or friends.
- **End call button**: Easily disconnect the call.

---

## Prerequisites
Before running the project, ensure you have the following installed:
- [Node.js](https://nodejs.org/) (v14 or higher)
- [npm](https://www.npmjs.com/) (usually comes with Node.js)
- [Chocolatey](https://chocolatey.org/) (for installing `ngrok` on Windows)
- [ngrok](https://ngrok.com/) (for exposing your local server to the internet)

---

## Getting Started

### 1. Fork and Clone the Repository
1. Fork this repository to your GitHub account.
2. Clone the forked repository to your local machine:
   ```bash
   git clone https://github.com/your-username/Video-Call-WebApp.git
   cd Video-Call-WebApp
   ```

### 2. Install Dependencies
Install the required dependencies using npm:
```bash
npm install
```

### 3. Run the Application
Start the development server:
```bash
npm run start
```
- The app should automatically open in your browser at `http://localhost:9000`.
- If it doesn’t open automatically, manually navigate to `http://localhost:9000` in your browser.

---

## Testing the Application

### 1. Multi-Tab Testing
1. Open two tabs in your browser and navigate to `http://localhost:9000` in both tabs.
2. Enter a username in both tabs and click **Create**.
3. In the contact list, click the **phone button** next to the username to initiate a call.
4. The two tabs will connect via video call.
5. Use the **End Call** button to disconnect.

### 2. Mobile Testing
1. **Install ngrok** (if not already installed):
   - Open PowerShell as Administrator and run:
     ```bash
     choco install ngrok
     ```
2. **Authenticate ngrok**:
   - Run the following command in PowerShell:
     ```bash
     ngrok config add-authtoken 2uAXjKTFL8luLFHYzu2pu0N58ri_3JP6ZNLu2o1KXnwHpp9TN
     ```
3. **Expose your local server**:
   - Run the following command in PowerShell:
     ```bash
     ngrok http http://localhost:9000
     ```
   - Copy the `ngrok` link (e.g., `https://abcd1234.ngrok.io`) from the terminal.

4. **Share the link**:
   - Open the `ngrok` link on your mobile phone or share it with friends.
   - Enter a username and click **Create** to join the call.

5. **Keep the server running**:
   - Ensure the PowerShell window running `ngrok` remains open while testing.

---

## Project Structure
```
Video-Call-WebApp/
├── public/              # Static files (HTML, CSS, JS)
├── src/                 # Source code
├── package.json         # Project dependencies and scripts
├── README.md            # Project documentation
└── ...                  # Other configuration files
```

---

## Technologies Used
- **WebRTC**: For real-time video and audio communication.
- **Node.js**: For the backend server.
- **Express.js**: For serving static files.
- **Socket.io**: For real-time signaling between clients.
- **ngrok**: For exposing the local server to the internet.

---

## Contributing
Contributions are welcome! If you’d like to contribute to this project, please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature-name`).
3. Commit your changes (`git commit -m "Add your feature"`).
4. Push to the branch (`git push origin feature/your-feature-name`).
5. Open a Pull Request.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments
- Thanks to WebRTC for enabling real-time communication.
- Thanks to ngrok for making local development easier.
- Connect with me on [LinkedIn](https://www.linkedin.com/in/manish-y-m-233496326/) for any questions or feedback.

---

## Happy Coding! 🚀
Enjoy using the Video-Call-WebApp! If you have any questions or feedback, feel free to open an issue or reach out.
