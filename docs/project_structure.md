# Estructura de Proyecto Base

**Versión:** 1.0  
**Fecha:** 2025-01-13  
**Autor:** [Tu Nombre]  
**Estado:** Activo

---

## 📁 Estructura Completa del Proyecto

```
project-root/
├── 📁 frontend/                    # Aplicación Next.js
│   ├── 📁 public/                  # Assets estáticos
│   │   ├── 📄 favicon.ico
│   │   ├── 📄 robots.txt
│   │   └── 📁 images/
│   ├── 📁 src/
│   │   ├── 📁 app/                 # App Router (Next.js 13+)
│   │   │   ├── 📁 (auth)/          # Route groups
│   │   │   │   ├── 📄 login/
│   │   │   │   └── 📄 register/
│   │   │   ├── 📁 (dashboard)/
│   │   │   │   ├── 📄 dashboard/
│   │   │   │   └── 📄 profile/
│   │   │   ├── 📄 globals.css
│   │   │   ├── 📄 layout.tsx
│   │   │   └── 📄 page.tsx
│   │   ├── 📁 components/          # Componentes reutilizables
│   │   │   ├── 📁 ui/              # Componentes base
│   │   │   │   ├── 📄 Button.tsx
│   │   │   │   ├── 📄 Input.tsx
│   │   │   │   ├── 📄 Card.tsx
│   │   │   │   └── 📄 index.ts
│   │   │   ├── 📁 forms/           # Componentes de formularios
│   │   │   ├── 📁 layout/          # Componentes de layout
│   │   │   └── 📁 features/        # Componentes específicos
│   │   ├── 📁 hooks/               # Custom React hooks
│   │   │   ├── 📄 useAuth.ts
│   │   │   ├── 📄 useApi.ts
│   │   │   └── 📄 useLocalStorage.ts
│   │   ├── 📁 lib/                 # Utilidades y configuraciones
│   │   │   ├── 📄 utils.ts
│   │   │   ├── 📄 constants.ts
│   │   │   └── 📄 api.ts
│   │   ├── 📁 store/               # Estado global
│   │   │   ├── 📄 auth.ts
│   │   │   └── 📄 index.ts
│   │   ├── 📁 types/               # Definiciones de TypeScript
│   │   │   ├── 📄 api.ts
│   │   │   ├── 📄 auth.ts
│   │   │   └── 📄 common.ts
│   │   └── 📁 styles/              # Estilos adicionales
│   │       ├── 📄 components.css
│   │       └── 📄 utilities.css
│   ├── 📁 tests/                   # Tests del frontend
│   │   ├── 📁 __mocks__/
│   │   ├── 📁 components/
│   │   ├── 📁 hooks/
│   │   └── 📁 utils/
│   ├── 📄 .eslintrc.js
│   ├── 📄 .prettierrc
│   ├── 📄 next.config.js
│   ├── 📄 package.json
│   ├── 📄 tailwind.config.js
│   ├── 📄 tsconfig.json
│   └── 📄 README.md
├── 📁 backend/                     # Aplicación FastAPI
│   ├── 📁 app/
│   │   ├── 📁 api/                 # Endpoints de la API
│   │   │   ├── 📁 v1/
│   │   │   │   ├── 📄 auth.py
│   │   │   │   ├── 📄 users.py
│   │   │   │   └── 📄 index.py
│   │   │   └── 📄 deps.py
│   │   ├── 📁 core/                # Configuraciones core
│   │   │   ├── 📄 config.py
│   │   │   ├── 📄 database.py
│   │   │   ├── 📄 security.py
│   │   │   └── 📄 exceptions.py
│   │   ├── 📁 models/              # Modelos de base de datos
│   │   │   ├── 📄 user.py
│   │   │   ├── 📄 base.py
│   │   │   └── 📄 __init__.py
│   │   ├── 📁 schemas/             # Esquemas Pydantic
│   │   │   ├── 📄 user.py
│   │   │   ├── 📄 auth.py
│   │   │   └── 📄 common.py
│   │   ├── 📁 services/            # Lógica de negocio
│   │   │   ├── 📄 auth_service.py
│   │   │   ├── 📄 user_service.py
│   │   │   └── 📄 email_service.py
│   │   ├── 📁 utils/               # Utilidades
│   │   │   ├── 📄 helpers.py
│   │   │   └── 📄 validators.py
│   │   └── 📄 main.py
│   ├── 📁 tests/                   # Tests del backend
│   │   ├── 📁 api/
│   │   ├── 📁 services/
│   │   ├── 📁 conftest.py
│   │   └── 📄 test_main.py
│   ├── 📁 alembic/                 # Migraciones de base de datos
│   │   ├── 📁 versions/
│   │   ├── 📄 env.py
│   │   └── 📄 alembic.ini
│   ├── 📄 .env.example
│   ├── 📄 .flake8
│   ├── 📄 Dockerfile
│   ├── 📄 requirements.txt
│   └── 📄 README.md
├── 📁 docs/                        # Documentación
│   ├── 📄 README.md
│   ├── 📄 API.md
│   ├── 📄 DEPLOYMENT.md
│   ├── 📄 CONTRIBUTING.md
│   └── 📁 diagrams/
├── 📁 docker/                      # Configuración Docker
│   ├── 📄 docker-compose.yml
│   ├── 📄 docker-compose.dev.yml
│   ├── 📄 docker-compose.prod.yml
│   └── 📁 nginx/
├── 📁 scripts/                     # Scripts de automatización
│   ├── 📄 setup.sh
│   ├── 📄 deploy.sh
│   ├── 📄 backup.sh
│   └── 📄 health-check.sh
├── 📁 .github/                     # GitHub Actions
│   └── 📁 workflows/
│       ├── 📄 ci.yml
│       ├── 📄 cd.yml
│       └── 📄 security.yml
├── 📄 .gitignore
├── 📄 .env.example
├── 📄 docker-compose.yml
├── 📄 package.json
└── 📄 README.md
```

