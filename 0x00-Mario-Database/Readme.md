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
- To connect to PostgreSQL using the psql command-line tool, you can use the following command: `psql -U username -d database_name`. Replace username with your PostgreSQL username and database_name with the name of the database you want to connect to.
- Once connected, you can execute SQL commands directly within the psql prompt. For example, you can run queries to retrieve data, create tables, or perform other database operations.
- To exit the psql prompt, you can use the following command: `\q`

## 3. Step-3: View Databases 

When you are in the postgreSQL, you'll notice that the prompt changed to let you know that you are now interacting with PostgreSQL. First thing to do is see what databases are here. Type \l into the prompt to list them.

#### HINTS

- Type `\l` into the psql prompt and press enter

## 4. Create `first_database`


The databases you see are there by default. You can make your own like this:

```sql
CREATE DATABASE database_name;
```

The capitalized words are keywords telling PostgreSQL what to do. The name of the database is the lowercase word. Note that **all commands need a semi-colon at the end.** Create a new database named `first_database`.

#### HINTS

- Don't forget the semi-colon at the end
- Type `CREATE DATABASE first_database;` into the psql prompt and press enter


