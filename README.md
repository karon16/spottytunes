Here’s the updated README file with information about the three APIs (Last.fm API, Spotify Web API, and MockAPI) used in your project:

SpottyTunes: A Music Streaming Web Application

Project Overview

SpottyTunes is a modern music streaming web application that allows users to discover new music releases, search for tracks, and create personalized playlists. The app integrates data from multiple APIs to provide a seamless user experience.
	•	Last.fm API is used to fetch track details and music data.
	•	Spotify Web API is used for fetching album art and additional metadata.
	•	MockAPI is used to manage user-specific data such as playlists and favorite tracks, with CRUD functionality.

Features
	•	Home Page: Displays the latest music releases fetched from the Spotify Web API.
	•	Search Page: Enables users to search for music tracks, with track details fetched from the Last.fm API and album art provided by the Spotify Web API.
	•	Playlist Page: Allows users to save, view, edit, and delete their favorite tracks using MockAPI.
	•	Seamless Integration: Combines data from Last.fm and Spotify APIs with user-specific data stored in MockAPI.

Technologies Used
	•	Frontend Framework: React
	•	APIs:
	•	Last.fm API: For fetching music data such as track titles, artists, and metadata.
	•	Spotify Web API: For fetching album art and other visual data.
	•	MockAPI: For managing user-specific data (e.g., playlists and favorite tracks) with full CRUD operations.
	•	Linting & Formatting: ESLint and Prettier

Installation and Setup

Prerequisites
	•	Node.js (>=16.x.x)
	•	npm (>=8.x.x)
	•	Spotify Developer Account (for API keys)
	•	Last.fm Developer Account (for API keys)
	•	MockAPI account (for managing mock datasets)

Steps
	1.	Clone the repository:

git clone https://github.com/your-repository-name.git
cd your-repository-name


	2.	Install dependencies:

npm install


	3.	Create a .env file in the root directory and add your API credentials:

REACT_APP_SPOTIFY_CLIENT_ID=your_spotify_client_id
REACT_APP_SPOTIFY_CLIENT_SECRET=your_spotify_client_secret
REACT_APP_SPOTIFY_REDIRECT_URI=http://localhost:3000
REACT_APP_LASTFM_API_KEY=your_lastfm_api_key


	4.	Start the development server:

npm start


	5.	Access the application at http://localhost:3000.

Setting Up ESLint and Prettier

Install Dependencies

To set up ESLint and Prettier in the project, run the following commands:

npm install --save-dev eslint prettier eslint-plugin-react eslint-config-prettier eslint-plugin-prettier

Configure ESLint
	1.	Create an .eslintrc.json file in the root directory:

{
  "env": {
    "browser": true,
    "es2021": true
  },
  "extends": [
    "eslint:recommended",
    "plugin:react/recommended",
    "plugin:prettier/recommended"
  ],
  "parserOptions": {
    "ecmaFeatures": {
      "jsx": true
    },
    "ecmaVersion": 12,
    "sourceType": "module"
  },
  "plugins": ["react", "prettier"],
  "rules": {
    "prettier/prettier": "error",
    "react/react-in-jsx-scope": "off"
  }
}


	2.	Add a lint script to your package.json:

"scripts": {
  "lint": "eslint ."
}



Configure Prettier
	1.	Create a .prettierrc file in the root directory:

{
  "semi": true,
  "singleQuote": true,
  "printWidth": 80
}


	2.	Add a format script to your package.json:

"scripts": {
  "format": "prettier --write ."
}

Running ESLint and Prettier
	•	To check for linting errors:

npm run lint


	•	To auto-format the code:

npm run format

Contributing
	1.	Fork the repository.
	2.	Create a new feature branch (git checkout -b feature/YourFeature).
	3.	Commit your changes (git commit -m 'Add YourFeature').
	4.	Push to the branch (git push origin feature/YourFeature).
	5.	Open a pull request.

License

This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgements
	•	Last.fm API
	•	Spotify Web API
	•	MockAPI
	•	ESLint and Prettier Guide

This updated README reflects the use of the Last.fm API for music data, Spotify API for images, and MockAPI for managing user data. Let me know if you need further edits!