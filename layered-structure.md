# Layered Structure

BookCourseShopService
│
├── src
│ ├── BookCourseShopService.Api # Presentation Layer
│ │ - REST API Controllers
│ │ - Middleware (Logging, Error Handling, Auth)
│ │ - API Models / DTOs
│ │
│ ├── BookCourseShopService.Application # Application Layer
│ │ - Business Use Cases (Commands, Queries)
│ │ - Interfaces (Repository, Services)
│ │ - DTOs and Validators
│ │
│ ├── BookCourseShopService.Domain # Domain Layer
│ │ - Core Entities (Book, Course, Order, User)
│ │ - Value Objects and Enums
│ │ - Domain Services & Events
│ │
│ ├── BookCourseShopService.Infrastructure # Infrastructure Layer
│ │ - Data Access (EF Core Repositories)
│ │ - External Services (Payment Gateway, Email)
│ │ - Configuration and Persistence
│ │
│ └── BookCourseShopService.Shared # Shared Kernel
│ - Common Utilities
│ - Constants
│ - Custom Exceptions
│
├── tests
│ ├── Unit Tests
│ └── Integration Tests
