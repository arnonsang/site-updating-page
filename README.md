# Table of Contents
1. [Website Under Maintenance](#website-under-maintenance)
2. [Overview](#overview)
3. [How it Works](#how-it-works)
    - [HTML Structure](#html-structure)
    - [CSS Styling](#css-styling)
    - [JavaScript Functionality](#javascript-functionality)
4. [Usage](#usage)
    - [Running with Docker](#running-with-docker)
5. [Customization](#customization)
6. [Contributing](#contributing)
7. [License](#license)
8. [Acknowledgments](#acknowledgments)

---

# Website Under Maintenance

This repository contains the HTML page that will be displayed while our website is undergoing maintenance or updates, along with the Docker configuration to run the maintenance page using Nginx in a Docker container.

## Overview

During scheduled maintenance or updates, it's important to provide visitors with a clear indication that the website is temporarily unavailable. This HTML page serves that purpose by displaying a friendly message informing users about the maintenance process and assuring them that the website will be back online shortly.

## How it Works
The code you provided is for a website undergoing maintenance. Here's a breakdown of how it works:

### HTML Structure:

- The HTML defines the basic structure of the page.
- It includes sections for a title, message, progress bar, countdown timer, contact button, maintenance ID, and last checked time.

### CSS Styling:

- The CSS styles the appearance of the page elements.
- It controls the layout, fonts, colors, and background.

### JavaScript Functionality:

The JavaScript code adds interactivity to the page. Here are the key functionalities:

1. **Checks website state:** It periodically checks if the website is still under maintenance by fetching the current page content.
   
2. **Displays countdown timer:** It sets an initial countdown time (default 5 minutes) and updates it on the page every second.
   
3. **Redirects to updated website:**
   - If the countdown reaches zero or the website content doesn't indicate maintenance anymore, it triggers a redirect to the updated website after a short delay (default 3 seconds).
   
4. **Displays hostname and contact email:** It retrieves the current website hostname and dynamically updates the contact button link (`mailto:admin@<hostname>`) and displayed hostname.
   
5. **Generates and stores maintenance ID:** It generates a unique identifier (UUID) for this maintenance session and stores it in the browser's local storage for reference.
   
6. **Displays last checked time:** It updates the "Last checked" time with the current time whenever it checks the website state.

In summary, this webpage informs visitors that the website is under maintenance and provides an estimated time until it's back online. It also offers a contact option and displays technical details for debugging purposes.

## Usage

### Running with Docker

1. Make sure you have Docker installed on your machine. If not, you can download and install it from [Docker's official website](https://www.docker.com/get-started).

2. Clone this repository to your local machine:
    ```
    git clone <repository-url>
    ```

3. Navigate to the root directory of the cloned repository:
    ```
    cd <repository-directory>
    ```

4. Run the docker container with docker compose:
    ```
    docker compose up -d
    ```

5. Access the maintenance page in your web browser at `http://localhost/` or `https://your-domain.com/`.

## Customization

Feel free to customize the content of `maintenance.html` to suit your organization's branding and communication style. You can modify the text, add your logo, or include any other relevant information to keep visitors informed and engaged during the maintenance period.

## Contributing

If you have suggestions for improvements or would like to contribute to enhancing the maintenance page or Docker configuration, please feel free to fork this repository, make your changes, and submit a pull request. We welcome any contributions that can help make the maintenance experience smoother and more informative for our users.

## License

This project is licensed under the [MIT License](LICENSE) - see the LICENSE file for details.

## Acknowledgments

- Hat tip to [GitHub](https://github.com) for providing a platform for collaborative development and version control.
- Special thanks to all contributors who help improve this project and make it more effective in serving its purpose.
- Our gratitude to the developers of [Nginx](https://www.nginx.com) for their powerful and flexible web server software.
- Thanks to the creators of [Docker](https://www.docker.com) for simplifying the deployment and management of applications.
- This project is owned by [JLR Lab](), a technology research, consulting and development team based in Thailand. Their expertise in researching and applying technology to various applications has been invaluable.
- This project is managed by [iamickdev](https://www.iamickdev.com), a member of JLR Lab.

---

**From JLR Lab**  
*A Gen Z technology research, consulting and development team based in Thailand.*
