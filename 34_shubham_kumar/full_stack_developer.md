# Full Stack Developer Interview Questions (One-Line Answers)

## JavaScript

1. What is the difference between var, let, and const? 
  — var is function-scoped and re-declarable; let and const are block-scoped and not re-declarable.

2. What is a closure? 
  — A closure lets an inner function access variables from its outer scope even after that scope ends.

3. Explain the event loop. 
  — It handles async tasks by processing the call stack, microtasks, and macrotasks in order.

4. Synchronous vs asynchronous programming? 
  — Sync blocks execution; async lets other work continue while waiting.

5. What are Promises? 
  — Promises represent future success or failure in async code and support chaining.

6. Explain async/await. 
  — It is syntax sugar over Promises that makes async code easier to read.

7. What is hoisting? 
  — Declarations are moved to the top of scope during execution setup.

8. Difference between == and ===? 
  — == coerces types; === checks both value and type.

9. What is the prototype chain? 
  — It allows objects to inherit properties and methods from other objects.

10. What is debouncing and throttling? 
  — Debounce delays repeated calls; throttle limits how often a function runs.

## React

11. Virtual DOM vs Real DOM? 
  — Virtual DOM is an in-memory copy used for efficient updates; Real DOM is the browser tree.

12. Explain React rendering lifecycle. 
  — React renders, diffs, commits updates, and runs effects.

13. useEffect vs useLayoutEffect? 
  — useEffect runs after paint; useLayoutEffect runs before paint.

14. Why should keys be unique? 
  — Unique keys help React track and update list items correctly.

15. When does React re-render? 
  — On state change, parent re-render, context change, or prop reference change.

16. Controlled vs uncontrolled components? 
  — Controlled components use React state; uncontrolled use DOM refs.

17. Context API vs Redux? 
  — Context is simple and built-in; Redux is better for complex shared state.

18. What is React reconciliation? 
  — It is the diffing algorithm React uses to update the UI efficiently.

19. What causes unnecessary re-renders? 
  — New object/function props, missing memoization, or context updates.

20. How do you optimize React performance? 
  — Use memoization, code splitting, and virtualized lists.

21. What are React hooks? 
  — Hooks let function components use state and lifecycle features.

22. Why can’t hooks be called conditionally? 
  — React depends on hooks being called in a stable order.

23. What are custom hooks? 
  — Custom hooks reuse stateful logic across components.

24. useMemo vs useCallback? 
  — useMemo memoizes values; useCallback memoizes functions.

25. What is React.lazy and Suspense? 
  — They enable lazy loading of components with a fallback UI.

## Next.js

26. SSR vs CSR vs SSG vs ISR? 
  — SSR renders per request, CSR on the client, SSG at build time, and ISR updates statically over time.

27. What is the App Router? 
  — It is the file-based routing system in Next.js using the app directory.

28. Server Components vs Client Components? 
  — Server Components render on the server; Client Components support interactivity.

29. What is middleware in Next.js? 
  — It runs before a request completes and can handle auth or redirects.

30. Explain routing in Next.js. 
  — Routes are mapped from files and folders in the app directory.

## HTML/CSS

31. Flexbox vs Grid? 
  — Flexbox is one-dimensional; Grid is two-dimensional.

32. What is the box model? 
  — It is the content, padding, border, and margin structure of an element.

33. What is z-index? 
  — It controls stacking order of positioned elements.

34. Absolute vs relative vs fixed positioning? 
  — Relative is relative to normal flow, absolute to a positioned ancestor, and fixed to the viewport.

35. How do you make a responsive website? 
  — Use flexible layouts, relative units, and media queries.

## Node.js

36. Why is Node.js single-threaded? 
  — It uses one main thread for async I/O and high concurrency.

37. How does Node.js handle multiple requests? 
  — It uses the event loop and background thread pool for I/O tasks.

38. Explain the event loop. 
  — It processes timers, I/O callbacks, and microtasks in phases.

39. What are streams? 
  — Streams process data in chunks without loading everything into memory.

40. process.nextTick vs setImmediate? 
  — nextTick runs before the next event loop phase; setImmediate runs in the check phase.

41. What is middleware? 
  — Middleware intercepts requests and can modify them or pass them along.

42. Express request lifecycle? 
  — Request -> middleware -> route handler -> response.

43. How do you organize a production Express project? 
  — Use a layered structure with controllers, services, models, and routes.

44. What is Helmet? 
  — It adds security headers to Express responses.

45. Explain CORS. 
  — It controls which origins can access your API from the browser.

46. How do you secure REST APIs? 
  — Use HTTPS, auth, validation, rate limiting, and headers.

47. Authentication vs authorization? 
  — Authentication checks identity; authorization checks permissions.

48. JWT flow? 
  — Login, sign token, send token, verify token on future requests.

49. Refresh token vs access token? 
  — Access tokens are short-lived; refresh tokens issue new access tokens.

