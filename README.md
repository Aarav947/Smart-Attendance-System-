# Smart-Attendance-System-

What It Does
Detects faces via webcam, extracts 512-dimensional embeddings using FaceNet, and matches them against a stored database using cosine similarity. Attendance is logged automatically with blink-based liveness verification to prevent spoofing.
ML Pipeline

Face Detection — MediaPipe BlazeFace
Embedding Extraction — FaceNet (512-D feature vectors)
Embedding Storage — SQLite database
Similarity Matching — Cosine distance
Classification — Threshold-based match vs unknown
Liveness Verification — Blink detection before logging
Backend Logging — Confidence score + once-per-day duplication control

Key Features

98%+ identification accuracy across varying lighting.
Blink-based anti-spoofing (prevents photo attacks)
FastAPI backend with exportable CSV attendance records

Tech Stack
Python · FaceNet · MediaPipe · FastAPI · SQLite · OpenCV
