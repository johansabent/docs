# Mintlify Documentation Project

## Directory Overview
This directory contains the source files for a documentation website built with **Mintlify**. It holds the configuration, Markdown/MDX content files, reusable snippets, and API reference specifications required to generate and serve the documentation portal.

## Key Files
*   **`docs.json`**: The core configuration file for Mintlify. It defines the navigation structure, grouping of pages, theme settings, colors, logos, and external links (e.g., social media, support).
*   **`README.md`**: Provides essential instructions for setting up the Mintlify development environment, running the local preview server, and deploying updates.
*   **`index.mdx`, `quickstart.mdx`, `development.mdx`**: Primary guide pages making up the "Getting started" section of the documentation.
*   **`api-reference/openapi.json`**: The OpenAPI specification file. This is used by Mintlify to automatically generate structured API reference pages.
*   **`essentials/`**: A directory containing guides on how to use Mintlify's features (e.g., markdown formatting, code blocks, images, and reusable snippets).
*   **`ai-tools/`**: A directory containing documentation on how to integrate and use various AI coding tools (Claude Code, Cursor, Windsurf) with this project.
*   **`snippets/`**: Contains reusable MDX snippets that can be imported across multiple documentation pages to prevent content duplication.

## Usage
*   **Local Development:** To preview documentation changes locally, ensure you have the Mintlify CLI installed globally (`npm i -g mint`). Run the command `mint dev` in the root directory (where `docs.json` is located) and navigate to `http://localhost:3000`.
*   **Adding Content:** Write new documentation pages as `.mdx` files in the appropriate directories. To make them visible on the site, add their paths (without the `.mdx` extension) to the `navigation` array inside `docs.json`.
*   **API Reference Updates:** Update the `api-reference/openapi.json` file to automatically reflect changes in the API reference section of the documentation.
*   **Deployment:** Changes are typically deployed automatically to production after pushing to the default branch, provided the Mintlify GitHub app is installed and configured.