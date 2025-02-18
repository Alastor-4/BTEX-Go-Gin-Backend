# BTEX - Backend for Audio and Video to Text Conversion

**BTEX** is a backend service developed in Go that converts audio and video files to text using **Faster Whisper**. The service exposes a RESTful API with **Gin Gonic** and supports **JWT** authentication. Additionally, **Redis** is used to handle rate limiting and optimize the number of requests per user.

## Features

- **Audio and video to text conversion**: Uses Faster Whisper to process the files.
- **JWT Authentication**: Secures endpoints with JWT-based authentication.
- **Rate limiting with Redis**: Limits the number of requests a user can make to prevent system overload.
- **RESTful API**: Exposes endpoints to interact with the service.

## Requirements

- **Go** (1.24 or higher)
- **Redis** (for rate limiting)
- **Faster Whisper** (for audio/video conversion)
- **JWT** for authentication

## Installation

### Step 1: Clone the repository

```bash
git clone https://github.com/alastor-4/BTEX-Go-Gin-Backend
cd BTEX-Go-Gin-Backend
go mod tidy
