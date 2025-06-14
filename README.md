# 🧠 Memory App — System & Database Design

This repository is dedicated to tracking and organizing the **system architecture** and **database design** journey of the _Memory App_, a productivity tool that helps users save, categorize, and revisit personal or creative memories.

> 🎯 Objective: Design the entire backend architecture from scratch using Spring Boot with a strong emphasis on planning — including requirement gathering, data modeling, and API design.

### 🎨 UI Design
- 📱 [View the Figma Prototype](https://www.figma.com/design/tT1NeXsZG9n306nEg4QpU0/Untitled?node-id=0-1&t=J2jeNuKiBIQBmsho-1)
- ✨ Designed using [**Stitch by Google**](https://stitch.withgoogle.com/)

---

## 📚 Table of Contents

- [🛠 Requirement Analysis](#-requirement-analysis)
- [📐 System Design](#-system-design)
- [🗃️ Database Design](#-database-design)
- [📈 Diagrams](#-diagrams)
- [📃 License](#-license)

---

## 🛠 Requirement Analysis

### ✅ Core Features
- User registration and login (Authentication & Authorization)
- Create, view, edit, draft, delete memories (with text, images, or video)
- Group memories into **boards**
- Drag & drop UI to rearrange memories across boards
- Calendar view for timeline-based visualization (optional)
- Daily memory reminder notifications (“On this day…”) (optional)

### 🧰 Non-Functional Requirements
- Secure media and user data handling
- Modular, scalable, and maintainable backend
- Media file upload support (Cloudinary / AWS S3)

---

## 📐 System Design

### 🔹 Overview
A layered architecture for separation of concerns:
- **Frontend** (Mobile & Web)
- **Backend API** (Spring Boot)
- **Database** (Relational)
- **Media Storage** (Cloudinary)
- **Scheduler/Notification Service** (optional)

### 🧩 Components
- Authentication Service (JWT-based)
- Memory & Media Service
- Board & Drag-n-Drop Service
- Notification Scheduler (optional)
- Calendar Module (optional)

### 📂 Design Process
- High-Level Design (HLD): System architecture, modules, technology decisions
- Low-Level Design (LLD): Class diagrams, service flow, database interaction patterns

---

## 🗃️ Database Design

- Modeled to ensure data integrity, relationship consistency, and efficient querying.
- Covers all core entities (Users, Memories, Boards, Media, Notifications, Tags)
- Focus on normalization and performance.

---

## 📈 Diagrams

| Diagram Type             | Description                                      | Status  |
|--------------------------|--------------------------------------------------|---------|
| System Architecture      | High-level overview of system components         | ✅ Added  |
| Flowchart Diagram        | Flow of user actions within the system           | ✅ Added  |
| Use Case Diagram         | Functionalities from user's perspective          | ✅ Added  |
| Entity Relationship (ER) | Database schema, tables and their relationships  | ✅ Added  |
| Class Diagram            | Class-level interaction and structure (LLD)      | ✅ Added  |
| API Flow Diagram         | Request/response and endpoint interactions       | ✅ Added  |

> 🛠 Tools Used: [draw.io](https://app.diagrams.net/), [Lucidchart](https://www.lucidchart.com/pages)

### Architecture Diagram
![Architecture Diagram](diagrams/architecture-diagram.png)

### Flowchart Diagram

#### Symbols Reference

| Symbol      | Name        | Function                                                       |
|-------------|-------------|----------------------------------------------------------------|
| 🟠 Oval          | Start/End     | An oval represents a start or end point                       |
| ➡️ Arrow         | Arrows        | A line is a connector that shows relationships between shapes |
| 🔷 Parallelogram | Input/Output  | A parallelogram represents input or output                |
| ▭ Rectangle      | Process       | A rectangle represents a process                              |
| 🔶 Diamond       | Decision      | A diamond indicates a decision                                |

#### Diagram
![Flowchart](diagrams/flowchart-diagram.png)

###  Use Case Diagram 

#### Symbols Reference

| Symbol / Shape      | Meaning                                  |
|---------------------|-------------------------------------------|
| 🧍 **Actor**         | A user or system that interacts with the system |
| 🟦 **System Boundary** | The entire application or a subsystem container |
| 🔹 **Use Case**      | A specific action or functionality in the system |
| 🔁 ``<<include>>``   | Mandatory relationship: common behavior reused by multiple use cases |
| 🧩 ``<<extend>>``    | Optional behavior that extends a base use case |
| -> **Association**   | Line connecting an actor to a use case (interaction) |

## 🖼 Use Case Diagram

- [Use Case Diagram](./diagrams/use-case-diagram.png)

###  Entity Relationship Diagram (ERD)

- [📘 Conceptual ERD](./diagrams/ERD.drawio.png)
- [📗 Logical ERD](./diagrams/erd-diagram.png)

> ✅ **Two approaches are used:**
> - The **first** diagram is a **Conceptual ERD** — focuses on entities and high-level relationships.
> - The **second** is a **Logical ERD** — includes attributes, primary/foreign keys, and relationship details.


## Class Diagram

- [Class Diagram](./diagrams/class-diagram.drawio.png)

## Api Flow Diagrams

Click to view each API flow diagram:

- [Auth Service Flow](./diagrams/auth-module.png)
- [Board Service Flow](./diagrams/board-module.png)
- [Memory Service Flow](./diagrams/memory-module.png)
- [Explore Service Flow](./diagrams/explore-module.png)
- [Calender Service Flow](./diagrams/calender-module.png)
- [Notification Service Flow](./diagrams/notification-module.png)
- [Profile Service Flow](./diagrams/profile-module.png)


## 📃 License

This project is licensed under the [MIT License](LICENSE).

---

## ✍️ Author

Built and maintained by Sana Gul — as part of a learning journey in full-stack system design and development.

