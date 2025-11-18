---
name: Bug Report
about: Report a bug in the application or pipeline.
title: "[BUG] "
labels: bug
assignees: ''
---

## Description  
Users are unable to see updated poll results on the landing page unless they manually refresh the browser. The real-time polling feature appears to be broken.

## Steps to Reproduce  
1. Open the landing page on localhost:5173  
2. Vote on any poll  
3. Observe that the vote count does not update automatically

## Expected Behavior  
Vote results should update instantly via API response without requiring a page refresh.

## Actual Behavior  
Votes are submitted successfully, but UI does not refresh with new poll percentages.

## Environment  
Branch: frontend/landing-page  
Commit SHA: a3f9c42  
Environment: development

## Screenshots  
(Add screenshot of frontend poll not updating)

## Additional Context  
The WebSocket/long-polling logic has not been implemented yet. Backend currently returns the updated value, but frontend does not re-fetch after vote submission.
