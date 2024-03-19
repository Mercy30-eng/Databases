# Building a Mario Database

>I will be creating a PostgreSQL database filled with video game characters on linux by following the steps below:

## 1. Step-1: Start the Terminal

**The first thing you need to do is start the terminal/CLI.** 

## 2. Step-2: Install PostgreSQL

###Instructions

- Open a terminal window and run the following command to add the PostgreSQL repository:
`sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt $(lsb_release -cs)-pgdg main" > /etc/apt/sources.list.d/pgdg.list'`.
- Next, add the PostgreSQL GPG key to your package manager by running the following command:
`wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -`
- Update and Install PostgreSQL: `sudo apt-get update`
- Finally, install PostgreSQL and the additional contrib package by running: `sudo apt-get install postgresql postgresql-contrib`
- To verify that PostgreSQL is installed, you can check the version using the command: `psql --version`
- After installation, set a password for the default postgres user by running the following command: `sudo -u postgres psql`
- Once installed, you can access PostgreSQL by using the psql command in the terminal. `psql`

## 2. Step-3: 
