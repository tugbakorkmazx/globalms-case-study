# GlobalMS — Stock Management System

A full-stack inventory and stock management system built end-to-end for
Global Sınıf Science Center, deployed to production and used daily across
multiple branches.

> **Note:** This repository documents the project (screenshots & architecture).
> The source code is private as this is a client system.

## Live
🔗 stok.globalsinif.com

## Tech Stack
- **Backend:** ASP.NET Core MVC, C#, Entity Framework Core
- **Frontend:** Razor, JavaScript, Bootstrap, jQuery
- **Database:** MySQL
- **Infrastructure:** Linux server, cron-based automated backups (mysqldump + rclone → Google Drive)

## Key Features
- Role-based access control (Superadmin / Admin / Manager / User)
- Stock tracking with real-time client-side calculations
- BOM (Bill of Materials) & consumables management
- Printable reports and bulk data imports
- Branch/office-based stock views on an interactive map (Google Geocoding API)
- CSRF protection across all controllers

## Engineering Highlights
- Designed and built the full system from database schema to deployment
- Administered the production Linux server (resolved MySQL out-of-memory
  issues via swap configuration, fixed server timezone)
- Built an automated nightly MySQL backup pipeline with 30-day cloud retention

## Screenshots

### Dashboard
![Dashboard](anasayfa.png)

### User Management
![User Management](kullanici-yonetimi.png)

### Stock Overview
![Stock Overview](stok-durumu.png)

### Branch Map
![Map](harita.png)
