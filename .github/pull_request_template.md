## 🎯 Objective
<!-- A clear, direct description of what this PR does. What did you add or fix? -->
- **Problem / Feature:** [Write here, e.g., Add task time-extension when due date is missed]
- **Business goal:** [Why do we need this? e.g., So Admins can see the reason for delay before approving]

---

## 🏗️ Technical and Architectural Changes
<!-- Which parts of the system were touched to implement this feature? -->
- **Layers Touched:**
  - [ ] Domain Layer (modify or add Entities/Enums)
  - [ ] Application Layer (add DTOs, Validators, Services)
  - [ ] Infrastructure Layer (DbContext, Repositories, Migrations)
  - [ ] Presentation/API Layer (Controllers, Endpoints)
- **Design Patterns Applied:** [e.g., Repository Pattern; Result Pattern]

---

## 🧠 Final Boss and Engineering Decisions
<!-- This section prepares you for interviews. Answer precisely and in detail. -->

### 1. Trade-offs and Alternatives
- **Why this solution?** [Explain why you wrote the code this way]
- **Alternatives considered and why rejected:** [e.g., considered X but rejected due to performance impact]
- **Known drawbacks of the chosen solution:** [No code is perfect; list limitations honestly]

### 2. Failure Points and Edge Cases
- **When will this code fail?** [e.g., user supplies a past date; ID not found]
- **How are these cases handled?** [e.g., added Custom Exception; used FluentValidation]

### 3. Debugging Reality
- **Hardest bug encountered:** [Describe the bug, how you traced it, and how you fixed it]

---

## 🛡️ Code Quality and Testing
<!-- How did you ensure the code works and won’t break the system? -->
- **How was it tested?**
  - [ ] Manual testing (Postman or Swagger)
  - [ ] Unit tests added
- **Database impact:**
  - [ ] No database changes
  - [ ] New migration added named: `[migration name here]`

---

## ✅ Checklist
<!-- Ensure strict rules are followed before merging -->
- [ ] Code fully respects Clean Architecture boundaries (e.g., no DbContext in API)
- [ ] No business logic inside controllers (controllers only route requests)
- [ ] Notion documentation (Knowledge Base & Execution Log) updated
- [ ] README updated if necessary
