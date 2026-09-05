# Peer-to-peer book lending

> **Historical archive:** This hackathon project is no longer maintained. It is
> preserved as a snapshot of the original ABV-IIITM Gwalior student project,
> not as a supported or production-ready service.

A PHP and MySQL website for students to list books, find peers willing to lend
them, request loans, and track lending/borrowing transactions and notifications.
The original workflow uses an institute email address when registering.

## Stack and repository layout

- Server-rendered PHP, HTML, CSS, and JavaScript
- MySQL/MariaDB database
- PHPMailer source bundled with the application
- `Book Your Book/` — application pages and static assets
- `Database/dbslab.sql` — schema and historical sample data for books, users,
  lenders, borrowers, transactions, and notifications

## Historical local setup

These instructions describe the environment expected by the source; they are
not a promise of compatibility with current PHP or MySQL releases.

1. Install a PHP/MySQL web stack such as XAMPP.
2. Create a database named `dbslab` and import `Database/dbslab.sql`.
3. Place the contents of `Book Your Book/` under the web server document root.
4. Review the database and mail settings in the PHP files, then open
   `index.php` through the local web server.

## Security and data warning

This is legacy educational code. It has not been security-audited and uses
outdated authentication, database-query, and mail patterns. The SQL dump
contains sample records. Do not expose it to the internet, reuse its credentials
or sample data, or use it with real personal information without a full security
review and modernization.

No license is declared; the code is retained for historical reference only.
