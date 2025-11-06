![Logo](./docs/images/kyberVisionLogo01.png)

# API v0.22.0

## Overview

### Conversion to TypeScript

This is a TypeScript Express.js API project. This project is based on the KyberVision20API.

- see the docs/TS_CONVERSION_STATUS.md for detailed step by step conversion process with Claude Code.

## .env

```bash
APP_NAME=KyberVision22API
JWT_SECRET=secret_code
PATH_DATABASE=Users/nickrodriguez/Documents/KyberVision22API/databases/KyberVision22API/
NAME_DB=kv22.db
PATH_VIDEOS=/Users/nickrodriguez/Documents/_project_resources/KyberVision22API/session_videos
PATH_VIDEOS_UPLOADED=/Users/nickrodriguez/Documents/_project_resources/KyberVision22API/session_videos/uploaded
PATH_VIDEOS_MONTAGE_CLIPS=/Users/nickrodriguez/Documents/_project_resources/KyberVision22API/session_videos/montage_clips
PATH_VIDEOS_MONTAGE_COMPLETE=/Users/nickrodriguez/Documents/_project_resources/KyberVision22API/session_videos/montage_complete
ADMIN_EMAIL_ADDRESS=kyber.vision.info@gmail.com
ADMIN_EMAIL_PASSWORD="secret_code"
PATH_DB_BACKUPS=/Users/nickrodriguez/Documents/_project_resources/KyberVision22API/db_backups
PATH_PROJECT_RESOURCES=/Users/nickrodriguez/Documents/_project_resources/KyberVision22API
ADMIN_EMAIL_KV_MANAGER_WEBSITE=["nrodrig1@gmail.com"]
URL_KV_MANAGER_WEBSITE=https://kv22-manager.dashanddata.com
URL_KV_JOB_QUEUER=http://localhost:8003
PATH_KV_VIDEO_PROCESSOR=/Users/nickrodriguez/Documents/KyberVisionVideoProcessor01
NAME_KV_VIDEO_PROCESSOR=videoProcessor.js
URL_BASE_KV_API=https://api.kv22.dashanddata.com
PATH_TEST_REQUEST_ARGS=/Users/nickrodriguez/Documents/project_resources/KyberVision22API/test_request_args
NODE_ENV=production
AUTHENTIFICATION_TURNED_OFF=false
```

## Folder Structure

```
.
├── CLAUDE.md
├── dist
│   ├── app.js
│   ├── modules
│   │   ├── adminDb.js
│   │   ├── common.js
│   │   ├── contractVideoAction.js
│   │   ├── mailer.js
│   │   ├── onStartUp.js
│   │   ├── players.js
│   │   ├── sessions.js
│   │   ├── userAuthentication.js
│   │   └── videos.js
│   ├── routes
│   │   ├── adminDb.js
│   │   ├── contractPlayerUsers.js
│   │   ├── contractTeamUsers.js
│   │   ├── contractUserActions.js
│   │   ├── contractVideoActions.js
│   │   ├── index.js
│   │   ├── leagues.js
│   │   ├── players.js
│   │   ├── scripts.js
│   │   ├── sessions.js
│   │   ├── teams.js
│   │   ├── users.js
│   │   └── videos.js
│   └── server.js
├── docs
│   ├── API_REFERENCE.md
│   ├── DATABASE_SCHEMA_OVERVIEW.md
│   ├── images
│   │   └── kyberVisionLogo01.png
│   ├── KyberVision18ApiReference
│   │   ├── app.js
│   │   ├── modules
│   │   └── routes
│   └── TS_CONVERSION_STATUS.md
├── package-lock.json
├── package.json
├── README.md
├── src
│   ├── app.ts
│   ├── modules
│   │   ├── adminDb.ts
│   │   ├── common.ts
│   │   ├── contractVideoAction.ts
│   │   ├── mailer.ts
│   │   ├── onStartUp.ts
│   │   ├── players.ts
│   │   ├── sessions.ts
│   │   ├── userAuthentication.ts
│   │   └── videos.ts
│   ├── public
│   ├── routes
│   │   ├── adminDb.ts
│   │   ├── contractPlayerUsers.ts
│   │   ├── contractTeamUsers.ts
│   │   ├── contractUserActions.ts
│   │   ├── contractVideoActions.ts
│   │   ├── index.ts
│   │   ├── leagues.ts
│   │   ├── players.ts
│   │   ├── scripts.ts
│   │   ├── sessions.ts
│   │   ├── teams.ts
│   │   ├── users.ts
│   │   └── videos.ts
│   ├── server.ts
│   └── templates
│       ├── registrationConfirmationEmail.html
│       ├── requestToRegisterEmail.html
│       ├── resetPasswordLinkEmail.html
│       └── videoMontageCompleteNotificationEmail.html
└── tsconfig.json
```
