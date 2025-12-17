# SQL CRUD Operations - Basic Database Management

## 📚 Overview
Basic SQL database operations tutorial covering fundamental commands for managing databases in MySQL/MariaDB. This repository contains practical examples with screenshots from phpMyAdmin.

## 🎯 What You'll Learn

- **CREATE DATABASE** - How to create a new database
- **DROP DATABASE** - How to delete an existing database
- **SHOW DATABASES** - How to list all databases

## 📝 SQL Commands

### Create Database

Creates a new database in MySQL/MariaDB.

**Syntax:**
```sql
CREATE DATABASE database_name;
```

**Example:**
```sql
CREATE DATABASE db_1;
```

![Create Database](CMDCREATE.jpeg)
![Database Created](DB_Created.jpeg)

---

### Drop Database

Deletes an existing database permanently.

**Syntax:**
```sql
DROP DATABASE database_name;
```

**Example:**
```sql
DROP DATABASE db_1;
```

![Delete Database](CMDDELETE.jpeg)
![Database Deleted](DB_Deleted.jpeg)

⚠️ **Warning:** This operation permanently deletes the database and all its data!

---

### Show Databases

Displays a list of all databases on the MySQL server.

**Syntax:**
```sql
SHOW DATABASES;
```

**Example:**
```sql
SHOW DATABASES;
```

![List Databases](DB_Listed.jpeg)
![Database List](DBLIST.jpeg)

**Common databases you'll see:**
- `information_schema` - System metadata
- `mysql` - User privileges and settings
- `performance_schema` - Performance metrics
- `phpmyadmin` - phpMyAdmin configuration
- Your custom databases (like `db_1`)

---

## 🔄 Complete Example

```sql
-- Step 1: Create a new database
CREATE DATABASE db_1;

-- Step 2: Verify it was created
SHOW DATABASES;

-- Step 3: Delete the database
DROP DATABASE db_1;

-- Step 4: Confirm deletion
SHOW DATABASES;
```

## 🛠️ Tools Used

- **MySQL/MariaDB** - Database management system
- **phpMyAdmin** - Web-based database administration tool

## 📖 Quick Reference

| Command | Purpose | Example |
|---------|---------|---------|
| `CREATE DATABASE` | Create new database | `CREATE DATABASE mydb;` |
| `DROP DATABASE` | Delete database | `DROP DATABASE mydb;` |
| `SHOW DATABASES` | List all databases | `SHOW DATABASES;` |

## 💡 Best Practices

1. **Use descriptive names** - `user_management` instead of `db1`
2. **Use lowercase** - `my_database` instead of `MyDatabase`
3. **Use underscores** - `order_system` instead of `ordersystem`
4. **Backup before DROP** - Always backup important data before deleting
5. **Use IF EXISTS** - Safer: `DROP DATABASE IF EXISTS db_name;`

## ⚠️ Important Notes

- `DROP DATABASE` is **irreversible** - all data will be lost
- Always double-check the database name before dropping
- Make backups of important databases regularly
- Test commands on development databases first

## 🚀 Getting Started

1. Install MySQL/MariaDB
2. Access phpMyAdmin (usually at `http://localhost/phpmyadmin`)
3. Go to the SQL tab
4. Run the commands from this guide
5. Check the results

## 📁 Repository Contents

```
.
├── CMDCREATE       # CREATE DATABASE command screenshot
├── CMDDELETE       # DROP DATABASE command screenshot
├── DB_Created      # Database creation result
├── DB_Deleted      # Database deletion result
├── DB_Listed       # SHOW DATABASES result
├── DBLIST          # Database list view
├── read            # Command reference
└── README.md       # This file
```

## 🎓 Learning Path

**Current:** Basic Database Operations ✅
- CREATE DATABASE
- DROP DATABASE  
- SHOW DATABASES

**Next:** Table Operations (Coming Soon)
- CREATE TABLE
- ALTER TABLE
- DROP TABLE

**Future:** Data Operations
- INSERT
- SELECT
- UPDATE
- DELETE

## 📚 Resources

- [MySQL Documentation](https://dev.mysql.com/doc/)
- [MariaDB Documentation](https://mariadb.com/kb/en/)
- [phpMyAdmin Docs](https://docs.phpmyadmin.net/)
- [SQL Tutorial - W3Schools](https://www.w3schools.com/sql/)

## 🤝 Contributing

Feel free to contribute by:
- Adding more examples
- Improving documentation
- Reporting issues
- Suggesting improvements

## 📄 License

Educational purposes

---

**Happy Learning! 🎉**
