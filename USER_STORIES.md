# User Stories - Library Management

## Group Information

- **Group Number:** G01
- **Module:** Library Management
- **Group Label:** team-01
- **Product Owner:** Ameed (ameed499)
- **Story Writer:** Ameed (ameed499)
- **Task Planner:** Ameed (ameed499)
- **Tester:** Shairy-prog
- **Reviewer:** Shairy-prog
- **Note:** The group has two members, so some roles are shared. The tester and reviewer of each story is the other group member where possible.

---

## US-01 - Search books by title, author or subject

### User Story
As a student,
I want to search for books by title, author or subject,
so that I can quickly find a required book without visiting every shelf.

### Acceptance Criteria
- [x] The library page displays a search box with a choice of title, author or subject.
- [x] The system displays books that match the complete or partial text entered.
- [x] The system displays "No books found" when no book matches the search.

### Technical Tasks
- [x] Design the search interface.
- [x] Implement the search function for title, author and subject.
- [x] Validate blank search input.
- [x] Test valid, partial and invalid search values.
- [x] Update the README with the search feature.

### Story Information
- **Priority:** High
- **Assignee:** ameed499
- **Status:** Done
- **Labels:** `type:user-story`, `team-01`

### Definition of Done
- [x] All acceptance criteria are satisfied.
- [x] The assigned tester has verified the story.
- [x] Another group member has reviewed the work.
- [x] The team has recorded the required evidence.

---

## US-02 - View book availability

### User Story
As a student,
I want to see whether a book is available or issued,
so that I do not go to the library for a book that is not on the shelf.

### Acceptance Criteria
- [x] Every book in the search results shows its status as Available or Issued.
- [x] An issued book shows its expected return date.
- [x] The status changes when a book is issued or returned.

### Technical Tasks
- [x] Design the availability label on the book result.
- [x] Implement the availability status check.
- [x] Validate the return date display for issued books.
- [x] Test an available book, an issued book and a returned book.
- [x] Update the README with the availability feature.

### Story Information
- **Priority:** High
- **Assignee:** Shairy-prog
- **Status:** Done
- **Labels:** `type:user-story`, `team-01`

### Definition of Done
- [x] All acceptance criteria are satisfied.
- [x] The assigned tester has verified the story.
- [x] Another group member has reviewed the work.
- [x] The team has recorded the required evidence.

---

## US-03 - Reserve an available book

### User Story
As a student,
I want to reserve an available book,
so that the book is kept for me until I reach the library.

### Acceptance Criteria
- [x] A Reserve button is shown only for books that are available.
- [x] After the student reserves a book, the system shows a confirmation message and the book status changes to Reserved.
- [x] The system rejects a reservation for a book that is already issued or reserved and shows a clear message.
- [x] A reservation is automatically cancelled 24 hours after it is made and the book becomes available again.

### Technical Tasks
- [x] Design the reserve button and confirmation message.
- [x] Implement the reservation function.
- [x] Validate that issued or reserved books cannot be reserved.
- [x] Test reserving an available book and an unavailable book.
- [x] Update the README with the reservation feature.
- [x] Implement a scheduled check that expires reservations older than 24 hours.

### Story Information
- **Priority:** High
- **Assignee:** ameed499
- **Status:** Done
- **Labels:** `type:user-story`, `team-01`

### Definition of Done
- [x] All acceptance criteria are satisfied.
- [x] The assigned tester has verified the story.
- [x] Another group member has reviewed the work.
- [x] The team has recorded the required evidence.

---

## US-04 - Renew an issued book

### User Story
As a student,
I want to renew a book that is issued to me,
so that I can keep it longer without visiting the library desk.

### Acceptance Criteria
- [x] A Renew option is shown for each book currently issued to the student.
- [x] After renewal, the return date moves forward by 7 days and the new date is displayed.
- [x] The system rejects the renewal with a clear message when another student has reserved the book.

### Technical Tasks
- [x] Design the renew option on the issued books page.
- [x] Implement the renewal function and return date update.
- [x] Validate the renewal against existing reservations.
- [x] Test a successful renewal and a rejected renewal.
- [x] Update the README with the renewal feature.

### Story Information
- **Priority:** Medium
- **Assignee:** Shairy-prog
- **Status:** Done
- **Labels:** `type:user-story`, `team-01`

### Definition of Done
- [x] All acceptance criteria are satisfied.
- [x] The assigned tester has verified the story.
- [x] Another group member has reviewed the work.
- [x] The team has recorded the required evidence.

---

## US-05 - Receive a return date reminder

### User Story
As a student,
I want to receive a reminder before my book is due,
so that I can return or renew it on time and avoid a late fine.

### Acceptance Criteria
- [x] The system sends a reminder 2 days before the return date.
- [x] The reminder shows the book title and the return date.
- [x] A student with no books due soon does not receive a reminder.

### Technical Tasks
- [x] Design the reminder message.
- [x] Implement the reminder check based on the return date.
- [x] Validate that the reminder is sent only once per book.
- [x] Test a book due in 2 days and a book not due soon.
- [x] Update the README with the reminder feature.

### Story Information
- **Priority:** Medium
- **Assignee:** ameed499
- **Status:** Done
- **Labels:** `type:user-story`, `team-01`

### Definition of Done
- [x] All acceptance criteria are satisfied.
- [x] The assigned tester has verified the story.
- [x] Another group member has reviewed the work.
- [x] The team has recorded the required evidence.

---

## Change Challenge Response

- **Affected User Story:** US-03 - Reserve an available book
- **New Requirement:** A reservation must automatically expire after 24 hours.
- **Updated Acceptance Criterion:** A reservation is automatically cancelled 24 hours after it is made and the book becomes available again.
- **New or Updated Task:** Implement a scheduled check that expires reservations older than 24 hours.

## Peer Review

- **Reviewed By Group:** G01 (internal review by Shairy-prog on US-01, as no other group was available)
- **User role is clear:** Yes
- **User value is clear:** Yes
- **Acceptance criteria are testable:** Yes
- **Missing condition:** The criteria do not say whether the search ignores upper and lower case letters.
- **Recommended improvement:** Add a criterion that the search returns the same results for "Java", "java" and "JAVA".