---

## 🚀 Configuración Inicial

### 1. Setup del Frontend (Next.js)

```bash
# Crear proyecto Next.js
npx create-next-app@latest frontend --typescript --tailwind --eslint --app --src-dir --import-alias "@/*"

cd frontend

# Instalar dependencias adicionales
npm install @radix-ui/react-icons lucide-react
npm install zustand @tanstack/react-query
npm install axios react-hook-form @hookform/resolvers zod
npm install clsx tailwind-merge

# Dependencias de desarrollo
npm install -D @types/node @types/react @types/react-dom
npm install -D @testing-library/react @testing-library/jest-dom
npm install -D @playwright/test
npm install -D prettier eslint-config-prettier
```

### 2. Setup del Backend (FastAPI)

```bash
# Crear entorno virtual
python -m venv backend
cd backend
source bin/activate  # En Windows: backend\Scripts\activate

# Instalar dependencias
pip install fastapi uvicorn sqlalchemy pydantic
pip install alembic psycopg2-binary redis
pip install python-jose[cryptography] passlib[bcrypt]
pip install python-multipart email-validator
pip install pytest pytest-asyncio httpx

# Crear requirements.txt
pip freeze > requirements.txt
```

### 3. Configuración de Base de Datos

```bash
# Instalar PostgreSQL (Ubuntu/Debian)
sudo apt update
sudo apt install postgresql postgresql-contrib

# Crear base de datos
sudo -u postgres psql
CREATE DATABASE myapp;
CREATE USER myapp_user WITH PASSWORD 'myapp_password';
GRANT ALL PRIVILEGES ON DATABASE myapp TO myapp_user;
\q

# Instalar Redis
sudo apt install redis-server
```

---

## 📝 Archivos de Configuración

### Frontend - next.config.js
```javascript
/** @type {import('next').NextConfig} */
const nextConfig = {
  experimental: {
    appDir: true,
  },
  images: {
    domains: ['localhost', 'your-domain.com'],
  },
  env: {
    NEXT_PUBLIC_API_URL: process.env.NEXT_PUBLIC_API_URL,
  },
  async rewrites() {
    return [
      {
        source: '/api/:path*',
        destination: `${process.env.NEXT_PUBLIC_API_URL}/api/:path*`,
      },
    ];
  },
};

module.exports = nextConfig;
```

