<<<<<<< HEAD
# Demo745
=======
# WCM-Dashboard

## Overview

WCM-Dashboard is a web application designed to manage various aspects of the WCM Mortgage Employee Dashboard. It includes functionalities for employee management, room bookings, request closings, PDA forms, ticket management, and Dropbox file handling.

## Figma Design
[Figma Design Link](https://www.figma.com/design/80cnr7S2W8aHI9GmksASIr/WCM-Website?node-id=1-3534&p=f)

## Prerequisites

- Python 3.x
- Docker

## Setup Instructions

### Step 1: Install Docker

To run MongoDB on your local Linux machine, execute the following commands:

```sh
sudo apt update
sudo apt install -y docker.io
sudo systemctl start docker
sudo systemctl enable docker
sudo docker run -d -p 27017:27017 --name mongodb mongo:latest
```

### Step 2: Create Python Environment

After creating a MongoDB server on your local machine, run the following command to create a Python environment:

```sh
python3 -m venv "backend-env"
```

### Step 3: Activate the Virtual Environment

To activate the virtual environment, run:

```sh
source ./backend-env/bin/activate
```

### Step 4: Install Dependencies

Install the required dependencies:

```sh
pip3 install -r requirements.txt
```

### Step 5: Run the Server

To run the server on your local machine, execute:

```sh
cd  WCM Mortgage Employee Dashboard

python3 -m applications.app
```

### Step 6: Deactivate the Virtual Environment

To deactivate the Python virtual environment, run:

```sh
deactivate
```

## Project Structure

```
WCM-Dashboard/
├── applications/
│   ├── __init__.py
│   ├── app.py
│   ├── config.py
│   ├── database.py
│   ├── utils.py
│   ├── routes/
│   │   ├── __init__.py
│   │   ├── main_routes.py
│   │   ├── admin_routes.py
│   │   ├── login_routes.py
│   │   ├── upload_routes.py
│   │   ├── scheduling_routes.py
│   │   ├── onboarding_routes.py
│   │   ├── ticket_routes.py
│   │   ├── pda_routes.py
│   │   ├── contract_routes.py
│   ├── templates/
│   │   ├── login.html
│   │   ├── home.html
│   │   ├── admin/
│   │   │   ├── dashboard.html
│   │   │   ├── pda.html
│   │   │   ├── tickets.html
│   │   │   ├── closing_requests.html
│   │   │   ├── onboarding.html
│   └── static/
│       ├── css/
│       │   ├── styles.css
│       └── js/
│           ├── scripts.js
├── requirements.txt
├── README.md
└── ...
```

## Key Features

* Employee Management: Manage employee data and credentials.
* Room Bookings: Handle room booking requests.
* Request Closings: Manage closing requests.
* PDA Forms: Handle PDA form submissions.
* Ticket Management: Manage support tickets.
* Dropbox File Handling: Manage files stored in Dropbox.

>>>>>>> master
