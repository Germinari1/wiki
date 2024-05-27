# Wiki 

This project is a web application that simulates a simplified version of Wikipedia. It allows users to browse, search, create, edit, and view encyclopedia entries stored in Markdown format. The application is built using the Django web framework and Python.

## Features

- **Entry Page**: Users can visit the page for a specific encyclopedia entry by navigating to `/wiki/TITLE`, where `TITLE` is the title of the entry. If the entry exists, its content (converted from Markdown to HTML) will be displayed. If the entry does not exist, an error page will be shown.

- **Index Page**: The index page (`/wiki/`) lists all available encyclopedia entries. Users can click on any entry name to be taken directly to that entry's page.

- **Search**: Users can search for encyclopedia entries by typing a query into the search box in the sidebar. If the query matches an entry's title, the user will be redirected to that entry's page. If the query does not match any titles, the search results page will display a list of all entries that contain the query as a substring in their titles or content. Clicking on any entry name in the search results will navigate to that entry's page.

- **New Page**: Users can create a new encyclopedia entry by clicking the "Create New Page" link in the sidebar. They can enter a title for the new entry and provide the content in Markdown format. If an entry with the same title already exists, an error message will be displayed. Otherwise, the new entry will be saved, and the user will be redirected to the new entry's page.

- **Edit Page**: On each entry's page, users can click a link to edit the entry's content. The existing Markdown content will be pre-populated in a textarea. Users can modify the content and save their changes, after which they will be redirected back to the entry's page with the updated content.

- **Random Page**: Clicking the "Random Page" link in the sidebar will take the user to a randomly selected encyclopedia entry.

- **Markdown to HTML Conversion**: The Markdown content of each entry is converted to HTML before being displayed to the user. This conversion is performed using the `python-markdown2` package.

## Installation and Setup

1. Clone the repository or download the source code.
2. Install the required dependencies by running `pip install -r requirements.txt`.
3. Navigate to the project directory and run `python manage.py runserver` to start the development server.
4. Open your web browser and visit `http://localhost:8000/wiki/` to access the Wiki Encyclopedia.

## Contributing

Contributions to this project are welcome. If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.
