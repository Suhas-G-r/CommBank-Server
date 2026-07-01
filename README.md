# CommBank-Server — Commonwealth Bank Software Engineering Job Simulation

[![.NET](https://img.shields.io/badge/.NET-C%23-purple.svg)](https://dotnet.microsoft.com/)
[![MongoDB](https://img.shields.io/badge/Database-MongoDB%20Atlas-green.svg)](https://www.mongodb.com/atlas)
[![Forage](https://img.shields.io/badge/Forage-Commonwealth%20Bank-yellow.svg)](https://www.theforage.com/simulations/commonwealth-bank/software-engineering-c4hw)

This repository contains my completed work for the **Commonwealth Bank Software Engineering Virtual Job Simulation** hosted on [Forage](https://www.theforage.com/simulations/commonwealth-bank/software-engineering-c4hw). The simulation replicates real backend engineering work performed by Commonwealth Bank's software engineering team, extending an existing .NET/C# server (`rSERVER`) that powers a customer savings-goals feature.

---

## What This Simulation Covered

* **Backend Setup:** Forked and configured the `rSERVER` starter repository (a .NET/C# API).
* **Database Provisioning:** Created and connected a live **MongoDB Atlas** cluster and database user, then wired the server to it via connection string configuration.
* **Database Seeding & API Testing:** Seeded the `Goals` collection with sample data and manually verified API endpoints (GET/POST) using tools like Postman, first without icons, then with icons enabled.
* **Data Model Extension:** Modified the `Goal` model in C# to add an optional `Icon` field, extending the schema to support richer client-side savings-goal displays.
* **Version Control:** Used Git throughout to track incremental changes and prepare the work for review, mirroring how the real engineering team manages pull requests.

---

## Tech Stack

* **C# / .NET** — backend API framework
* **MongoDB Atlas** — cloud-hosted NoSQL database
* **xUnit** — unit testing for controller/model changes
* **Git** — version control

---

## Key Challenges & What I Learned

* **Target Framework Mismatches:** Resolved .NET SDK/target framework version conflicts between the starter project and my local environment to get the solution building cleanly.
* **MongoDB Tooling on Windows:** Worked around a PATH environment variable lag after installing MongoDB tools by invoking `mongoimport` via its full executable path to seed the database successfully.
* **Schema Evolution:** Got hands-on practice extending a live data model (`Goal`) in a way that stays backward-compatible with existing API consumers — a common real-world backend engineering concern.

---

## Running This Project

1. Clone the repository:
```bash
   git clone https://github.com/Suhas-G-r/CommBank-Server.git
   cd CommBank-Server
```
2. Open `Server.sln` in Visual Studio (or your preferred .NET IDE).
3. Set up a MongoDB Atlas cluster and update the connection string in the server configuration.
4. Restore dependencies and build the solution.
5. Run the server and test the API endpoints (e.g., via Postman or `curl`).

---

## About This Program

The Commonwealth Bank Software Engineering Job Simulation is a self-paced, 5–6 hour program on Forage that mirrors real day-to-day engineering tasks at Commonwealth Bank — extending backend services, working with live databases, and validating changes through testing. Learn more at [theforage.com](https://www.theforage.com/simulations/commonwealth-bank/software-engineering-c4hw).

---

*Completed by **Suhas G R** as part of the Forage Commonwealth Bank Software Engineering Virtual Job Simulation.*