### Frontend - tailwind.config.js
```javascript
/** @type {import('tailwindcss').Config} */
module.exports = {
  darkMode: ['class'],
  content: [
    './pages/**/*.{ts,tsx}',
    './components/**/*.{ts,tsx}',
    './app/**/*.{ts,tsx}',
    './src/**/*.{ts,tsx}',
  ],
  theme: {
    container: {
      center: true,
      padding: '2rem',
      screens: {
        '2xl': '1400px',
      },
    },
    extend: {
      colors: {
        border: 'hsl(var(--border))',
        input: 'hsl(var(--input))',
        ring: 'hsl(var(--ring))',
        background: 'hsl(var(--background))',
        foreground: 'hsl(var(--foreground))',
        primary: {
          DEFAULT: 'hsl(var(--primary))',
          foreground: 'hsl(var(--primary-foreground))',
        },
        secondary: {
          DEFAULT: 'hsl(var(--secondary))',
          foreground: 'hsl(var(--secondary-foreground))',
        },
        destructive: {
          DEFAULT: 'hsl(var(--destructive))',
          foreground: 'hsl(var(--destructive-foreground))',
        },
        muted: {
          DEFAULT: 'hsl(var(--muted))',
          foreground: 'hsl(var(--muted-foreground))',
        },
        accent: {
          DEFAULT: 'hsl(var(--accent))',
          foreground: 'hsl(var(--accent-foreground))',
        },
        popover: {
          DEFAULT: 'hsl(var(--popover))',
          foreground: 'hsl(var(--popover-foreground))',
        },
        card: {
          DEFAULT: 'hsl(var(--card))',
          foreground: 'hsl(var(--card-foreground))',
        },
      },
      borderRadius: {
        lg: 'var(--radius)',
        md: 'calc(var(--radius) - 2px)',
        sm: 'calc(var(--radius) - 4px)',
      },
      keyframes: {
        'accordion-down': {
          from: { height: 0 },
          to: { height: 'var(--radix-accordion-content-height)' },
        },
        'accordion-up': {
          from: { height: 'var(--radix-accordion-content-height)' },
          to: { height: 0 },
        },
      },
      animation: {
        'accordion-down': 'accordion-down 0.2s ease-out',
        'accordion-up': 'accordion-up 0.2s ease-out',
      },
    },
  },
  plugins: [require('tailwindcss-animate')],
};
```

### Backend - app/core/config.py
```python
from pydantic_settings import BaseSettings
from typing import Optional
import os

class Settings(BaseSettings):
    # Database
    DATABASE_URL: str = "postgresql://user:password@localhost/myapp"
    
    # Security
    SECRET_KEY: str = "your-secret-key-here"
    ALGORITHM: str = "HS256"
    ACCESS_TOKEN_EXPIRE_MINUTES: int = 30
    
    # CORS
    BACKEND_CORS_ORIGINS: list = ["http://localhost:3000"]
    
    # Email
    SMTP_TLS: bool = True
    SMTP_PORT: Optional[int] = None
    SMTP_HOST: Optional[str] = None
    SMTP_USER: Optional[str] = None
    SMTP_PASSWORD: Optional[str] = None
    EMAILS_FROM_EMAIL: Optional[str] = None
    EMAILS_FROM_NAME: Optional[str] = None
    
    # Redis
    REDIS_URL: str = "redis://localhost:6379"
    
    # Environment
    ENVIRONMENT: str = "development"
    DEBUG: bool = True
    
    class Config:
        env_file = ".env"

settings = Settings()
```

### Docker - docker-compose.yml
```yaml
version: '3.8'

services:
  frontend:
    build: ./frontend
    ports:
      - "3000:3000"
    environment:
      - NEXT_PUBLIC_API_URL=http://localhost:8000
    depends_on:
      - backend
    volumes:
      - ./frontend:/app
      - /app/node_modules
    networks:
      - app-network

  backend:
    build: ./backend
    ports:
      - "8000:8000"
    environment:
      - DATABASE_URL=postgresql://myapp_user:myapp_password@db:5432/myapp
      - REDIS_URL=redis://redis:6379
    depends_on:
      - db
      - redis
    volumes:
      - ./backend:/app
    networks:
      - app-network

  db:
    image: postgres:15
    environment:
      - POSTGRES_DB=myapp
      - POSTGRES_USER=myapp_user
      - POSTGRES_PASSWORD=myapp_password
    volumes:
      - postgres_data:/var/lib/postgresql/data
    ports:
      - "5432:5432"
    networks:
      - app-network

  redis:
    image: redis:7-alpine
    ports:
      - "6379:6379"
    volumes:
      - redis_data:/data
    networks:
      - app-network

  nginx:
    image: nginx:alpine
    ports:
      - "80:80"
      - "443:443"
    volumes:
      - ./docker/nginx/nginx.conf:/etc/nginx/nginx.conf
      - ./docker/nginx/ssl:/etc/nginx/ssl
    depends_on:
      - frontend
      - backend
    networks:
      - app-network

volumes:
  postgres_data:
  redis_data:

networks:
  app-network:
    driver: bridge
```

