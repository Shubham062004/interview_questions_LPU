# Python & FastAPI Fundamentals (One-Line Answers)

1. Why did the instructor choose FastAPI instead of Flask or Django? 
  — It is fast, async-friendly, and includes built-in validation and docs.

2. What are the main advantages of FastAPI? 
  — It is fast, easy to write, reduces bugs, and follows OpenAPI standards.

3. How does FastAPI generate API documentation? 
  — It uses type hints and Pydantic to create Swagger and ReDoc docs automatically.

4. What is ASGI, and why does FastAPI use it? 
  — ASGI supports async, non-blocking requests and WebSockets.

5. What is the lifecycle of a FastAPI request? 
  — Request -> middleware -> routing -> validation -> handler -> response.

6. What are Path Operations in FastAPI? 
  — They are route handlers decorated with HTTP methods like get/post/put/delete.

7. How do path parameters differ from query parameters? 
  — Path params go in the URL path; query params go after ?.

8. Why does route order matter in FastAPI? 
  — Specific routes should be declared before dynamic routes to avoid overlap.

9. What is dependency injection in FastAPI? 
  — It lets endpoints reuse shared dependencies like DB sessions and auth checks.

10. How does FastAPI perform request validation? 
  — It validates inputs using Python types and Pydantic and returns 422 on failure.

## Pydantic & Validation

11. What is Pydantic? 
  — It validates and parses data using Python type hints.

12. Why does FastAPI use Pydantic models? 
  — They provide validation, parsing, serialization, and schema generation.

13. Difference between request and response models? 
  — Request models validate input; response models shape output.

14. Explain schema validation with an example. 
  — Fields can use constraints like min length and positive integers.

15. Difference between Pydantic and SQLAlchemy models? 
  — Pydantic validates API data; SQLAlchemy maps database tables.

## REST APIs & CRUD

16. Explain CRUD operations in REST APIs. 
  — Create, read, update, and delete resources using HTTP methods.

17. Why should POST return 201 Created? 
  — It clearly indicates that a new resource was created.

18. What are idempotent HTTP methods? 
  — Methods like GET, PUT, and DELETE that can be retried safely.

19. Difference between PUT and PATCH. 
  — PUT replaces the whole resource; PATCH updates only part of it.

20. How should API error responses be designed? 
  — They should return clear status codes and structured error details.

## PostgreSQL & SQL

21. Why use PostgreSQL instead of SQLite for production? 
  — PostgreSQL is more scalable, concurrent, and feature-rich.

22. Explain primary keys and foreign keys. 
  — Primary keys uniquely identify rows; foreign keys link rows across tables.

23. What are database constraints? 
  — They enforce rules like uniqueness, not null, and relationships.

24. Difference between WHERE, LIKE, and IN. 
  — WHERE filters exactly; LIKE matches patterns; IN checks a list.

25. Explain ORDER BY, LIMIT, and OFFSET. 
  — They sort, restrict, and paginate query results.

26. What are SQL joins, and when would you use them? 
  — They combine data from related tables.

27. Difference between INNER JOIN and LEFT JOIN. 
  — INNER returns matches only; LEFT keeps all rows from the left table.

28. How would you optimize a slow SQL query? 
  — Use EXPLAIN ANALYZE, add indexes, and reduce unnecessary data fetches.

## SQLAlchemy ORM

29. What is an ORM, and why use SQLAlchemy? 
  — It maps database tables to Python objects for easier development.

30. Raw SQL vs SQLAlchemy ORM. 
  — Raw SQL is faster but less safe and less abstracted; ORM is cleaner and safer.

31. How are relationships defined in SQLAlchemy? 
  — With ForeignKey and relationship helpers.

32. Explain one-to-many relationships. 
  — One parent can have many children, but each child has one parent.

33. How does SQLAlchemy handle database sessions? 
  — It tracks changes and commits or rolls back them atomically.

34. What is lazy loading in an ORM? 
  — It loads related data only when it is accessed.

## Authentication & Security

35. Explain the complete JWT authentication flow. 
  — Client logs in, receives a token, and sends it in the Authorization header.

36. Why should passwords never be stored in plain text? 
  — They can be exposed in a breach and reused across services.

37. How does password hashing work? 
  — It transforms passwords into one-way hashes with salts.

38. What is OAuth2 PasswordRequestForm? 
  — It parses login form data for FastAPI token endpoints.

39. How do protected routes work in FastAPI? 
  — They require a valid token through a dependency check.

40. What happens when a JWT token expires? 
  — It becomes invalid and returns 401 Unauthorized.

## Alembic & Database Migrations

41. What problem does Alembic solve? 
  — It tracks and applies schema changes safely across environments.

42. Why are migrations better than recreating the database? 
  — They preserve existing data and apply changes incrementally.

43. How do you roll back a migration? 
  — Use alembic downgrade to revert to a previous revision.

## Docker & Deployment

44. What should a production Dockerfile for FastAPI include? 
  — A slim Python image, dependencies, app code, and a uvicorn command.

45. Difference between Docker Image and Docker Container. 
  — An image is a template; a container is a running instance.

46. Why use Docker Compose with FastAPI and PostgreSQL? 
  — It runs multiple services together with shared networking and storage.
47. Why should environment variables be used instead of hard-coded 
credentials? 
  — They keep secrets out of source code and support different environments.

## Testing & CI/CD

48. How do you test FastAPI endpoints using TestClient? 
  — Use pytest and TestClient to simulate requests in memory.

49. What are pytest fixtures, and why are they useful? 
  — They set up reusable test dependencies and isolate state.
50. Explain how a GitHub Actions CI/CD pipeline works for a FastAPI 
application. 
  — It runs tests, builds the app, and deploys it automatically.
