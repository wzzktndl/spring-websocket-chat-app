# Chat Application

This project is a real-time chat application using Spring WebSocket and message queues. The application allows multiple users to send and receive messages in real-time.

## Overview

The application architecture is designed to handle real-time communication between users. Here's an overview of the key components:

- **Users**: Users can publish messages to a message queue.
- **Message Queue**: The message queue (`john/queue/messages`) receives messages from users.
- **Subscription**: Users subscribe to the message queue to receive messages.
- **ChatRoom**: Manages chat sessions and routes messages to the correct recipients.
- **ChatMessage**: Represents the message structure including details like chat ID, sender ID, recipient ID, content, and timestamp.

## Key Features

- **Real-time Communication**: Users can send and receive messages instantly.
- **Message Queue**: Ensures reliable message delivery.
- **Chat Sessions**: Manages active chat sessions and routes messages appropriately.