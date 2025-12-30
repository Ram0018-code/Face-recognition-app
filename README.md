👁️ Face Recognition Access System

A real-time biometric security application that runs entirely in the browser. This project uses machine learning models to detect faces, register a user's biometric data, and grant or deny access based on facial recognition.

[🔗 VIEW LIVE DEMO HERE]([PASTE YOUR NETLIFY LINK HERE])

📸 Screenshots

<!-- Tip: Upload screenshots to your repo and link them here for a better look -->

🚀 Features

Real-Time Detection: Uses the webcam to detect faces at 30+ FPS.

One-Click Registration: Instantly captures and stores facial descriptors in browser memory.

Access Control Logic: Compares live video feed against registered data to Grant or Deny access.

Client-Side Privacy: No video data is sent to a server; all processing happens locally on the user's device.

Futuristic UI: Custom HUD (Heads-Up Display) overlay using HTML5 Canvas.

🛠️ Tech Stack

Core: HTML5, CSS3, Vanilla JavaScript.

ML Library: face-api.js (built on TensorFlow.js).

Models Used: TinyFaceDetector (for speed) and FaceLandmark68Net.

Hosting: Netlify / GitHub Pages.

⚙️ How It Works

Initialization: The app loads pre-trained neural network models (tinyFaceDetector, faceLandmark68Net, faceRecognitionNet) from the CDN.

Registration: When the user clicks "Register", the system extracts a 128-float descriptor vector of the face currently in view.

Inference: During scanning, the app continuously calculates the Euclidean distance between the live face and the stored descriptor.

Decision: If the distance is below the threshold (0.6), access is GRANTED. Otherwise, it is DENIED.

🏃‍♂️ How to Run Locally

Clone the repository:

git clone [https://github.com/YourUsername/face-recognition-access.git](https://github.com/Ram0018-code/face-recognition-app.git)


Navigate to the project folder.

Important: Due to browser security restrictions on camera access, you must run this on a local server (you cannot just double-click index.html).

Option A (VS Code): Right-click index.html and select "Open with Live Server".

Option B (Python): Run python -m http.server in the terminal and open localhost:8000.

🤝 Contributing

Feel free to fork this project and add features like:

Multi-user registration.

Voice greeting upon access.

Database integration (Firebase/Supabase) for persistent storage.

📝 License

This project is open source and available under the MIT License.

Created by [Your Name] - Connect with me on [LinkedIn]([PASTE YOUR LINKEDIN URL])
