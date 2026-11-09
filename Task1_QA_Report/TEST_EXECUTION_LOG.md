# Task 1 — Test execution log
Target: https://demo.realworld.io
Tester: Jagadeesh Dangeti
Date/time: [fill actual date/time]
Browser/device: [fill]

The scenarios below are candidate tests, not confirmed defects. Record actual behavior.

| # | Scenario and steps | Expected behavior | Actual result | Pass/Fail | Screenshot |
|---|---|---|---|---|---|
| 1 | Sign-up: submit empty fields and malformed email | Required fields and email format validated | [record] | [ ] | [file] |
| 2 | Login: submit invalid credentials and blank fields | Clear safe error; app remains usable | [record] | [ ] | [file] |
| 3 | Create article: submit blank title/body | Invalid article blocked with guidance | [record] | [ ] | [file] |
| 4 | Edit/delete: test own article and another user's article if possible | Only owner can edit/delete | [record] | [ ] | [file] |
| 5 | Logout: refresh, press Back, revisit protected route | Protected actions require valid session | [record] | [ ] | [file] |

Also try long inputs, special characters, network interruption during save, repeated submit clicks, and page refresh. Mark a defect only if reproduced. If a scenario passes, test another edge case to find a real issue.
