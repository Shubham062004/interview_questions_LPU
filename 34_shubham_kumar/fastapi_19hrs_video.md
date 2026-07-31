Here are **50 medium-level interview questions** inspired by the course.

---

# Python & FastAPI Fundamentals (1–10)

1. Why did the instructor choose FastAPI instead of Flask or Django?
2. What are the main advantages of FastAPI?
3. Explain how FastAPI automatically generates API documentation.
4. What is ASGI, and why does FastAPI use it?
5. Explain the lifecycle of a FastAPI request.
6. What are Path Operations in FastAPI?
7. How do Path Parameters differ from Query Parameters?
8. Why does the order of routes matter in FastAPI?
9. What is dependency injection in FastAPI?
10. How does FastAPI perform request validation?

---

# Pydantic & Validation (11–15)

11. What is Pydantic?
12. Why does FastAPI use Pydantic models?
13. Difference between request models and response models.
14. Explain schema validation with an example.
15. What is the difference between a Pydantic model and a SQLAlchemy model?

---

# REST APIs & CRUD (16–20)

16. Explain CRUD operations in REST APIs.
17. Why should POST return **201 Created** instead of **200 OK**?
18. Explain idempotent HTTP methods.
19. Difference between PUT and PATCH.
20. How should API error responses be designed?

---

# PostgreSQL & SQL (21–28)

21. Why use PostgreSQL instead of SQLite for production?
22. Explain primary keys and foreign keys.
23. What are database constraints?
24. Difference between WHERE, LIKE, and IN.
25. Explain ORDER BY, LIMIT, and OFFSET.
26. What are SQL joins, and when would you use them?
27. Difference between INNER JOIN and LEFT JOIN.
28. How would you optimize a slow SQL query?

---

# SQLAlchemy ORM (29–34)

29. What is an ORM, and why use SQLAlchemy?
30. Difference between raw SQL and SQLAlchemy ORM.
31. How are relationships defined in SQLAlchemy?
32. Explain one-to-many relationships.
33. How does SQLAlchemy handle database sessions?
34. What is lazy loading in an ORM?

---

# Authentication & Security (35–40)

35. Explain the complete JWT authentication flow.
36. Why should passwords never be stored in plain text?
37. How does password hashing work?
38. What is OAuth2 PasswordRequestForm?
39. How do protected routes work in FastAPI?
40. What happens when a JWT token expires?

---

# Alembic & Database Migrations (41–43)

41. What problem does Alembic solve?
42. Why are migrations better than recreating the database?
43. How do you roll back a migration?

---

# Docker & Deployment (44–47)

44. What should a production Dockerfile for FastAPI include?
45. Difference between Docker Image and Docker Container.
46. Why use Docker Compose with FastAPI and PostgreSQL?
47. Why should environment variables be used instead of hard-coded credentials?

---

# Testing & CI/CD (48–50)

48. How do you test FastAPI endpoints using `TestClient`?
49. What are pytest fixtures, and why are they useful?
50. Explain how a GitHub Actions CI/CD pipeline works for a FastAPI application.

---

## Interview Follow-up Questions (Very Likely)

After many of the questions above, interviewers may ask:

* Can you explain what happens internally?
* Can you draw the request flow?
* How did you implement this in one of your projects?
* What are the common mistakes?
* What are the security implications?
* How would you scale this in production?
* How would you optimize performance?
* What are the alternatives?
* How would you debug an issue here?
* How would you test this feature?

