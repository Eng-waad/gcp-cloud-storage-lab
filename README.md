#  GCP Cloud Storage Security 

This project demonstrates hands-on experience with Google Cloud Storage, focusing on security, encryption, lifecycle management, and versioning.

---

##  Project Overview

In this lab, I implemented a secure and managed cloud storage solution using GCP. The work includes:

- Creating and configuring a Cloud Storage bucket
- Managing access using ACL (Access Control Lists)
- Applying Customer-Supplied Encryption Keys (CSEK)
- Performing encryption key rotation
- Configuring lifecycle management policies
- Enabling object versioning and recovery
- Synchronizing local directories with Cloud Storage

---

##  Lab Tasks

### 1. Bucket Creation
- Created a globally unique bucket in us-central1
- Used fine-grained access control

### 2. Access Control (ACL)
- Uploaded objects to the bucket
- Set object access to private
- Modified permissions to make an object publicly readable

### 3. Customer-Supplied Encryption Keys (CSEK)
- Generated AES-256 encryption key
- Configured .boto file
- Uploaded encrypted objects to Cloud Storage

### 4. Key Rotation
- Rotated encryption keys securely
- Re-encrypted selected objects
- Verified behavior when old keys are removed

### 5. Lifecycle Management
- Created lifecycle policy to automatically delete objects after 31 days

### 6. Object Versioning
- Enabled versioning on the bucket
- Uploaded multiple versions of a file
- Recovered an older version successfully

### 7. Directory Synchronization
- Created nested directory structure
- Synced local files to Cloud Storage using gsutil rsync

---

##  Screenshots

All screenshots are available in the screenshots/ directory.

| Step | Description |
|------|------------|
| 1 | Bucket overview |
| 2 | Files inside bucket |
| 3 | Public access (ACL) |
| 4 | CLI ACL verification |
| 5 | Encryption proof (CSEK) |
| 6 | Lifecycle policy |
| 7 | Versioning enabled |
| 8 | Version history |
| 9| Lab completion |

---

##  Key Learnings

- Implemented secure access control using ACL
- Learned how to use Customer-Supplied Encryption Keys (CSEK)
- Understood how encryption key rotation works in practice
- Applied lifecycle policies for automated storage management
- Used versioning to protect and recover data
- Practiced real-world cloud storage operations using CLI tools

---

##  Challenges Faced

- .boto file was initially empty and required manual configuration
- Encryption was not applied correctly until objects were re-uploaded
- Understanding key rotation behavior and its effect on object access

---

##  Outcome

Successfully built a secure, encrypted, and managed Cloud Storage solution using GCP with real-world practices including access control, encryption, lifecycle automation, and version recovery.

---

##  Tools & Technologies

- Google Cloud Platform (GCP)
- Cloud Storage
- gsutil & gcloud CLI
- Cloud Shell

---

## Notes

- Sensitive information such as encryption keys and project IDs has been removed or hidden.
- This lab was completed as part of hands-on cloud engineering training.