---

## 🔧 Scripts de Automatización

### Script de Setup - scripts/setup.sh
```bash
#!/bin/bash

echo "🚀 Setting up development environment..."

# Check if Docker is installed
if ! command -v docker &> /dev/null; then
    echo "❌ Docker is not installed. Please install Docker first."
    exit 1
fi

# Check if Docker Compose is installed
if ! command -v docker-compose &> /dev/null; then
    echo "❌ Docker Compose is not installed. Please install Docker Compose first."
    exit 1
fi

# Create .env files if they don't exist
if [ ! -f ".env" ]; then
    echo "📝 Creating .env file..."
    cp .env.example .env
fi

if [ ! -f "frontend/.env.local" ]; then
    echo "📝 Creating frontend .env.local file..."
    cp frontend/.env.example frontend/.env.local
fi

if [ ! -f "backend/.env" ]; then
    echo "📝 Creating backend .env file..."
    cp backend/.env.example backend/.env
fi

# Install frontend dependencies
echo "📦 Installing frontend dependencies..."
cd frontend
npm install
cd ..

# Install backend dependencies
echo "📦 Installing backend dependencies..."
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
cd ..

# Start services
echo "🐳 Starting Docker services..."
docker-compose up -d db redis

# Wait for database to be ready
echo "⏳ Waiting for database to be ready..."
sleep 10

# Run database migrations
echo "🗄️ Running database migrations..."
cd backend
source venv/bin/activate
alembic upgrade head
cd ..

echo "✅ Setup complete! You can now start the development servers:"
echo "  Frontend: npm run dev (in frontend directory)"
echo "  Backend: uvicorn app.main:app --reload (in backend directory)"
echo "  Or use: docker-compose up"
```

### Script de Deploy - scripts/deploy.sh
```bash
#!/bin/bash

set -e

echo "🚀 Starting deployment..."

# Environment variables
ENVIRONMENT=${1:-production}
DOCKER_REGISTRY=${DOCKER_REGISTRY:-"your-registry.com"}
VERSION=${VERSION:-$(git rev-parse --short HEAD)}

echo "📦 Building Docker images..."

# Build frontend
echo "Building frontend image..."
docker build -t $DOCKER_REGISTRY/frontend:$VERSION ./frontend
docker tag $DOCKER_REGISTRY/frontend:$VERSION $DOCKER_REGISTRY/frontend:latest

# Build backend
echo "Building backend image..."
docker build -t $DOCKER_REGISTRY/backend:$VERSION ./backend
docker tag $DOCKER_REGISTRY/backend:$VERSION $DOCKER_REGISTRY/backend:latest

# Push images
echo "📤 Pushing images to registry..."
docker push $DOCKER_REGISTRY/frontend:$VERSION
docker push $DOCKER_REGISTRY/frontend:latest
docker push $DOCKER_REGISTRY/backend:$VERSION
docker push $DOCKER_REGISTRY/backend:latest

# Deploy to environment
echo "🌍 Deploying to $ENVIRONMENT..."
if [ "$ENVIRONMENT" = "production" ]; then
    docker-compose -f docker-compose.prod.yml up -d
else
    docker-compose -f docker-compose.staging.yml up -d
fi

echo "✅ Deployment complete!"
echo "Version: $VERSION"
echo "Environment: $ENVIRONMENT"
```

---

## 🧪 Configuración de Testing

