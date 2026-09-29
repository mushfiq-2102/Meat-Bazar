# Meat Bazar

Online meat-delivery web app (PHP + MySQL) with three roles: **User**, **Distributor**, **Admin**.

## Project structure

```
MeatBazar/
├── index.php              Entry point (redirects to auth/login.php)
├── auth/                  login, create_account, forgot_password, logout
├── user/                  Customer pages: home, beef, mutton, chicken, cart, payment,
│                          process_order, order_success, history, profile, contact,
│                          change_user_personal_info
├── admin/                 Admin dashboard, orders, assignment, inventory,
│                          manage/add/edit/delete for admins, distributors and users
├── distributor/           Distributor dashboard, inventory, orders, profile
├── api/                   update_order_status.php (JSON endpoint used by Admin + Distributor)
├── includes/              db.php (database connection settings)
├── database/              meatbazar.sql (full schema + sample data), setup_database.php
└── assets/images/         Logo and product images