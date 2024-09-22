# Team Let Me Ride

## Project Goal
This project aims to use computer vision to detect people waiting in taxi ranks in Aberdeen city.
With this information, this program alerts taxi companies to send units to the locations according to the demand.

## Motivation
People waiting for a taxi in Aberdeen city centre and the airport are usually unsure whether a taxi will arrive, while waiting in long queues. Furthermore, not everyone can call the taxi companies and their mobile application are difficult to use and sometimes do not work properly.

## Progress Made
- Implemented a YOLO model to detect people standing on a video
- Save the amount of people waiting for a minimum amount of time
- Developed a web application to retrieve the data and show it in a map
- Connected the model to an IP camera

## Directory Structure
- **model/**: object tracking (YOLO) model implementation
- **templates/**: HTML templates for the application view
- **utils/**: Configuration files and helper functions

## Installation Guide

### Prerequisites
- Redis
- Python 3.10+

### 1. Set a virtual environment
```bash
python -m venv .env
```
### 2. Install the environment
```bash
pip install -r requirements.txt
```

## How to Run the Program

### 1. Start Redis server
```bash
redis-server --daemonize yes
```

### 2. Start Flask application