### Frontend - jest.config.js
```javascript
const nextJest = require('next/jest')

const createJestConfig = nextJest({
  // Provide the path to your Next.js app to load next.config.js and .env files
  dir: './',
})

// Add any custom config to be passed to Jest
const customJestConfig = {
  setupFilesAfterEnv: ['<rootDir>/jest.setup.js'],
  moduleNameMapping: {
    '^@/(.*)$': '<rootDir>/src/$1',
  },
  testEnvironment: 'jest-environment-jsdom',
  collectCoverageFrom: [
    'src/**/*.{js,jsx,ts,tsx}',
    '!src/**/*.d.ts',
    '!src/**/*.stories.{js,jsx,ts,tsx}',
  ],
  coverageThreshold: {
    global: {
      branches: 80,
      functions: 80,
      lines: 80,
      statements: 80,
    },
  },
}

// createJestConfig is exported this way to ensure that next/jest can load the Next.js config which is async
module.exports = createJestConfig(customJestConfig)
```

### Backend - pytest.ini
```ini
[tool:pytest]
testpaths = tests
python_files = test_*.py
python_classes = Test*
python_functions = test_*
addopts = 
    --strict-markers
    --strict-config
    --verbose
    --tb=short
    --cov=app
    --cov-report=term-missing
    --cov-report=html
    --cov-fail-under=80
markers =
    unit: Unit tests
    integration: Integration tests
    e2e: End-to-end tests
    slow: Slow running tests
```

---

## 📊 Monitoreo y Logging

### Frontend - lib/analytics.ts
```typescript
// Analytics configuration
export const analytics = {
  track: (event: string, properties?: Record<string, any>) => {
    // Send to analytics service
    console.log('Analytics:', event, properties);
  },
  
  page: (page: string) => {
    analytics.track('page_view', { page });
  },
  
  error: (error: Error, context?: Record<string, any>) => {
    analytics.track('error', { 
      message: error.message, 
      stack: error.stack,
      ...context 
    });
  }
};

// Error boundary
export class ErrorBoundary extends React.Component<
  { children: React.ReactNode },
  { hasError: boolean }
> {
  constructor(props: { children: React.ReactNode }) {
    super(props);
    this.state = { hasError: false };
  }

  static getDerivedStateFromError(error: Error) {
    return { hasError: true };
  }

  componentDidCatch(error: Error, errorInfo: React.ErrorInfo) {
    analytics.error(error, { errorInfo });
  }

  render() {
    if (this.state.hasError) {
      return <h1>Something went wrong.</h1>;
    }

    return this.props.children;
  }
}
```

### Backend - app/core/logging.py
```python
import logging
import sys
from typing import Any, Dict
from loguru import logger

class InterceptHandler(logging.Handler):
    def emit(self, record):
        try:
            level = logger.level(record.levelname).name
        except ValueError:
            level = record.levelno

        frame, depth = logging.currentframe(), 2
        while frame.f_code.co_filename == logging.__file__:
            frame = frame.f_back
            depth += 1

        logger.opt(depth=depth, exception=record.exc_info).log(
            level, record.getMessage()
        )

def setup_logging():
    # Remove default handler
    logger.remove()
    
    # Add console handler
    logger.add(
        sys.stdout,
        format="<green>{time:YYYY-MM-DD HH:mm:ss}</green> | <level>{level: <8}</level> | <cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> - <level>{message}</level>",
        level="INFO"
    )
    
    # Add file handler
    logger.add(
        "logs/app.log",
        rotation="10 MB",
        retention="7 days",
        format="{time:YYYY-MM-DD HH:mm:ss} | {level: <8} | {name}:{function}:{line} - {message}",
        level="DEBUG"
    )
    
    # Intercept standard logging
    logging.basicConfig(handlers=[InterceptHandler()], level=0, force=True)
    
    # Intercept uvicorn logging
    for _log in ["uvicorn", "uvicorn.error", "fastapi"]:
        _logger = logging.getLogger(_log)
        _logger.handlers = [InterceptHandler()]

# Structured logging
def log_event(event: str, data: Dict[str, Any] = None, level: str = "INFO"):
    logger.bind(event=event, data=data or {}).log(level, f"Event: {event}")

def log_error(error: Exception, context: Dict[str, Any] = None):
    logger.bind(error=str(error), context=context or {}).error(f"Error: {error}")
```

---

## 🔒 Configuración de Seguridad

