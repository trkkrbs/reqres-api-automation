# API Test Automation with Postman, Newman & GitHub Actions

## Project Overview

This project shows API test automation using Postman.  
Tests are executed with Newman.  
GitHub Actions runs the tests automatically on a schedule.

---

## The project uses the ReqRes API and covers a full user flow: 

- Login (extract token)
- Create User (extract ID)
- Get User List
- Get Single User
- Update User
- Delete User

---

## Technologies

- Postman
- Newman
- Newman HTML Extra Reporter
- GitHub Actions
- Cron schedule

---

## Local Run

-- Runs the collection
-- Executes all tests
-- Generates an HTML report
-- Saves the report in the reports folder

---

## CI/CD (GitHub Actions)

-- Installs Node.js
-- Installs Newman
-- Runs the collection
-- Generates an HTML report
-- Uploads the report as an artifact

---

### Workflow Schedule

-- Runs every Monday
-- Can run manually (Run workflow button)

---

### Reports

-- Reports are generated automatically
-- Download from:
   -- Actions
   -- Select workflow run
   -- Open Artifacts
   -- Download newman-report

---

### Purpose

-- Practice API automation
-- Show CI/CD integration
-- Run tests on schedule
-- Generate HTML reports
   

   