50. Why is rate limiting important? 
  — It protects APIs from abuse, brute force, and overload.

## FastAPI

51. Why is FastAPI faster than Flask? 
  — It uses Starlette and Pydantic and supports async non-blocking requests.

52. What is ASGI? 
  — It is the async server interface that supports HTTP and WebSockets.

53. What is dependency injection? 
  — It lets functions receive dependencies from the framework instead of creating them manually.

54. How does FastAPI validation work? 
  — It validates inputs using Python type hints and Pydantic models.

55. Pydantic model vs ORM model? 
  — Pydantic validates API payloads; ORM models map database tables.

56. How do background tasks work? 
  — They run after the response is returned to keep the request fast.

57. Explain async endpoints. 
  — Async endpoints use await for non-blocking operations.

58. When should you use async? 
  — Use it for I/O-bound operations; use sync for blocking CPU-bound work.

59. What is FastAPI middleware? 
  — It runs around every request and response for cross-cutting concerns.

60. How do you deploy FastAPI? 
  — Run it with Uvicorn/Gunicorn, containerize it, and place it behind a proxy.

## REST APIs

61. REST principles. 
  — REST uses stateless, resource-based HTTP APIs with standard methods.

62. PUT vs PATCH? 
  — PUT replaces the whole resource; PATCH updates part of it.

63. POST vs PUT? 
  — POST creates a new resource; PUT creates or replaces a known resource.

64. What is idempotency? 
  — Repeating the same request should not change the state further.

65. Explain HTTP status codes. 
  — They describe the result of the request, such as success, redirect, or error.

66. What happens when a browser sends an API request? 
  — DNS, TCP/TLS, request, server processing, and response occur.

67. API versioning methods. 
  — Versioning can be done via URL, query params, or headers.

68. Pagination techniques. 
  — Offset pagination is simple; cursor pagination is better for large datasets.

69. Filtering and sorting APIs. 
  — Use query parameters for filters and sort order.

70. How do you document APIs? 
  — Use OpenAPI/Swagger and generated docs.

## Database

71. SQL vs NoSQL? 
  — SQL is relational and structured; NoSQL is flexible and scalable for unstructured data.

72. MongoDB vs PostgreSQL? 
  — MongoDB stores JSON-like documents; PostgreSQL stores relational tables with SQL features.

73. Explain indexing. 
  — Indexes speed up lookups by reducing the need to scan every row.

74. What is normalization? 
  — It reduces redundancy and improves data integrity.

75. Explain ACID properties. 
  — Atomicity, consistency, isolation, and durability ensure reliable transactions.

76. What are joins? 
  — Joins combine rows from related tables.

77. INNER vs LEFT JOIN? 
  — INNER returns only matches; LEFT returns all left rows plus matches.

78. Explain transactions. 
  — Transactions group database changes so they all succeed or all fail.

79. What is a foreign key? 
  — It links a row in one table to a row in another table.

80. Why do indexes improve performance? 
  — They turn scans into fast lookups using sorted structures.

81. What causes slow queries? 
  — Missing indexes, poor joins, large selects, and N+1 issues.

82. Explain aggregation pipeline in MongoDB. 
  — It transforms documents through stages like match, group, sort, and project.

## Authentication & Security

83. How does JWT authentication work? 
  — A server issues a signed token and the client sends it on future requests.

84. Explain OAuth. 
  — OAuth lets apps access user data through an authorization flow without exposing passwords.

85. Cookies vs localStorage? 
  — Cookies are sent automatically and can be HttpOnly; localStorage is accessible to JavaScript.

86. What is CSRF? 
  — It tricks a browser into sending unwanted authenticated requests.

87. What is XSS? 
  — It injects malicious scripts into a web app and runs them in browsers.

88. How do you prevent SQL injection? 
  — Use parameterized queries or a safe ORM.

## Docker & DevOps

89. What is Docker? 
  — Docker packages applications into isolated containers for portability.

90. Docker image vs container? 
  — An image is the blueprint; a container is the running instance.

91. Explain Dockerfile. 
  — It defines how to build a Docker image.

92. What is Docker Compose? 
  — It orchestrates multi-container apps with a single config file.

93. What happens during docker build? 
  — Docker executes each build step and creates cached layers.

94. CI/CD pipeline explanation. 
  — CI runs tests on code changes; CD deploys passing builds automatically.

## System Design Basics

95. Design a URL shortener. 
  — Create short codes, store mappings, and redirect efficiently.

96. Design a chat application. 
  — Use WebSockets, a backend, and persistent storage for messages.

97. How would you scale a REST API? 
  — Scale horizontally, add DB replicas, cache hot data, and use queues.

98. What is caching? 
  — Caching stores frequently used data in fast memory for quick access.

99. Explain load balancing. 
  — It distributes traffic across servers to improve availability and performance.

100. How would you deploy a MERN application? 
  — Build frontend assets, deploy backend containers, and connect to managed databases.
