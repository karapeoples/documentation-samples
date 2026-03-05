##School'R — Setup & Run Guide

## Overview
School'R is a React app that uses a mock API for CRUD workflows during local development.

## Prerequisites
- Node.js (LTS recommended)
- npm or yarn

## Install
1. Clone the repo
2. Install dependencies:
   - `npm install` or `yarn`

## Start the mock API (json-server)
Run one of the following:
- `npm run mock:api`
- `yarn mock:api`

This starts the mock API used for CRUD operations via the `db.json` file.

## Run the app
In a separate terminal:
- `npm start` or `yarn start`

## Notes
- If the UI loads but data is missing, confirm the mock API is running.
- If ports conflict, update the script in `package.json` or stop the existing service.
