# Headless WordPress Theme

This is a headless WordPress theme designed to be used in conjunction with a front-end framework like React, Vue, or Angular. The theme serves as a minimal WordPress backend, providing content via the WordPress REST API to be consumed by your front-end application.

## Installation

### Prerequisites

- A WordPress installation (version 5.0 or higher)
- Basic knowledge of WordPress themes
- A front-end application ready to consume data from the WordPress REST API

### Steps to Install the Theme

1.  **Download the Theme:**

    - Clone or download the theme from the repository:
      ```bash
      git clone https://github.com/CareProID/headless-wordpress-theme.git
      ```
    - Alternatively, download the theme as a `.zip` file and extract it to your local machine.

2.  **Upload the Theme:**

    - Log in to your WordPress admin panel.
    - Navigate to `Appearance > Themes`.
    - Click on `Add New` and then `Upload Theme`.
    - Select the `.zip` file if you downloaded it, or upload the theme folder if you cloned the repository.

3.  **Activate the Theme:**

    - Once the theme is uploaded, click on `Activate` to make it your active WordPress theme.

4.  **Configure Permalinks:**

    - Navigate to `Settings > Permalinks`.
    - Ensure you have a custom structure or post name option selected to make sure the REST API endpoints are correctly formatted.

5.  **Setup API**

    a. **REST API:** Ensure that the WordPress REST API is enabled. It is enabled by default in WordPress 4.7 and later.

    b. **GraphQL:** You can use [WPGraphQL](https://github.com/wp-graphql/wp-graphql)

6.  **Connect to Your Front-End Application:**

    a. **WordPress REST API:**

    - Point your front-end application to your WordPress site's REST API endpoint, typically located at:

    ```
    https://yourdomain.com/wp-json/wp/v2/
    ```

    - Start consuming content via the REST API.

    b. **WordPress GraphQL API:**

    - Point your front-end application to your WordPress site's GraphQL API endpoint, typically located at:

    ```
    https://yourdomain.com/graphql
    ```

    - And either you can customize your own endpoint by set in wordpress admin dashboard : `GraphQL on Sidebar > Settings > WPGraphQL General Settings > GraphQL Endpoint`

    - Start consuming content via the GraphQL API.

## License

This project is licensed under the MIT License. You are free to use, modify, and distribute this theme as per the terms of the license.

For more information, see the [LICENSE](./LICENSE) file.
