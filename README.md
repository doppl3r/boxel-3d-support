# Boxel 3D Support

Boxel 3D Support is an open source project for the community to submit issues or find documentation for modding.

Link: [https://doppl3r.github.io/boxel-3d-support/](https://doppl3r.github.io/boxel-3d-support/)

## Submitting a bug

Please create a New issue with the appropriate information needed to resolve a bug. Link: [https://github.com/doppl3r/boxel-3d-support/issues](https://github.com/doppl3r/boxel-3d-support/issues)

![Boxel 3D Support](docs/images/Boxel3DSupportBanner.png)

## Local Development

The documentation for this website was made using a library called MkDocs. This tool requires Python libraries to build the web documents.

### Cloning the Project

You will need to clone the project to your local machine in order to make changes.

1. Open your Terminal application
2. Set the directory to your favorite project folder. Ex: `cd C:\Users\YOURNAME\Documents\`
3. Clone the repo (requires Git installed): `git clone https://github.com/doppl3r/boxel-3d-support`

### Installing Python (Windows)

1. Download Python from the official website: https://www.python.org/downloads/
2. During the installation, be sure to check `py launcher` and `Add Python to environment variables`
3. (optional) Restart your computer if the Python commands are not working in the next steps

![Python Screenshot 1](docs/images/python-screenshot-1.png)
![Python Screenshot 2](docs/images/python-screenshot-2.png)

### Installing Dependencies

After installing Python, run the following commands to install the `pip` libraries:

1. `pip install mkdocs`
2. `pip install mkdocs-material`

## Development Workflow

When your MkDocs libraries are installed, you should be ready to serve your changes over a local IP address using the following instructions:

1. Run `mkdocs serve`
2. Copy/paste the IP address into your browser (http://127.0.0.1:8000/mysite/)

If you would like to make changes to the documentations, please use the following steps:

1. Save your local files (ex: index.md)
2. Pull the latest file changes: `git pull`
2. Stage your files: `git add -A`
3. Commit your files: `git commit -m "Update homepage text"` (Replace message with whatever you did)
4. Push your files: `git push`

## Publishing Changes

You will need to be invited as a collaborator to the github project in order to publish changes to the `gh-pages` branch. Please request an invite from `doppl3r` from our Discord server or create a new issue using the Github interface.

1. Run `mkdocs gh-deploy --force`

This will automatically deploy the changes to the `gh-pages` branch, and the documentation website will reflect the changes within a few minutes.