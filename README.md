# ConflictCore — Multi-User File Management & Conflict Resolution System

> A database-backed multi-user file management system designed to safely handle concurrent file operations using process management, scheduling, file locking, deadlock handling, version tracking, and conflict resolution.

---

## 📌 Overview

**ConflictCore** is a Project-Based Learning (PBL) project that combines concepts from **Operating Systems, DBMS, Data Structures, and Backend Development** to build a controlled multi-user file management system.

When multiple users access or modify the same file simultaneously, problems such as:

- Lost updates
- Race conditions
- Inconsistent file states
- Resource contention
- Process waiting
- Deadlocks

can occur.

ConflictCore addresses these challenges by treating file operations as processes and coordinating them through **process scheduling, file-level locking, database-backed state management, deadlock handling, and conflict resolution mechanisms**.

---

## 🎯 Problem Statement

Traditional and collaborative file-sharing systems allow multiple users to access or modify shared files concurrently. Concurrent operations can result in lost updates, inconsistent data, race conditions, and possible deadlocks.

ConflictCore provides controlled file access, conflict visibility, process tracking, and database-backed coordination for concurrent file operations.

---

## 💡 Motivation

The project aims to:

- Prevent lost updates and inconsistent file data.
- Manage concurrent file operations safely.
- Control access to shared file resources.
- Track file operations and process states.
- Detect and handle resource contention and deadlocks.
- Provide visibility into concurrent operations.
- Demonstrate practical integration of OS and DBMS concepts.

---

## 👥 Target Users

ConflictCore is designed for:

- 👨‍🎓 Students collaborating on shared files
- 👨‍💻 Developers sharing project files
- 🏢 Small organizations and startups
- 👥 Teams working with shared resources
- 🛠️ Administrators monitoring file operations, locks, and processes

---

# ✨ Key Features

## 📁 File & Folder Management

- Create and manage folders
- Upload and manage file metadata
- Organize files using folder hierarchy
- Update and delete files
- Track file ownership

## 👤 User Management

- User creation
- User lookup by ID, username, and email
- User listing and updating
- User deactivation
- User deletion

## 🔐 File Permissions

- Grant permissions to users
- Check user permissions
- Update permissions
- Revoke permissions
- Retrieve permissions associated with files

## ⚙️ Process Management

Every file operation can be represented as a process.

Supported process states:

```text
NEW
READY
RUNNING
WAITING
TERMINATED
KILLED
