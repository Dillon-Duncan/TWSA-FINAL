# Two-Way South Africa Application

## Table of Contents
1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Installation](#installation)
4. [Running the Application](#running-the-application)
5. [Usage](#usage)
6. [Data Structures](#data-structures)
   - [ServiceRequestTree](#servicerequesttree)
   - [IssueGraph](#issuegraph)
   - [UpdateQueue](#updatequeue)
   - [Event System](#event-system)
7. [Contributing](#contributing)
8. [License](#license)

### Introduction
The Two-Way South Africa application is designed to facilitate communication between citizens and local authorities regarding municipal services. Users can report issues, request services, and stay updated with local events and news. The application features a chat interface for real-time communication and a dashboard for managing service requests.

### Prerequisites
- A modern web browser (Chrome, Firefox, etc.)
- Basic knowledge of HTML, CSS, and JavaScript

### Installation
1. Clone the repository:
   ```
   git clone https://github.com/Dillon-Duncan/TWSA-FINAL.git
   ```
2. Navigate to the project directory:
   ```
   cd twsa
   ```

### Running the Application
1. Open the TWSA.html file in your preferred web browser.
2. The application will load, and you can start interacting with it.

### Usage
- **Report Issues/Request Services**: Click on the "Get Started" button to open the report form.
- **Track Service Requests**: Click on the "Track Now" button to view the status of your requests.
- **Local Events & News**: Click on the "View Events" button to see upcoming events and news in your area.
- **Chat Support**: Use the chat feature to communicate with the bot for assistance.

### Data Structures

#### ServiceRequestTree
The ServiceRequestTree is a binary search tree that organizes service requests based on their IDs. This structure allows for efficient insertion, searching, and traversal of service requests.

- **Searching**: Finding a specific request by ID allows users to quickly access their service requests.
- **Traversal**: The in-order traversal method provides a sorted list of requests, which can be useful for displaying requests in a user-friendly manner.

#### IssueGraph
The IssueGraph is a graph that represents relationships between different service requests. Each request is a vertex, and edges connect related requests.

- **Related Requests**: This structure allows for efficient retrieval of requests, which can help in identifying common issues in a community.

#### UpdateQueue
The UpdateQueue is a queue data structure that manages updates related to service requests.

- **Order of Updates**: This structure ensures that updates are processed in the order they are received, which is crucial for maintaining the correct sequence of information for users.
- **Simplicity**: The queue operations (enqueue, dequeue) make it efficient for handling updates without significant overhead.

#### Event System
The event system manages community events and news. It uses a combination of objects and sets to store events, categories, and locations.

- **Fast Access**: The use of a map for events allows for access to event details by ID, making it quick to retrieve information.
- **Filtering**: The system can efficiently filter events based on type, category, and location, providing users with relevant information without unnecessary delays.