### Frontend - lib/security.ts
```typescript
// Security utilities
export const security = {
  // Sanitize user input
  sanitize: (input: string): string => {
    return input.replace(/[<>]/g, '');
  },
  
  // Validate email
  isValidEmail: (email: string): boolean => {
    const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
    return emailRegex.test(email);
  },
  
  // Generate CSRF token
  generateCSRFToken: (): string => {
    return Math.random().toString(36).substring(2, 15) + 
           Math.random().toString(36).substring(2, 15);
  },
  
  // Store token securely
  storeToken: (token: string): void => {
    localStorage.setItem('auth_token', token);
  },
  
  // Get token securely
  getToken: (): string | null => {
    return localStorage.getItem('auth_token');
  },
  
  // Remove token
  removeToken: (): void => {
    localStorage.removeItem('auth_token');
  }
};

// HTTP client with security headers
export const apiClient = axios.create({
  baseURL: process.env.NEXT_PUBLIC_API_URL,
  headers: {
    'Content-Type': 'application/json',
    'X-Requested-With': 'XMLHttpRequest',
  },
});

// Request interceptor
apiClient.interceptors.request.use((config) => {
  const token = security.getToken();
  if (token) {
    config.headers.Authorization = `Bearer ${token}`;
  }
  return config;
});

// Response interceptor
apiClient.interceptors.response.use(
  (response) => response,
  (error) => {
    if (error.response?.status === 401) {
      security.removeToken();
      window.location.href = '/login';
    }
    return Promise.reject(error);
  }
);
```

### Backend - app/core/security.py
```python
from fastapi import HTTPException, status, Depends
from fastapi.security import HTTPBearer, HTTPAuthorizationCredentials
from jose import JWTError, jwt
from passlib.context import CryptContext
from datetime import datetime, timedelta
from typing import Optional
import secrets

# Password hashing
pwd_context = CryptContext(schemes=["bcrypt"], deprecated="auto")

# JWT configuration
SECRET_KEY = "your-secret-key"
ALGORITHM = "HS256"
ACCESS_TOKEN_EXPIRE_MINUTES = 30

# Security headers middleware
from fastapi.middleware.cors import CORSMiddleware
from fastapi.middleware.trustedhost import TrustedHostMiddleware

def add_security_middleware(app):
    # CORS
    app.add_middleware(
        CORSMiddleware,
        allow_origins=["http://localhost:3000"],
        allow_credentials=True,
        allow_methods=["*"],
        allow_headers=["*"],
    )
    
    # Trusted hosts
    app.add_middleware(
        TrustedHostMiddleware,
        allowed_hosts=["localhost", "127.0.0.1", "your-domain.com"]
    )

# Rate limiting
from slowapi import Limiter, _rate_limit_exceeded_handler
from slowapi.util import get_remote_address
from slowapi.errors import RateLimitExceeded

limiter = Limiter(key_func=get_remote_address)

def setup_rate_limiting(app):
    app.state.limiter = limiter
    app.add_exception_handler(RateLimitExceeded, _rate_limit_exceeded_handler)

# Input validation
import re
from typing import Any

def validate_input(data: Any, max_length: int = 1000) -> bool:
    """Validate and sanitize user input"""
    if isinstance(data, str):
        # Check length
        if len(data) > max_length:
            return False
        
        # Check for dangerous patterns
        dangerous_patterns = [
            r'<script.*?>',
            r'javascript:',
            r'on\w+\s*=',
            r'<iframe.*?>',
        ]
        
        for pattern in dangerous_patterns:
            if re.search(pattern, data, re.IGNORECASE):
                return False
    
    return True

# CSRF protection
def generate_csrf_token() -> str:
    return secrets.token_urlsafe(32)

def validate_csrf_token(token: str, stored_token: str) -> bool:
    return secrets.compare_digest(token, stored_token)
```

---

## 📈 Performance y Optimización

