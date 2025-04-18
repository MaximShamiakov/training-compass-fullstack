# training-compass-fullstack

## Description

This project combines a Django backend and React frontend into a fullstack application, managed via Docker Compose for easy development and deployment.
The structure preserves the Git history of both projects using Git Submodules.

## Tech Stack

- Frontend: React (created with create-react-app)
- Backend: Django REST Framework
- Containerization: Docker + Docker Compose
- Version Control: Git Submodules

## Clone the Repository

git clone --recursive git@github.com:MaximShamiakov/training-compass-fullstack.git

## Start the Application

docker-compose up --build

## (Optional) Run Services Individually

## Start only the frontend

cd frontend && npm start

## Start only the backend

cd backend && python manage.py runserver

## If the original repositories (frontend/backend) receive update

git submodule update --remote

## Rebuilding Docker Containers after making changes to either project

docker-compose up --build

## This project uses Git Submodules to track the frontend and backend repositories separately.

- Frontend Submodule: react-training-compass
- Backend Submodule: django-training-compass

## To view the commit history of each submodule

cd frontend && git log   # Frontend history

cd ../backend && git log # Backend history



