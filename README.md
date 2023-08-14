Dockerized Web Server with WordPress, MySQL, and PhpMyAdmin for **Windows**. 

This GitHub project provides a convenient way to set up a local development environment for a web server using Docker. The environment includes containers for WordPress, MySQL, and PhpMyAdmin, allowing you to easily develop, test, and manage your web applications.

Features:
- **Docker Compose Configuration:** The project includes a well-structured Docker Compose YAML file that defines the services required for the web server setup.

- **WordPress Container:** The WordPress container runs the popular WordPress content management system. You can develop and test your WordPress-based websites in an isolated environment.

- **MySQL Container:** The MySQL container provides the necessary database backend for your WordPress installation. It ensures data persistence and allows you to manage your site's data without affecting other components.

- **PhpMyAdmin Container:** The PhpMyAdmin container offers a graphical user interface to interact with the MySQL database. This enables you to manage and manipulate your database easily.

- **Scalability and Isolation:** Each component is containerized, offering scalability and isolation. You can focus on developing your application without worrying about conflicts between dependencies.

How to Run the Project:
1. **Prerequisites:** Make sure you have Docker and Docker Compose installed on your system.

2. **Clone the Repository:** Clone this GitHub repository to your local machine.

   ```bash
   git clone https://github.com/Anchenni/docker-web-server-wordpress.git
   ```

3. **Navigate to the Project Directory:** Move into the project directory.

   ```bash
   cd docker-web-server-wordpress
   ```

4. **Edit Configuration (Optional):** Open the `docker-compose.yml` file and modify any environment variables, passwords, or settings according to your preferences.

5. **Start the Containers:** Run the following command to start the containers.

   ```bash
   docker-compose up -d
   ```

   The `-d` flag runs the containers in the background.

6. **Access WordPress:** Open your web browser and navigate to `http://localhost:8080` to access your WordPress site. Follow the WordPress installation instructions.

7. **Access PhpMyAdmin:** To manage your database, go to `http://localhost:8081`. Log in with the MySQL username and password specified in the `docker-compose.yml` file.

8. **Stop and Clean Up:** When you're done working, you can stop and remove the containers.

   ```bash
   docker-compose down
   ```

   This will stop and remove the containers, but your data will persist if you haven't modified the volume configurations.

With this project, you can easily set up a local development environment for web applications that require WordPress, MySQL, and a database management interface. It provides a streamlined and reproducible way to work on web projects without the hassle of manual installation and configuration.
