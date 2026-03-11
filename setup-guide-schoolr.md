# School'R — Setup & Run Guide

## Overview

School'R is a React application that uses a mock API workflow for CRUD operations during local development.

This documentation sample focuses on helping a developer clone, install, and run the project successfully in a local environment.

## Prerequisites

- Node.js (LTS recommended)
- npm or yarn

## Installation

1. Clone the repository.
2. Install dependencies:

```bash
npm install
```
or
```
yarn
```

## Start the Mock API

Run one of the following commands:
```
npm run mock:api
```
or
```
yarn mock:api
```
This starts the mock API used to support CRUD workflows through the local data source.

## Start the Application

In a separate terminal, run:
```
npm start
```
or
```
yarn start
```

## Troubleshooting Notes

If the UI loads but project data is missing, confirm the mock API is running.

If a port conflict occurs, update the script in package.json or stop the conflicting process.

If CRUD changes do not appear, verify that the local mock API process started successfully.

## Documentation Goal

This sample demonstrates clear setup guidance for a collaborative React project using a mock API workflow, with emphasis on:

-prerequisite clarity
-step-by-step setup
-command visibility
-common troubleshooting points
