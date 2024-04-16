# weather-station-api

## Worrking example project structure

myproject/
│
├── app/ # Application-specific components
│ ├── api/ # Endpoints and route definitions
│ │ ├── deps.py # Dependency injection scripts
│ │ ├── api_v1/ # Version 1 of the API routes
│ │ │ ├── endpoints/ # Specific routes (e.g., users, items)
│ │ │ └── router.py # Router for API v1
│ │ └── router.py # Global router that includes all version routers
│ ├── core/ # Application configuration and settings
│ │ ├── config.py # Configuration settings
│ │ └── security.py # Security policies (e.g., password hashing)
│ ├── models/ # Database models
│ │ ├── base.py # Base model definitions
│ │ └── item.py # Example model
│ ├── schemas/ # Pydantic schemas for request and response data
│ ├── services/ # Business logic
│ └── main.py # FastAPI application instance
│
├── tests/ # Tests for the application
│ ├── api/ # Tests for the API endpoints
│ ├── models/ # Tests for model logic
│ └── conftest.py # Test configuration and fixtures
│
├── alembic/ # Database migrations
│ └── versions/ # Migration scripts
│
├── .env # Environment-specific variables
├── Dockerfile # Docker configuration file
├── requirements.txt # Project dependencies
└── README.md # Project overview
