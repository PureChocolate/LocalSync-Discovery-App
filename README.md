# LocalSync | MERN-Stack Discovery Platform

A full-stack application architected to bridge real-time external data with localized discovery. Built to demonstrate proficiency in REST API integration, NoSQL data structures, and asynchronous state management.

##  Technical Architecture
- **Frontend:** React.js utilizing functional components and specialized Hooks for state synchronization.
- **Backend:** Node.js/Express.js environment managing server-side logic and API routing.
- **Database:** MongoDB (NoSQL) for high-availability user and venue data persistence.
- **Data Source:** Yelp Fusion REST API integration for real-time external telemetry.

##  Key Engineering Challenges
### 1. External Data Normalization
*Challenge:* Handling varying data structures from the Yelp Fusion API and ensuring they were normalized before reaching the front-end state.  
*Solution:* Implemented a middleware logic layer in the Express server to parse and filter JSON responses, reducing client-side processing load.

### 2. Database Connectivity & Security
*Challenge:* Securing connection strings and managing database state across a distributed architecture.  
*Solution:* Implemented environment variable management and robust error-handling for MongoDB connection strings to ensure high-uptime and secure data flow.

##  Deployment & Setup
1. Clone the repository.
2. Configure your `DATABASE_URL` and `PORT` in the environment environment.
3. Execute `npm install` in both `/ravenous` and `/server` directories.
4. Launch the environment using `npm run dev`.
