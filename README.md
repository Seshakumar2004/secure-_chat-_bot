🔐 Secure Chat App with End-to-End Encryption
A lightweight, real-time chat application built using Flask, Flask-SocketIO, and JavaScript, with end-to-end encryption using AES to ensure that only the intended recipient can view the message. The app supports secure user registration and login using bcrypt for password hashing.

🚀 Features
✅ User Registration & Login (with hashed passwords)
✅ Real-Time Chat using WebSockets (Socket.IO)
✅ AES-based End-to-End Message Encryption
✅ Session-based Authentication
✅ Recipient-Specific Messaging (only recipient sees the message)
✅ Clean UI with Cybersecurity Theme
✅ Logout Option
✅ Message not visible to the sender after sending
🛠️ Tech Stack
Layer	Technology
Backend	Python, Flask, Flask-SocketIO
Frontend	HTML, CSS, JavaScript
Encryption	AES (Advanced Encryption Standard)
User Storage	JSON File
Security	bcrypt (Password Hashing)


🧰 Installation
Clone the repository
git clone https://github.com/Ranjith1410/secure-chatbot
cd secure-chat-app
Create a virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install the dependencies
pip install -r requirements.txt
Run the Flask application
python app.py
Open your browser
Visit http://localhost:5000 to access the app.


📁 Project Structure
project/
├── app.py                  # Main Flask backend
├── crypto_utils.py         # AES Encryption/Decryption functions
├── users.json              # Stores registered users and hashed passwords
├── templates/
│   ├── register.html       # Registration page
│   ├── login.html          # Login page
│   └── chat.html           # Chat interface
├── static/
│   ├── js/
│   │   ├── script.js       # SocketIO + AES frontend logic
│   │   └── crypto-utils.js # AES encryption/decryption logic
│   └── css/
│       └── style.css       # Cybersecurity-themed styling
├── requirements.txt        # Python dependencies
└── README.md               # Project documentation


📌 Usage Notes
Users must register only once.
All messages are encrypted before sending and only decrypted by the recipient.
Messages are not stored; this ensures privacy and data security.
Ensure multiple users open different browser sessions for full testing.


✅ Conclusion
The Secure Chat App successfully demonstrates a real-time communication system with strong security measures in place. By integrating AES-based end-to-end encryption and secure password hashing, the application ensures that sensitive user data and messages remain private. This project highlights the importance of secure communication in the digital age and showcases how Flask and Socket.IO can be used to build scalable, privacy-focused web applications. The modular structure, clean interface, and security-first approach make it a strong foundation for further enhancements like group chats, media sharing, or cloud storage integration.

✅ "Secure your messages. Empower your communication." 🔐
