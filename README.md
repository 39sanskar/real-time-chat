- Real-Time Chat Application Using Raw WebSockets (Node.js)
- Design and implement a real-time chat application using raw WebSockets in Node.js with the following features and constraints:
- 1. Chat Room Management (Admin Controls)
- An admin should be able to create and manage chat rooms (sessions). Each chat room must support the following configurable properties:
- Name: A unique identifier for the chat room
- Start Time: The scheduled time at which the chat session becomes active
- Is Open: A boolean flag indicating whether users are allowed to join and send messages
- Cool-down Time: A time interval that limits how frequently users can send messages

- 2. User Participation
- Users should be able to join an active chat room.
- Once inside a room, users can send real-time messages to other participants, subject to the room’s rules (e.g., cool-down time and open status).

- 3. Message Upvoting System
- Users should be able to upvote messages posted in the chat.
- Each message must maintain a real-time count of upvotes.

- 4. Message Highlighting & Moderation
- If a message receives more than 3 upvotes, it should be automatically moved to a highlighted section (e.g., “Top Messages”).
- If a message receives more than 10 upvotes, the system should notify or alert the admin, indicating that the message requires an official response or attention.

- 5. Real-Time Communication
- All interactions (joining rooms, sending messages, upvoting, and alerts) must occur in real time using raw WebSockets, without relying on higher-level abstractions such as Socket.IO.
