# CoralBarrier.LK: Coral Reef Conservation Platform

A community and awareness web platform about coral reef conservation in Sri Lanka. Users learn about coral reefs, read news, join community discussions and explore reef predictions. Administrators manage content and users from a dashboard.

## Features

### Users
- Register, log in and manage a profile, including a profile picture
- **Community**: create posts and comment on other users' posts
- **News**: read the latest coral reef news
- **Map**: explore reef locations
- **Prediction**: select a year and month to view a coral reef prediction
- Educational pages about why coral reefs matter

### Administrators
- Separate admin login and registration
- Dashboard with user and content tables
- Add and delete news articles
- Moderate users and community posts

## Tech stack

PHP · MySQL · HTML5 · CSS3 · JavaScript · Bootstrap

## Database

The schema is in [`coralbarrer.sql`](coralbarrer.sql) and has these tables:

| Table | Purpose |
|-------|---------|
| `users` | Registered users |
| `admins` | Administrator accounts |
| `post` | Community posts |
| `comment` | Comments on posts |
| `news` | News articles |

## Getting started

**Prerequisites:** PHP 7.4+, MySQL, and a local server such as XAMPP, WAMP or LAMP.

1. Clone the repository into your web root (for example `htdocs/`):

   ```bash
   git clone https://github.com/SamithaPrabath/Coral-reef--frontend.git
   ```

2. Create a database and import the schema:

   ```bash
   mysql -u root -p -e "CREATE DATABASE coralbarrer"
   mysql -u root -p coralbarrer < coralbarrer.sql
   ```

3. Update the database host, port and credentials in `database_connect.php`. It defaults to `localhost:3308`, user `root`.
4. Open `http://localhost/Coral-reef--frontend/`.

## Contributors

- **Samitha Prabath**: [GitHub](https://github.com/SamithaPrabath)
- **Isuru**
- **Thathsara Pramuditha**
