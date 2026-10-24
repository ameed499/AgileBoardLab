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
- **Note:** The group has two members, so some roles are shared. The tester and reviewer of a story are always different from its assignee.

---

## US-01 - Search books by title, author or subject

### User Story
As a student,
I want to search for books by title, author or subject,
so that I can quickly find a required book without visiting every shelf.

### Acceptance Criteria
- [ ] The library page displays a search box with a choice of title, author or subject.
- [ ] The system displays books that match the complete or partial text entered.
- [ ] The system displays "No books found" when no book matches the search.

### Technical Tasks
- [ ] Design the search interface.
- [ ] Implement the search function for title, author and subject.
- [ ] Validate blank search input.
- [ ] Test valid, partial and invalid search values.
- [ ] Update the README with the search feature.

### Story Information
- **Priority:** High
- **Assignee:** ameed499
- **Status:** Backlog
- **Labels:** `type:user-story`, `team-01`

### Definition of Done
- [ ] All acceptance criteria are satisfied.
- [ ] The assigned tester has verified the story.
- [ ] Another group member has reviewed the work.
- [ ] The team has recorded the required evidence.

---

## US-02 - View book availability

### User Story
As a student,
I want to see whether a book is available or issued,
so that I do not go to the library for a book that is not on the shelf.

### Acceptance Criteria
- [ ] Every book in the search results shows its status as Available or Issued.
- [ ] An issued book shows its expected return date.
- [ ] The status changes when a book is issued or returned.

### Technical Tasks
- [ ] Design the availability label on the book result.
- [ ] Implement the availability status check.
- [ ] Validate the return date display for issued books.
- [ ] Test an available book, an issued book and a returned book.
- [ ] Update the README with the availability feature.

### Story Information
- **Priority:** High
- **Assignee:** Shairy-prog
- **Status:** Backlog
- **Labels:** `type:user-story`, `team-01`

### Definition of Done
- [ ] All acceptance criteria are satisfied.
- [ ] The assigned tester has verified the story.
- [ ] Another group member has reviewed the work.
- [ ] The team has recorded the required evidence.

---

## US-03 - Reserve an available book

### User Story
As a student,
I want to reserve an available book,
so that the book is kept for me until I reach the library.

### Acceptance Criteria
- [ ] A Reserve button is shown only for books that are available.
- [ ] After the student reserves a book, the system shows a confirmation message and the book status changes to Reserved.
- [ ] The system rejects a reservation for a book that is already issued or reserved and shows a clear message.

### Technical Tasks
- [ ] Design the reserve button and confirmation message.
- [ ] Implement the reservation function.
- [ ] Validate that issued or reserved books cannot be reserved.
- [ ] Test reserving an available book and an unavailable book.
- [ ] Update the README with the reservation feature.

### Story Information
- **Priority:** High
- **Assignee:** ameed499
- **Status:** Backlog
- **Labels:** `type:user-story`, `team-01`

### Definition of Done
- [ ] All acceptance criteria are satisfied.
- [ ] The assigned tester has verified the story.
- [ ] Another group member has reviewed the work.
- [ ] The team has recorded the required evidence.

---

## US-04 - Renew an issued book

### User Story
As a student,
I want to renew a book that is issued to me,
so that I can keep it longer without visiting the library desk.

### Acceptance Criteria
- [ ] A Renew option is shown for each book currently issued to the student.
- [ ] After renewal, the return date moves forward by 7 days and the new date is displayed.
- [ ] The system rejects the renewal with a clear message when another student has reserved the book.

### Technical Tasks
- [ ] Design the renew option on the issued books page.
- [ ] Implement the renewal function and return date update.
- [ ] Validate the renewal against existing reservations.
- [ ] Test a successful renewal and a rejected renewal.
- [ ] Update the README with the renewal feature.

### Story Information
- **Priority:** Medium
- **Assignee:** Shairy-prog
- **Status:** Backlog
- **Labels:** `type:user-story`, `team-01`

### Definition of Done
- [ ] All acceptance criteria are satisfied.
- [ ] The assigned tester has verified the story.
- [ ] Another group member has reviewed the work.
- [ ] The team has recorded the required evidence.

---

## US-05 - Receive a return date reminder

### User Story
As a student,
I want to receive a reminder before my book is due,
so that I can return or renew it on time and avoid a late fine.

### Acceptance Criteria
- [ ] The system sends a reminder 2 days before the return date.
- [ ] The reminder shows the book title and the return date.
- [ ] A student with no books due soon does not receive a reminder.

### Technical Tasks
- [ ] Design the reminder message.
- [ ] Implement the reminder check based on the return date.
- [ ] Validate that the reminder is sent only once per book.
- [ ] Test a book due in 2 days and a book not due soon.
- [ ] Update the README with the reminder feature.

### Story Information
- **Priority:** Medium
- **Assignee:** ameed499
- **Status:** Backlog
- **Labels:** `type:user-story`, `team-01`

### Definition of Done
- [ ] All acceptance criteria are satisfied.
- [ ] The assigned tester has verified the story.
- [ ] Another group member has reviewed the work.
- [ ] The team has recorded the required evidence.

---

## Change Challenge Response

- **Affected User Story:** US-03 - Reserve an available book
- **New Requirement:** A reservation must automatically expire after 24 hours if the student does not collect the book.
- **Updated Acceptance Criterion:** [ ] A reservation that is not collected within 24 hours expires automatically, and the book status returns to Available.
- **New or Updated Task:** [ ] Implement the 24-hour expiry check for reservations and test it with a reservation older than 24 hours.

## Peer Review

- **Reviewed By Group:** [Write the number of the group you reviewed]
- **User role is clear:** [Yes / No]
- **User value is clear:** [Yes / No]
- **Acceptance criteria are testable:** [Yes / No]
- **Missing condition:** [Write here]
- **Recommended improvement:** [Write here]
