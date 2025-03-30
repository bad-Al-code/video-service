# Video Service - Main Repository

This repository serves as the main entry point and coordinator for the Video Service project. It utilizes Git submodules to include the necessary microservices:

- **video-upload-service:** Handles the uploading of video files.
- **video-proccessing-service:** Handles the processing, transcoding, and preparation of uploaded videos.

This parent repository primarily tracks specific versions of the submodules and may contain top-level configuration or orchestration files (like Docker Compose, CI/CD pipelines) if needed.

## Submodules

- **video-upload-service:** [https://github.com/bad-Al-code/video-upload-service.git](https://github.com/bad-Al-code/video-upload-service.git)
  - Responsible for receiving video uploads from users.
- **video-proccessing-service:** [https://github.com/bad-Al-code/video-proccessing-service.git](https://github.com/bad-Al-code/video-proccessing-service.git)
  - Responsible for tasks like transcoding video formats, generating thumbnails, etc.

## Getting Started

### Prerequisites

- Git installed

### Cloning

To clone this repository **and** initialize the submodules correctly, use the `--recurse-submodules` flag:

```bash
git clone --recurse-submodules https://github.com/bad-Al-code/video-service.git
cd video-service
```

If you have already cloned the repository without the flag, you can initialize and update the submodules using:

```bash
# Navigate to the cloned directory if you aren't already there
cd video-service

# Initialize and fetch the submodule content
git submodule update --init --recursive
```
