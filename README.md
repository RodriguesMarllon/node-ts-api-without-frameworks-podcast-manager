# Podcast Manager

## 📖 About

**Podcast Manager** is an API for a Netflix-style application, aiming to centralize and organize video podcast episodes. The idea is to create a single interface where users can discover and watch their favorite podcasts, segmented by categories of interest.

## ✨ Key Features

  - **Episode Listing:** Returns a complete list of podcast episodes.
  - **Categorization:** Organizes episodes into categories such as "Health", "Bodybuilding", "Mindset", "Humor", etc.
  - **Filter by Podcast:** Allows the client to filter episodes by the podcast name.

## 🚀 Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

To run this project, you will need to have the following installed:

  - [Node.js](https://nodejs.org/) (version **v24.6.0** was used in development)
  - [npm](https://www.npmjs.com/) or [Yarn](https://yarnpkg.com/)

### Installation

1.  Clone the repository:
    ```bash
    git clone https://github.com/RodriguesMarllon/node-ts-api-without-frameworks-podcast-manager.git
    ```
2.  Navigate to the project directory:
    ```bash
    cd podcast-manager
    ```
3.  Install the dependencies:
    ```bash
    npm install
    ```
    or, if you use Yarn:
    ```bash
    yarn install
    ```

### Running the Application

To start the server, run the following command:

```bash
npm run start:dev
```

The server will be running on `http://localhost:3333` (or the port you configure in the .env file).

## API Endpoints

The API provides the following endpoints to interact with the podcast data.

### 1\. List all episodes

Returns a complete list of all registered podcast episodes.

  - **URL:** `/episodes`
  - **Method:** `GET`
  - **Success Response (200 OK):**

<!-- end list -->

```json
[
    {
        "podcastName": "flow",
        "episode": "CBUM - Flow #319",
        "videoId": "pQSuQmUfS30",
        "category": ["health", "bodybuilding"]
    },
    {
        "podcastName": "flow",
        "episode": "RUBENS BARRICHELLO - Flow #339",
        "videoId": "4KDGTdiOV4I",
        "category": ["sports", "racing"]
    },
    {
        "podcastName": "podpah",
        "episode": "NEYMAR JR - Podpah #451",
        "videoId": "exampleVideoId123",
        "category": ["sports", "soccer"]
    }
]
```

### 2\. Filter episodes by podcast name

Returns a list of episodes filtered by the podcast name, sent as a query parameter.

  - **URL:** `/episodes`
  - **Method:** `GET`
  - **Query Parameter:** `podcastName` (string)
  - **Example URL:** `/episodes?podcastName=flow`
  - **Success Response (200 OK):**

<!-- end list -->

```json
[
    {
        "podcastName": "flow",
        "episode": "CBUM - Flow #319",
        "videoId": "pQSuQmUfS30",
        "category": ["health", "bodybuilding"]
    },
    {
        "podcastName": "flow",
        "episode": "RUBENS BARRICHELLO - Flow #339",
        "videoId": "4KDGTdiOV4I",
        "category": ["sports", "racing"]
    }
]
```

## 🛠️ Technologies Used

  - [Node.js](https://nodejs.org/en/) - JavaScript runtime environment

## 🤝 How to Contribute

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## 📜 License

Distributed under the MIT License. See `LICENSE` for more information.