# photo-spotter-media-service

## Table of Contents
- [Overview](#overview)
- [Planned Features](#planned-features)
- [Environment and Dependencies](#environment-and-dependencies)
- [API Endpoints](#api-endpoints)
- [Deployment and Usage](#deployment-and-usage)
- [Tasks](#tasks)

## Overview
This service handles photo uploads, metadata extraction (EXIF), and storing images either locally or in a cloud storage. It also facilitates linking media to other services like user or location data.

## Planned Features
- Photo upload endpoint
- EXIF extraction (camera model, focal length, etc.)
- Storage adapters (local disk or S3-compatible)
- Linking media to user-service or geo-service data

## Environment and Dependencies
- C# or Go for core service logic
- Local or S3-like storage for photos
- Docker for containerization

## API Endpoints
- `/media/upload` to handle file uploads
- `/media/{id}` for retrieving media details
- `/media/{id}/exif` for EXIF metadata

## Deployment and Usage
- Run locally with `dotnet run` or `go run main.go`
- Build container via `docker build -t photo-spotter-media-service .`
- Deploy using Kubernetes manifests or a Helm chart

## Tasks
- Set up basic file upload handling
- Extract and store EXIF data
- Integrate with continuous integration
- Provide a `/health` endpoint
