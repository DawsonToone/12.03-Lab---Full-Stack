# CS208 Full Stack Final Project

- Name: Dawson Toone
- GitHub: [https://github.com/DawsonToone](https://github.com/DawsonToone)
- Term: Fall 2026

## Project Description

This is my full-stack application for CS208, built with node.js. I built a web
application that allows you to add tasks to a todo list, while also being able to
edit them, delete them, or mark them as complete. The application uses Express for
the backend and MariaDB (MySQL) for the database. Please read the following
instructions carefully because some of the setup only needs to be done once.

## Install the Database

To set up the database, run the `install_db.sh` script in the setup_scripts
directory. This script will install MariaDB and start the server running. You
only need to run this script once per Codespace.

```bash
./setup_scripts/install_db.sh
```

If the terminal asks you questions, refer to this guide:

- Switch to unix_socket authentication [Y/n] n
- Change the root password? [Y/n] Y
  - Set the password to 12345
- Remove anonymous users? [Y/n] Y
- Disallow root login remotely? [Y/n] Y
- Remove test database and access to it? [Y/n] Y
- Reload privilege tables now? [Y/n] Y

## Create the Database Tables

Create the initial tables by running the following command:

```bash
sudo mysql -u root -p < ./setup_scripts/create_demo_table.sql
```

## Install Dependencies

Install the required dependencies using npm:

```bash
npm install
```

## Run the Application

Start the application using the following command:

```bash
npm start
```

## Access the Application

On Codespaces, you can access the application by forwarding port 3000. Open the
forwarded port in your browser to view the application.