### Frontend - lib/performance.ts
```typescript
// Performance monitoring
export const performance = {
  // Measure page load time
  measurePageLoad: () => {
    if (typeof window !== 'undefined') {
      window.addEventListener('load', () => {
        const loadTime = performance.now();
        analytics.track('page_load_time', { loadTime });
      });
    }
  },
  
  // Lazy load images
  lazyLoadImages: () => {
    const images = document.querySelectorAll('img[data-src]');
    const imageObserver = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          const img = entry.target as HTMLImageElement;
          img.src = img.dataset.src!;
          img.classList.remove('lazy');
          imageObserver.unobserve(img);
        }
      });
    });
    
    images.forEach(img => imageObserver.observe(img));
  },
  
  // Debounce function
  debounce: <T extends (...args: any[]) => any>(
    func: T,
    wait: number
  ): ((...args: Parameters<T>) => void) => {
    let timeout: NodeJS.Timeout;
    return (...args: Parameters<T>) => {
      clearTimeout(timeout);
      timeout = setTimeout(() => func(...args), wait);
    };
  },
  
  // Throttle function
  throttle: <T extends (...args: any[]) => any>(
    func: T,
    limit: number
  ): ((...args: Parameters<T>) => void) => {
    let inThrottle: boolean;
    return (...args: Parameters<T>) => {
      if (!inThrottle) {
        func(...args);
        inThrottle = true;
        setTimeout(() => inThrottle = false, limit);
      }
    };
  }
};

// Service Worker for caching
export const registerServiceWorker = () => {
  if ('serviceWorker' in navigator) {
    navigator.serviceWorker
      .register('/sw.js')
      .then(registration => {
        console.log('SW registered: ', registration);
      })
      .catch(registrationError => {
        console.log('SW registration failed: ', registrationError);
      });
  }
};
```

### Backend - app/core/cache.py
```python
import redis
from typing import Any, Optional
import json
from functools import wraps

# Redis connection
redis_client = redis.Redis(
    host='localhost',
    port=6379,
    db=0,
    decode_responses=True
)

class Cache:
    def __init__(self, redis_client: redis.Redis):
        self.redis = redis_client
    
    def get(self, key: str) -> Optional[Any]:
        """Get value from cache"""
        try:
            value = self.redis.get(key)
            return json.loads(value) if value else None
        except Exception as e:
            logger.error(f"Cache get error: {e}")
            return None
    
    def set(self, key: str, value: Any, expire: int = 3600) -> bool:
        """Set value in cache"""
        try:
            self.redis.setex(key, expire, json.dumps(value))
            return True
        except Exception as e:
            logger.error(f"Cache set error: {e}")
            return False
    
    def delete(self, key: str) -> bool:
        """Delete value from cache"""
        try:
            self.redis.delete(key)
            return True
        except Exception as e:
            logger.error(f"Cache delete error: {e}")
            return False
    
    def clear_pattern(self, pattern: str) -> bool:
        """Clear all keys matching pattern"""
        try:
            keys = self.redis.keys(pattern)
            if keys:
                self.redis.delete(*keys)
            return True
        except Exception as e:
            logger.error(f"Cache clear pattern error: {e}")
            return False

# Cache decorator
def cache_result(expire: int = 3600):
    def decorator(func):
        @wraps(func)
        async def wrapper(*args, **kwargs):
            # Generate cache key
            cache_key = f"{func.__name__}:{hash(str(args) + str(kwargs))}"
            
            # Try to get from cache
            cached_result = cache.get(cache_key)
            if cached_result is not None:
                return cached_result
            
            # Execute function
            result = await func(*args, **kwargs)
            
            # Store in cache
            cache.set(cache_key, result, expire)
            
            return result
        return wrapper
    return decorator

# Initialize cache
cache = Cache(redis_client)
```

---

## ✅ Checklist de Implementación

### Estructura Base
- [ ] Repositorio inicializado con estructura
- [ ] Configuración de Git y .gitignore
- [ ] Archivos de configuración base creados
- [ ] Scripts de setup implementados
- [ ] Documentación README actualizada

### Frontend
- [ ] Next.js configurado con TypeScript
- [ ] Tailwind CSS configurado
- [ ] Componentes base implementados
- [ ] Sistema de routing configurado
- [ ] Estado global configurado (Zustand)
- [ ] Testing setup implementado

### Backend
- [ ] FastAPI configurado
- [ ] Base de datos configurada
- [ ] Autenticación implementada
- [ ] API endpoints creados
- [ ] Testing setup implementado
- [ ] Migraciones configuradas

### DevOps
- [ ] Docker configurado
- [ ] Docker Compose implementado
- [ ] CI/CD pipeline configurado
- [ ] Monitoreo básico implementado
- [ ] Logging configurado

### Seguridad
- [ ] CORS configurado
- [ ] Autenticación JWT implementada
- [ ] Rate limiting configurado
- [ ] Input validation implementada
- [ ] Security headers configurados

### Performance
- [ ] Caching implementado
- [ ] Lazy loading configurado
- [ ] Image optimization implementada
- [ ] Bundle analysis configurado
- [ ] Performance monitoring activo 