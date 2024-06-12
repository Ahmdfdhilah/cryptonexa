# ![Icon](./logo.png) 
# MariBelajar | Capstone Project 
## Kelompok Angklungis

 - Rima Artha (Mentor Capstone)
 - Ahmad Fadillah (Data Analyst and AI)
 - Muhammad Addin (Data Analyst and AI)
 - Muhammad Wahyu Ilham (Mobile & Web Developer)
 - Putri Rahayu Kusuma Ningrum (Microsoft Data Engineer)

# Automated Distributed Approval System

This project is an automated distributed approval system designed to streamline and manage various types of approvals within an organization, such as purchase approvals, budget approvals, and leave approvals. The system leverages Power Apps, Power Automate, SharePoint Lists, Python, and FastAPI to handle and check the status of approvals, providing both client and admin dashboards for efficient management.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Architecture](#architecture)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Overview

The automated distributed approval system is designed to facilitate the approval process within an organization. Workers submit requests that are first received by their division managers. Once the division manager reviews the request, it is forwarded to the HR manager for final approval or rejection.

## Features

- **Distributed Approval Flow**: Handles purchase, budget, and leave approvals.
- **Client and Admin Dashboards**: Provides intuitive interfaces for workers and managers.
- **Real-time Status Updates**: Allows users to check the status of their requests in real-time.
- **Integration with Microsoft Tools**: Utilizes Power Apps, Power Automate, and SharePoint Lists for seamless integration.
- **Backend with FastAPI**: Uses Python and FastAPI for efficient and scalable backend processing for models agent.

## Architecture

- **Power Apps**: Frontend client and admin dashboards for submitting and managing requests.
- **Power Automate**: Automates the approval workflow and forwards requests between managers.
- **SharePoint Lists**: Stores and manages approval data.
- **Python & FastAPI**: Backend services for handling models request.

## Setup and Installation

### Prerequisites

- Microsoft Power Apps
- Microsoft Power Automate
- SharePoint
- Python 3.x
- FastAPI
- Git

### Steps

1. **Clone the Repository**

   ```bash
   git clone https://github.com/Ahmdfdhilah/cryptonexa
   ```
    ```bash
   cd cryptonexa/agent-model
   ```

2. **Add Submodules**

   ```bash
   git submodule update --init --recursive
   ```

3. **Install Python Dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Set Up FastAPI Server**

   Create a `.env` file and configure your environment variables.

   ```bash
   uvicorn main:app --reload
   ```

5. **Set Up Power Apps and Power Automate**

   - Import the provided Power Apps and Power Automate flows into your Microsoft account.
   - Configure the flows to interact with your SharePoint lists and FastAPI backend.

## Usage

### Client Dashboard

- Workers submit requests via the Power Apps client dashboard.
- Requests are automatically forwarded to the division manager for review.

### Admin Dashboard

- Managers access the admin dashboard to review and approve/reject requests.
- Division managers forward requests to HR managers for final approval.

### Checking Status

- Users can check the status of their requests in real-time through the dashboards.

## Contributing

We welcome contributions to improve the system. Please fork the repository and submit pull requests.

## License

This project is licensed under the MIT License.

---

### Changelog

- **13 minutes ago**
  - Added flows to GitHub: `Microsoft.Flow/flows`
  - Added Power Apps to GitHub: `Microsoft.PowerApps/apps/7146436220200447491`
- **Now**
  - Added model repo: `agent-model @ 74f62e7`
  - Updated `.gitmodules`: Adding model repo
  - Updated `manifest.json`