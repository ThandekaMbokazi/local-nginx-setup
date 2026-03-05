# Local Web Server Setup (Nginx on Linux)

## Project Overview
This project documents the step-by-step setup of a local Nginx web server on a Linux Virtual Machine. It covers installation, service management, file system verification, and HTML customization.

---

## 1. Installation & Service Status
The Nginx server was installed and the service was managed using `systemctl`. As shown in the status output, the service is **active (running)** and **enabled** to start automatically on system boot.

**Evidence: Service Management**
<img width="916" height="699" alt="nginx" src="https://github.com/user-attachments/assets/7e166de5-73d6-4532-b24e-a89039d31dc0" />

---


## 2. Successful Default Landing Page
After navigating directly to `http://localhost`, the Nginx default landing page was successfully served. This confirms that the web server is correctly listening on Port 80.

**Evidence: Default Nginx Page**
<img width="1282" height="873" alt="nginx installed" src="https://github.com/user-attachments/assets/e49430fd-4407-4cc1-b275-f05ed7aa8074" />


---

## 3. Web Root & Folder Structure
To satisfy the folder structure requirement, the `ls -l` command was used to inspect the web root directory. This confirms the location of the server's index file.
* **Web Root:** `/var/www/html`
* **Configured File:** `index.nginx-debian.html`

**Evidence: Directory Structure**

<img width="890" height="693" alt="nginx root" src="https://github.com/user-attachments/assets/90f81a17-5280-4ac4-b84b-d277d873c6cf" />

---

## 4. HTML Customization (Command Line)
Using the `nano` text editor, the raw HTML code of the index file was modified. This demonstrates the ability to configure server content via the Linux terminal.

**Evidence: Editing via Nano**

<img width="844" height="556" alt="nginx html" src="https://github.com/user-attachments/assets/f8fabe9d-c664-4ce6-b296-921aec4ee10f" />

---

## 5. Final Customized Result
The final screenshot shows the personalized web server page. The header was successfully changed to "This is Thandeka's server!", proving the end-to-end success of the configuration.

**Evidence: Customized Server Output**
<img width="1091" height="770" alt="Thandeka Nginx" src="https://github.com/user-attachments/assets/9add4fdb-9a99-4598-a478-2904fbaa963a" />

---

## Technical Services Configured
* **Nginx (1.24.0):** High-performance HTTP server.
* **Systemd:** Used for service persistence and lifecycle management.
* **Linux File Permissions:** Managed via `sudo` to allow modification of system-level web files.

---

## Contributing
Contributions, issues, and feature requests are welcome! Feel free to fork this repository if you want to experiment with your own local server settings.

## License
This project is [MIT](https://choosealicense.com/licenses/mit/) licensed.
