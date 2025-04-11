# RedditClone
A minimalist Reddit clone built with .NET 9, Razor Pages, and a Web API.

## Table of Contents
-   [Project Description](#project-description)
-   [Features](#features)
-   [Getting Started](#getting-started)
    -   [Prerequisites](#prerequisites)
    -   [Installation](#installation)
    -   [Running the Application](#running-the-application)
-   [Folder Structure](#folder-structure)
-   [Technologies Used](#technologies-used)
-   [Contributing](#contributing)
-   [License](#license)
-   [Contact](#contact)

## Project Description
This project is a simplified Reddit clone designed to demonstrate best practices in .NET 9 development, including Clean Architecture, API-first design, and modular UI development using Razor Pages. It prioritizes a clean, intuitive user experience with a minimalist design.

## Features v0.0.1
-   **User Authentication and Authorization:**
    - [ ]  Registration and login.
    - [ ]  Role-based access control.
    - [ ]  Secure password management.
-   **Community Management (Subreddits):**
    - [ ]  Create and manage communities.
    - [ ]  Subscribe/unsubscribe to communities.
    - [ ]  Display community lists.
-   **Post Creation and Display:**
    - [ ]  Create text and link posts.
    - [ ]  Sort posts (hot, new, top).
    - [ ]  Community association.
-   **Commenting System:**
    - [ ]  Add and reply to comments.
    - [ ]  Edit and delete comments.
    - [ ]  Hierarchical comment display.
-   **Voting System:**
    - [ ]  Upvote and downvote posts and comments.
    - [ ]  Display scores.
-   **Search Functionality:**
    - [ ]  Search for posts and communities.
-   **User Profiles:**
    - [ ]  Display user posts and comments.
    - [ ]  Display joined communities.

## Getting Started
### Prerequisites
-   [.NET 9 SDK](https://dotnet.microsoft.com/download/dotnet/9.0)
-   [Entity Framework Core Tools](https://docs.microsoft.com/en-us/ef/core/cli/)
-   A database system (e.g., PostgreSQL, SQL Server).
-   A code editor (e.g., Visual Studio, VS Code).

### Installation
1.  Clone the repository:
    ```bash
    git clone https://github.com/Riguidix/reddit-clone.git
    cd RedditClone
    ```
2.  Navigate to the API project and update the database connection string in `RedditClone.Api/appsettings.json`.
3.  Apply database migrations:
    ```bash
    cd RedditClone.Api
    dotnet ef database update
    ```
4.  Navigate to the Web project and update the API base URL in `RedditClone.Web/appsettings.json`.
5.  Install necessary front end libraries.
    ```bash
    cd RedditClone.Web/wwwroot/lib
    ```

### Running the Application
1.  Run the API project:
    ```bash
    cd RedditClone.Api
    dotnet run
    ```
2.  Run the Web project in a new terminal:
    ```bash
    cd RedditClone.Web
    dotnet run
    ```
3.  Open your browser and navigate to `http://localhost:5000` (or the port specified in your `appsettings.json`).

## Folder Structure
```
RedditClone/
├── RedditClone.Api/
│   ├── Controllers/
│   ├── Data/
│   ├── Models/
│   ├── appsettings.json
│   ├── RedditClone.Api.csproj
│   └── Program.cs
├── RedditClone.Web/
│   ├── Pages/
│   ├── wwwroot/
│   ├── appsettings.json
│   ├── RedditClone.Web.csproj
│   └── Program.cs
├── RedditClone.sln
└── README.md
```

## Technologies Used

-   .NET 9
-   Razor Pages
-   ASP.NET Core Web API
-   Entity Framework Core
-   ASP.NET Core Identity
-   JWT Authentication

## Contributing
Contributions are welcome! Please feel free to submit pull requests or open issues to suggest improvements.

1.  Fork the repository.
2.  Create a new branch (`git checkout -b feature/your-feature`).
3.  Make your changes.
4.  Commit your changes (`git commit -am 'Add some feature'`).
5.  Push to the branch (`git push origin feature/your-feature`).
6.  Open a pull request.

## License
[MIT](LICENSE)

## Contact
[Riguidix](https://github.com/Riguidix/)
