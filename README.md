# Matillion Tech Test 2025 Solution

This repository contains my completed solution for the Matillion placement student technical test.

## Solution Overview

### ✅ Part 1: Fixed Failing Tests
- Implemented CSV parsing with null value detection
- Added error handling for malformed CSV and content validation
- All 14 Part 1 tests passing

### ✅ Part 2: Extended API Functionality  
- GET `/api/analysis/{id}` - Retrieve previous analyses
- DELETE `/api/analysis/{id}` - Delete analysis records
- Unique value counting across all columns
- All 12 Part 2 tests passing

### ✅ Part 3: Creative Feature - Data Health Scoring
- GET `/api/analysis/{id}/health` - Data quality assessment endpoint
- Returns: healthScore (0-100), completenessPercentage, healthStatus
- Scoring: EXCELLENT (95%+), GOOD (80-94%), FAIR (60-79%), POOR (<60%)
- Helps users quickly understand data quality

## Running the Solution

```bash
./gradlew test    # Run all tests (26 tests total)
./gradlew bootRun # Start the application on http://localhost:8080
