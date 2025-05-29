# Premium Chat
A modern, real-time chat application with sleek dark UI, private spaces, and seamless collaboration features.

## Features ✨

- **Real-time messaging** with Socket.IO
- **Private chat spaces** with member management
- **Glossy UI** with modern design
- **User authentication** (login/signup)
- **Responsive design** works on all devices
- **Message history** for each space

## Technologies Used 🛠️

### Frontend
- HTML5, CSS3 (with modern Flexbox/Grid layouts)
- JavaScript (ES6+)
- [Socket.IO](https://socket.io/) for real-time communication
- [Font Awesome](https://fontawesome.com/) for icons

### Backend
- Python with Flask
- MongoDB for data storage
- JWT for authentication

## Installation & Setup ⚙️

### Prerequisites
- Python 3.8+
- MongoDB Atlas account or local MongoDB instance

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/premium-chat.git
   cd premium-chat
   ```

2. Set up virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up environment variables:
   Create a `.env` file in the root directory:
   ```
   MONGO_URI=your_mongodb_connection_string
   ```

5. Run the application:
   ```bash
   python app.py
   ```

6. Access the app at:
   ```
   http://localhost:5000
   ```

## Project Structure 📂

```
premium-chat/
├── static/
│   ├── styles.css       # Main stylesheet
│   └── ...              # Other static assets
├── templates/
│   ├── index.html       # Homepage/dashboard
│   ├── view_room.html   # Chat room interface
│   ├── create_room.html # Space creation form
│   ├── login.html       # Login page
│   ├── signup.html      # Signup page
│   └── ...              # Other templates
├── app.py               # Flask application
├── db.py                # Database functions
├── user.py              # User functions
├── requirements.txt     # Python dependencies
└── README.md            # This file
```

## API Endpoints 🌐

| Endpoint | Method | Description |
|----------|--------|-------------|
| `/api/rooms` | GET | Get all rooms for current user |
| `/api/rooms` | POST | Create new room |
| `/api/rooms/<room_id>` | GET | Get room details |
| `/api/rooms/<room_id>/messages` | GET | Get room message history |
| `/api/rooms/<room_id>/members` | GET | Get room members |

## Socket.IO Events 📡

| Event | Direction | Description |
|-------|-----------|-------------|
| `join_room` | Client → Server | Join a chat room |
| `leave_room` | Client → Server | Leave a chat room |
| `send_message` | Client → Server | Send new message |
| `receive_message` | Server → Client | Receive new message |


## Screenshots 📸

### Main
https://github.com/user-attachments/assets/59b04353-bf0b-49ee-8ac3-16b7fa5c56df

### Login and Sign Up
<img width="959" alt="image" src="https://github.com/user-attachments/assets/ab8eb362-ed63-4eff-a8de-9b12f83e6c11" />
<img width="959" alt="image" src="https://github.com/user-attachments/assets/5ecff9eb-dc64-4958-867b-a91df0f665c6" />

### Dashboard
<img width="959" alt="image" src="https://github.com/user-attachments/assets/7d49152c-ba39-4bf3-a3f2-9ee99d3c6a2a" />

### Spaces
<img width="959" alt="image" src="https://github.com/user-attachments/assets/b5da6e88-899e-447d-a302-75f3289a8094" />

### Chat Room
https://github.com/user-attachments/assets/2a1f07af-3ee0-4cd7-9aab-0b688fc1f394


### Create Space
<img width="959" alt="image" src="https://github.com/user-attachments/assets/515514c1-1115-4055-b4a1-a001883520ff" />



## Contributing 🤝

Contributions are welcome! Please follow these steps:

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License 📄

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
