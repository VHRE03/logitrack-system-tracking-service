# LogiTrack: Tracking Service

## Overview
This repository contains the Tracking Service, an asynchronous application that listens to dispatch events via a message broker to record fleet coordinates.

## Technical Stack
* Framework: Spring Boot
* Messaging: Spring for RabbitMQ / Kafka
* Default Port: 8083

## Core Entities
* **DispatchEvent**: In-memory DTO for deserializing broker messages.
* **TrackingCoordinate**: Records the spatial location history (latitude, longitude, speed) linked to specific routes and vehicles in the database.
