# 📁 Document Storage API

Secure backend for personal document storage with JWT authentication.

## Features
- ✅ User Registration & Login (JWT)
- ✅ Upload files (PDF, Images only)
- ✅ Download own files only
- ✅ File metadata (name, size, timestamp)
- ✅ File ownership validation
- ✅ Error handling (empty files, wrong formats, unauthorized access)

## Tech Stack
- Node.js + Express
- MongoDB + Mongoose
- Multer (file uploads)
- JWT Authentication

## API Endpoints
- Method	Endpoint	Description
- POST	/api/auth/register	Register user
- POST	/api/auth/login	Login (get token)
- POST	/api/files/upload	Upload file
- GET	/api/files/my-files	Get all my files
- GET	/api/files/download/:id	Download file
- DELETE	/api/files/:id	Delete file
  
  ## Security Features
- Only owner can download their files
- File type validation (PDF, JPG, PNG only)
- File size limit (5MB)
- JWT token required for all file operations
