# TrackNBack

**Discover Lost, Reunite Found.**
TrackNBack is a campus lost-and-found web application. Students post items they have lost, others mark them as found, and admins moderate every post before it goes public.

## Features

**Users**
- Register and log in with a university email and student ID
- Post a lost item with category, description and photo
- Browse the community feed of approved lost items
- Mark an item as found and notify the owner with the finder's name and mobile number
- View notifications
- Edit profile and settings, including profile photo

**Admins**
- Separate admin login and dashboard
- Approve or decline pending posts
- Delete posts
- View stats: total lost items, items marked found, total users
- Manage users and remove members
- Add and manage item categories (Pen, Notepad, Bottle, Money, etc.)
- Edit the welcome and about pages

## Tech Stack
- PHP 8.2
- MySQL / MariaDB
- Tailwind CSS
- XAMPP (Apache + MySQL) for local development



## Getting Started

1. Install [XAMPP](https://www.apachefriends.org/) and start Apache and MySQL.
2. Copy the project folder into `xampp/htdocs/`.
3. Open phpMyAdmin, create a database named `tracknback`, and import `SQL/tracknback.sql`.
4. Check `config.php` matches your setup (defaults: host `localhost`, user `root`, empty password, database `tracknback`).
5. Visit `http://localhost/TRACKNBACK/landing.php`.

## Database Tables
| Table | Purpose |
|---|---|
| `users` | Registered students |
| `admintab` | Admin accounts |
| `lostposts` | Lost-item posts with approval and found status |
| `category` | Item categories |
| `notifications` | Found-item alerts sent to owners |
| `aboutus` | About page content |

## How It Works
1. A user registers and posts a lost item.
2. The post goes to the admin as **Pending**.
3. After admin approval, it appears in the community feed.
4. Someone who finds the item clicks **Found**, and the owner gets a notification with the finder's contact.
5. The post is marked **FOUND!**.


## Participants : 
- Tairin Islam
- Mohammad Darain Khan

