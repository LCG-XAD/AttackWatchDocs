# AttackWatch

## Release Notes

### version 1.1.25.12 (2025-03-24) 

### Overview:

This release introduces improvements to the logging system, an enhanced language system, and several bug fixes.
It aims to optimize server performance, stability, and usability.

### 🚀 Added (New Features & Improvements):

-   [AW-15](https://lcg-xad.atlassian.net/jira/software/c/projects/AW/boards/7?selectedIssue=AW-15 'AW-15'): Improved Feedback panel with feedback type selection. Enhanced the AttackWatch feedback input by replicating Jira's modal feedback input. The email notification now includes the selected feedback type.

![AW-15_1](https://github.com/user-attachments/assets/9e4eedc7-bec4-4aa2-a520-38c6669c363c)


-   [AW-17](https://lcg-xad.atlassian.net/jira/software/c/projects/AW/boards/7?selectedIssue=AW-17 'AW-17'): Implemented a new Activity Logger in AttackWatch. It records all created, modified, and deleted data, as well as sent emails and requests.

| Log Table | Log Info |
|---------|---------|
| ![AW-17_1](https://github.com/user-attachments/assets/d54a51c5-5bee-438b-9398-07eb48aa0393) | ![AW-17_2](https://github.com/user-attachments/assets/23e0c861-b0c6-4fc3-9818-630de7b85a70) |


-   [AW-28](https://lcg-xad.atlassian.net/jira/software/c/projects/AW/boards/7?selectedIssue=AW-28 'AW-28'): Enabled multi-language support for AttackWatch. We added a button to switch between supported languages in the interface. We implemented a new translation system inside AttackWatch and created its translations.

| English | Portuguese Translation |
|---------|---------|
| ![AW-28_1](https://github.com/user-attachments/assets/205075fe-2751-4a5e-81ba-2ff48ff40a0a) | ![AW_28_2](https://github.com/user-attachments/assets/4ff45389-c5f9-4e43-8380-e6c99f3f47db) |


-   [AW-29](https://lcg-xad.atlassian.net/jira/software/c/projects/AW/boards/7?selectedIssue=AW-29 'AW-29'): We improved the AttackWatch dashboard for compromised accounts by updating the labels. We replaced the "Last Month Compromised Accounts" with the "Total Compromised Accounts" metric.

![AW-29](https://github.com/user-attachments/assets/859f89c2-8a2b-42f1-bd92-2a9b76f4af05)


-   [AW-49](https://lcg-xad.atlassian.net/jira/software/c/projects/AW/boards/7?selectedIssue=AW-49 'AW-49'): Added web server release notes to the footer. This release note allows users to see which version of AttackWatch is currently running.

![AW-49](https://github.com/user-attachments/assets/d4f670c3-be98-4dd0-bc60-d6b57cd2769c)


### 🪲 Fixed (Bugs):

-   [AW-31](https://lcg-xad.atlassian.net/jira/software/c/projects/AW/boards/7?selectedIssue=AW-31 'AW-31'): Fixed issue where submitting the first feedback required changing the type first when selecting "Ask a Question". The bug was found in the new feedback modal created in AW-15. The "Ask a Question" option would be locked unless another type was selected first. To fix this, we added a default label 'Choose one'.

-   [AW-47](https://lcg-xad.atlassian.net/jira/software/c/projects/AW/boards/7?selectedIssue=AW-47 'AW-47'): Fixed an issue where the new translation feature caused the 'faker' functionality in .sh files to stop working. Due to the new translation feature in AW-28, the 'faker' functionality in .sh files stopped working.

-   [AW-48](https://lcg-xad.atlassian.net/jira/software/c/projects/AW/boards/7?selectedIssue=AW-48 'AW-48'): A bug was found during the initial AttackWatch setup. AttackWatch raises an error when trying to create the first user of the Webserver due to the new log validations in AW-17.

### ❌ Removed:

-   N/A
