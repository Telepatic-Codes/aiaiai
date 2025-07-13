# UI/UX Guidelines

**Versión:** 1.0  
**Fecha:** 2025-01-13  
**Autor:** [Tu Nombre]  
**Estado:** Activo

---

## 🎨 Propósito

Este documento establece las guías de diseño, patrones de interfaz y principios de experiencia de usuario para mantener consistencia y calidad en toda la aplicación.

---

## 🎯 Principios de Diseño

### 1. User-Centered Design
- **Empatía**: Entender las necesidades reales del usuario
- **Iteración**: Diseño basado en feedback continuo
- **Accesibilidad**: Inclusivo para todos los usuarios
- **Simplicidad**: Menos es más

### 2. Consistencia Visual
- **Sistema de diseño**: Componentes reutilizables
- **Jerarquía clara**: Información organizada por importancia
- **Patrones familiares**: Interfaces que los usuarios conocen
- **Branding coherente**: Identidad visual consistente

### 3. Performance y Usabilidad
- **Carga rápida**: Tiempo de respuesta < 2 segundos
- **Feedback inmediato**: Confirmación de acciones
- **Navegación intuitiva**: Encontrar información fácilmente
- **Error prevention**: Prevenir errores antes de que ocurran

---

## 🎨 Design System

### Paleta de Colores

#### Colores Primarios
```css
:root {
  /* Primary Colors */
  --primary-50: #eff6ff;
  --primary-100: #dbeafe;
  --primary-200: #bfdbfe;
  --primary-300: #93c5fd;
  --primary-400: #60a5fa;
  --primary-500: #3b82f6;
  --primary-600: #2563eb;
  --primary-700: #1d4ed8;
  --primary-800: #1e40af;
  --primary-900: #1e3a8a;
  --primary-950: #172554;
}
```

#### Colores Semánticos
```css
:root {
  /* Success */
  --success-50: #f0fdf4;
  --success-500: #22c55e;
  --success-600: #16a34a;
  --success-700: #15803d;

  /* Warning */
  --warning-50: #fffbeb;
  --warning-500: #f59e0b;
  --warning-600: #d97706;
  --warning-700: #b45309;

  /* Error */
  --error-50: #fef2f2;
  --error-500: #ef4444;
  --error-600: #dc2626;
  --error-700: #b91c1c;

  /* Info */
  --info-50: #eff6ff;
  --info-500: #3b82f6;
  --info-600: #2563eb;
  --info-700: #1d4ed8;
}
```

#### Colores Neutros
```css
:root {
  /* Neutral Colors */
  --neutral-50: #fafafa;
  --neutral-100: #f5f5f5;
  --neutral-200: #e5e5e5;
  --neutral-300: #d4d4d4;
  --neutral-400: #a3a3a3;
  --neutral-500: #737373;
  --neutral-600: #525252;
  --neutral-700: #404040;
  --neutral-800: #262626;
  --neutral-900: #171717;
  --neutral-950: #0a0a0a;
}
```

### Tipografía

#### Jerarquía de Texto
```css
:root {
  /* Font Sizes */
  --text-xs: 0.75rem;    /* 12px */
  --text-sm: 0.875rem;   /* 14px */
  --text-base: 1rem;     /* 16px */
  --text-lg: 1.125rem;   /* 18px */
  --text-xl: 1.25rem;    /* 20px */
  --text-2xl: 1.5rem;    /* 24px */
  --text-3xl: 1.875rem;  /* 30px */
  --text-4xl: 2.25rem;   /* 36px */
  --text-5xl: 3rem;      /* 48px */
  --text-6xl: 3.75rem;   /* 60px */

  /* Font Weights */
  --font-light: 300;
  --font-normal: 400;
  --font-medium: 500;
  --font-semibold: 600;
  --font-bold: 700;
  --font-extrabold: 800;
}
```

#### Clases de Tipografía
```css
/* Headings */
.heading-1 {
  font-size: var(--text-4xl);
  font-weight: var(--font-bold);
  line-height: 1.2;
  letter-spacing: -0.025em;
}

.heading-2 {
  font-size: var(--text-3xl);
  font-weight: var(--font-semibold);
  line-height: 1.3;
}

.heading-3 {
  font-size: var(--text-2xl);
  font-weight: var(--font-semibold);
  line-height: 1.4;
}

/* Body Text */
.body-large {
  font-size: var(--text-lg);
  font-weight: var(--font-normal);
  line-height: 1.6;
}

.body-medium {
  font-size: var(--text-base);
  font-weight: var(--font-normal);
  line-height: 1.5;
}

.body-small {
  font-size: var(--text-sm);
  font-weight: var(--font-normal);
  line-height: 1.4;
}

/* Caption */
.caption {
  font-size: var(--text-xs);
  font-weight: var(--font-medium);
  line-height: 1.3;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}
```

### Espaciado

#### Sistema de Espaciado
```css
:root {
  /* Spacing Scale */
  --space-0: 0;
  --space-1: 0.25rem;   /* 4px */
  --space-2: 0.5rem;    /* 8px */
  --space-3: 0.75rem;   /* 12px */
  --space-4: 1rem;      /* 16px */
  --space-5: 1.25rem;   /* 20px */
  --space-6: 1.5rem;    /* 24px */
  --space-8: 2rem;      /* 32px */
  --space-10: 2.5rem;   /* 40px */
  --space-12: 3rem;     /* 48px */
  --space-16: 4rem;     /* 64px */
  --space-20: 5rem;     /* 80px */
  --space-24: 6rem;     /* 96px */
  --space-32: 8rem;     /* 128px */
}
```

### Sombras y Elevación

#### Sistema de Sombras
```css
:root {
  /* Shadow System */
  --shadow-sm: 0 1px 2px 0 rgb(0 0 0 / 0.05);
  --shadow-base: 0 1px 3px 0 rgb(0 0 0 / 0.1), 0 1px 2px -1px rgb(0 0 0 / 0.1);
  --shadow-md: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);
  --shadow-lg: 0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1);
  --shadow-xl: 0 20px 25px -5px rgb(0 0 0 / 0.1), 0 8px 10px -6px rgb(0 0 0 / 0.1);
  --shadow-2xl: 0 25px 50px -12px rgb(0 0 0 / 0.25);
}
```

---

## 🧩 Componentes Base

### Botones

#### Variantes de Botón
```typescript
// components/ui/Button.tsx
interface ButtonProps {
  variant?: 'primary' | 'secondary' | 'outline' | 'ghost' | 'destructive';
  size?: 'sm' | 'md' | 'lg';
  disabled?: boolean;
  loading?: boolean;
  children: React.ReactNode;
  onClick?: () => void;
}

const Button: React.FC<ButtonProps> = ({
  variant = 'primary',
  size = 'md',
  disabled = false,
  loading = false,
  children,
  onClick
}) => {
  const baseClasses = 'inline-flex items-center justify-center rounded-md font-medium transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:opacity-50 disabled:pointer-events-none';
  
  const variantClasses = {
    primary: 'bg-primary text-primary-foreground hover:bg-primary/90',
    secondary: 'bg-secondary text-secondary-foreground hover:bg-secondary/80',
    outline: 'border border-input bg-background hover:bg-accent hover:text-accent-foreground',
    ghost: 'hover:bg-accent hover:text-accent-foreground',
    destructive: 'bg-destructive text-destructive-foreground hover:bg-destructive/90'
  };
  
  const sizeClasses = {
    sm: 'h-9 px-3 text-sm',
    md: 'h-10 px-4 py-2',
    lg: 'h-11 px-8'
  };

  return (
    <button
      className={`${baseClasses} ${variantClasses[variant]} ${sizeClasses[size]}`}
      disabled={disabled || loading}
      onClick={onClick}
    >
      {loading && <Spinner className="mr-2 h-4 w-4" />}
      {children}
    </button>
  );
};
```

#### Uso de Botones
```typescript
// Ejemplos de uso
<Button variant="primary" size="md">
  Guardar Cambios
</Button>

<Button variant="outline" size="sm">
  Cancelar
</Button>

<Button variant="destructive" loading>
  Eliminar
</Button>
```

### Inputs

#### Componente Input
```typescript
// components/ui/Input.tsx
interface InputProps {
  type?: 'text' | 'email' | 'password' | 'number' | 'tel' | 'url';
  placeholder?: string;
  value?: string;
  onChange?: (value: string) => void;
  error?: string;
  disabled?: boolean;
  required?: boolean;
  label?: string;
  helperText?: string;
}

const Input: React.FC<InputProps> = ({
  type = 'text',
  placeholder,
  value,
  onChange,
  error,
  disabled = false,
  required = false,
  label,
  helperText
}) => {
  return (
    <div className="space-y-2">
      {label && (
        <label className="text-sm font-medium leading-none peer-disabled:cursor-not-allowed peer-disabled:opacity-70">
          {label}
          {required && <span className="text-destructive">*</span>}
        </label>
      )}
      
      <input
        type={type}
        className={`flex h-10 w-full rounded-md border border-input bg-background px-3 py-2 text-sm ring-offset-background file:border-0 file:bg-transparent file:text-sm file:font-medium placeholder:text-muted-foreground focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:cursor-not-allowed disabled:opacity-50 ${
          error ? 'border-destructive' : ''
        }`}
        placeholder={placeholder}
        value={value}
        onChange={(e) => onChange?.(e.target.value)}
        disabled={disabled}
        required={required}
      />
      
      {error && (
        <p className="text-sm text-destructive">{error}</p>
      )}
      
      {helperText && !error && (
        <p className="text-sm text-muted-foreground">{helperText}</p>
      )}
    </div>
  );
};
```

### Cards

#### Componente Card
```typescript
// components/ui/Card.tsx
interface CardProps {
  children: React.ReactNode;
  className?: string;
  padding?: 'sm' | 'md' | 'lg';
  shadow?: 'sm' | 'md' | 'lg';
}

const Card: React.FC<CardProps> = ({
  children,
  className = '',
  padding = 'md',
  shadow = 'md'
}) => {
  const paddingClasses = {
    sm: 'p-4',
    md: 'p-6',
    lg: 'p-8'
  };
  
  const shadowClasses = {
    sm: 'shadow-sm',
    md: 'shadow-md',
    lg: 'shadow-lg'
  };

  return (
    <div className={`bg-card text-card-foreground rounded-lg border ${paddingClasses[padding]} ${shadowClasses[shadow]} ${className}`}>
      {children}
    </div>
  );
};

// Subcomponentes
const CardHeader: React.FC<{ children: React.ReactNode }> = ({ children }) => (
  <div className="flex flex-col space-y-1.5 pb-4">
    {children}
  </div>
);

const CardTitle: React.FC<{ children: React.ReactNode }> = ({ children }) => (
  <h3 className="text-2xl font-semibold leading-none tracking-tight">
    {children}
  </h3>
);

const CardDescription: React.FC<{ children: React.ReactNode }> = ({ children }) => (
  <p className="text-sm text-muted-foreground">
    {children}
  </p>
);

const CardContent: React.FC<{ children: React.ReactNode }> = ({ children }) => (
  <div className="pt-0">
    {children}
  </div>
);

const CardFooter: React.FC<{ children: React.ReactNode }> = ({ children }) => (
  <div className="flex items-center pt-4">
    {children}
  </div>
);
```

---

## 📱 Patrones de Interfaz

### Layouts

#### Layout Principal
```typescript
// components/layout/MainLayout.tsx
interface MainLayoutProps {
  children: React.ReactNode;
  sidebar?: React.ReactNode;
  header?: React.ReactNode;
}

const MainLayout: React.FC<MainLayoutProps> = ({
  children,
  sidebar,
  header
}) => {
  return (
    <div className="min-h-screen bg-background">
      {header && (
        <header className="sticky top-0 z-50 w-full border-b bg-background/95 backdrop-blur supports-[backdrop-filter]:bg-background/60">
          {header}
        </header>
      )}
      
      <div className="flex">
        {sidebar && (
          <aside className="w-64 border-r bg-background">
            {sidebar}
          </aside>
        )}
        
        <main className="flex-1">
          {children}
        </main>
      </div>
    </div>
  );
};
```

#### Grid System
```css
/* Grid Classes */
.grid {
  display: grid;
}

.grid-cols-1 { grid-template-columns: repeat(1, minmax(0, 1fr)); }
.grid-cols-2 { grid-template-columns: repeat(2, minmax(0, 1fr)); }
.grid-cols-3 { grid-template-columns: repeat(3, minmax(0, 1fr)); }
.grid-cols-4 { grid-template-columns: repeat(4, minmax(0, 1fr)); }
.grid-cols-6 { grid-template-columns: repeat(6, minmax(0, 1fr)); }
.grid-cols-12 { grid-template-columns: repeat(12, minmax(0, 1fr)); }

.gap-1 { gap: var(--space-1); }
.gap-2 { gap: var(--space-2); }
.gap-3 { gap: var(--space-3); }
.gap-4 { gap: var(--space-4); }
.gap-6 { gap: var(--space-6); }
.gap-8 { gap: var(--space-8); }
```

### Navegación

#### Navigation Menu
```typescript
// components/navigation/Navigation.tsx
interface NavigationItem {
  label: string;
  href: string;
  icon?: React.ReactNode;
  children?: NavigationItem[];
}

interface NavigationProps {
  items: NavigationItem[];
  orientation?: 'horizontal' | 'vertical';
}

const Navigation: React.FC<NavigationProps> = ({
  items,
  orientation = 'horizontal'
}) => {
  return (
    <nav className={orientation === 'vertical' ? 'space-y-2' : 'flex space-x-4'}>
      {items.map((item) => (
        <NavigationItem key={item.href} item={item} />
      ))}
    </nav>
  );
};

const NavigationItem: React.FC<{ item: NavigationItem }> = ({ item }) => {
  const [isOpen, setIsOpen] = useState(false);
  
  return (
    <div className="relative">
      <Link
        href={item.href}
        className="flex items-center px-3 py-2 text-sm font-medium rounded-md hover:bg-accent hover:text-accent-foreground"
      >
        {item.icon && <span className="mr-2">{item.icon}</span>}
        {item.label}
        {item.children && (
          <ChevronDown className="ml-auto h-4 w-4" />
        )}
      </Link>
      
      {item.children && isOpen && (
        <div className="absolute left-0 mt-2 w-48 rounded-md shadow-lg bg-background border">
          {item.children.map((child) => (
            <Link
              key={child.href}
              href={child.href}
              className="block px-4 py-2 text-sm hover:bg-accent"
            >
              {child.label}
            </Link>
          ))}
        </div>
      )}
    </div>
  );
};
```

### Formularios

#### Form Layout
```typescript
// components/forms/FormLayout.tsx
interface FormLayoutProps {
  children: React.ReactNode;
  title?: string;
  description?: string;
  onSubmit?: (data: any) => void;
  submitLabel?: string;
  loading?: boolean;
}

const FormLayout: React.FC<FormLayoutProps> = ({
  children,
  title,
  description,
  onSubmit,
  submitLabel = 'Guardar',
  loading = false
}) => {
  return (
    <form onSubmit={onSubmit} className="space-y-6">
      {(title || description) && (
        <div className="space-y-2">
          {title && <h2 className="text-2xl font-semibold">{title}</h2>}
          {description && <p className="text-muted-foreground">{description}</p>}
        </div>
      )}
      
      <div className="space-y-4">
        {children}
      </div>
      
      {onSubmit && (
        <div className="flex justify-end space-x-2">
          <Button type="submit" loading={loading}>
            {submitLabel}
          </Button>
        </div>
      )}
    </form>
  );
};
```

---

## ♿ Accesibilidad

### Principios de Accesibilidad

#### 1. Perceptible
- **Contraste de color**: Mínimo 4.5:1 para texto normal
- **Tamaño de texto**: Mínimo 16px para texto del cuerpo
- **Alternativas de texto**: Alt text para imágenes
- **Subtítulos**: Para contenido multimedia

#### 2. Operable
- **Navegación por teclado**: Todas las funciones accesibles
- **Tiempo suficiente**: No límites de tiempo estrictos
- **No parpadeo**: Evitar contenido que parpadee
- **Navegación clara**: Breadcrumbs y estructura lógica

#### 3. Comprensible
- **Lenguaje claro**: Texto legible y comprensible
- **Consistencia**: Patrones de navegación consistentes
- **Prevención de errores**: Validación y confirmación
- **Ayuda contextual**: Instrucciones y etiquetas claras

#### 4. Robusto
- **Compatibilidad**: Funciona con tecnologías asistivas
- **Marcado válido**: HTML semántico correcto
- **Fallbacks**: Alternativas para funcionalidades

### Implementación

#### ARIA Labels
```typescript
// Ejemplos de ARIA
<button aria-label="Cerrar modal">
  <X className="h-4 w-4" />
</button>

<div role="alert" aria-live="polite">
  {errorMessage}
</div>

<nav aria-label="Navegación principal">
  <Navigation items={navItems} />
</nav>
```

#### Focus Management
```typescript
// hooks/useFocusTrap.ts
import { useEffect, useRef } from 'react';

export const useFocusTrap = (isActive: boolean) => {
  const containerRef = useRef<HTMLDivElement>(null);

  useEffect(() => {
    if (!isActive || !containerRef.current) return;

    const container = containerRef.current;
    const focusableElements = container.querySelectorAll(
      'button, [href], input, select, textarea, [tabindex]:not([tabindex="-1"])'
    );

    const firstElement = focusableElements[0] as HTMLElement;
    const lastElement = focusableElements[focusableElements.length - 1] as HTMLElement;

    const handleKeyDown = (e: KeyboardEvent) => {
      if (e.key === 'Tab') {
        if (e.shiftKey) {
          if (document.activeElement === firstElement) {
            e.preventDefault();
            lastElement.focus();
          }
        } else {
          if (document.activeElement === lastElement) {
            e.preventDefault();
            firstElement.focus();
          }
        }
      }
    };

    container.addEventListener('keydown', handleKeyDown);
    firstElement?.focus();

    return () => {
      container.removeEventListener('keydown', handleKeyDown);
    };
  }, [isActive]);

  return containerRef;
};
```

---

## 📱 Responsive Design

### Breakpoints
```css
/* Breakpoints */
:root {
  --breakpoint-sm: 640px;
  --breakpoint-md: 768px;
  --breakpoint-lg: 1024px;
  --breakpoint-xl: 1280px;
  --breakpoint-2xl: 1536px;
}

/* Responsive Classes */
.sm\:block { display: block; }
.md\:flex { display: flex; }
.lg\:grid { display: grid; }

.sm\:text-sm { font-size: var(--text-sm); }
.md\:text-base { font-size: var(--text-base); }
.lg\:text-lg { font-size: var(--text-lg); }

.sm\:p-4 { padding: var(--space-4); }
.md\:p-6 { padding: var(--space-6); }
.lg\:p-8 { padding: var(--space-8); }
```

### Mobile-First Approach
```typescript
// components/layout/ResponsiveLayout.tsx
const ResponsiveLayout: React.FC<{ children: React.ReactNode }> = ({ children }) => {
  return (
    <div className="
      w-full
      px-4 sm:px-6 lg:px-8
      py-4 sm:py-6 lg:py-8
      max-w-7xl mx-auto
    ">
      <div className="
        grid
        grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4
        gap-4 sm:gap-6 lg:gap-8
      ">
        {children}
      </div>
    </div>
  );
};
```

---

## 🎭 Estados de Interfaz

### Loading States
```typescript
// components/ui/LoadingState.tsx
interface LoadingStateProps {
  size?: 'sm' | 'md' | 'lg';
  text?: string;
}

const LoadingState: React.FC<LoadingStateProps> = ({
  size = 'md',
  text = 'Cargando...'
}) => {
  const sizeClasses = {
    sm: 'h-4 w-4',
    md: 'h-8 w-8',
    lg: 'h-12 w-12'
  };

  return (
    <div className="flex items-center justify-center space-x-2">
      <div className={`animate-spin rounded-full border-2 border-primary border-t-transparent ${sizeClasses[size]}`} />
      <span className="text-sm text-muted-foreground">{text}</span>
    </div>
  );
};
```

### Empty States
```typescript
// components/ui/EmptyState.tsx
interface EmptyStateProps {
  icon?: React.ReactNode;
  title: string;
  description: string;
  action?: React.ReactNode;
}

const EmptyState: React.FC<EmptyStateProps> = ({
  icon,
  title,
  description,
  action
}) => {
  return (
    <div className="flex flex-col items-center justify-center py-12 text-center">
      {icon && (
        <div className="mb-4 text-muted-foreground">
          {icon}
        </div>
      )}
      
      <h3 className="text-lg font-semibold mb-2">{title}</h3>
      <p className="text-muted-foreground mb-4 max-w-sm">{description}</p>
      
      {action && action}
    </div>
  );
};
```

### Error States
```typescript
// components/ui/ErrorState.tsx
interface ErrorStateProps {
  title?: string;
  message: string;
  retry?: () => void;
}

const ErrorState: React.FC<ErrorStateProps> = ({
  title = 'Algo salió mal',
  message,
  retry
}) => {
  return (
    <div className="flex flex-col items-center justify-center py-12 text-center">
      <AlertCircle className="h-12 w-12 text-destructive mb-4" />
      
      <h3 className="text-lg font-semibold mb-2">{title}</h3>
      <p className="text-muted-foreground mb-4 max-w-sm">{message}</p>
      
      {retry && (
        <Button onClick={retry} variant="outline">
          Intentar de nuevo
        </Button>
      )}
    </div>
  );
};
```

---

## 🎨 Animaciones y Transiciones

### Transiciones Suaves
```css
/* Transitions */
.transition-all {
  transition: all 0.2s ease-in-out;
}

.transition-colors {
  transition: color 0.2s ease-in-out, background-color 0.2s ease-in-out, border-color 0.2s ease-in-out;
}

.transition-transform {
  transition: transform 0.2s ease-in-out;
}

.transition-opacity {
  transition: opacity 0.2s ease-in-out;
}

/* Animations */
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

@keyframes slideIn {
  from { transform: translateY(20px); opacity: 0; }
  to { transform: translateY(0); opacity: 1; }
}

@keyframes scaleIn {
  from { transform: scale(0.95); opacity: 0; }
  to { transform: scale(1); opacity: 1; }
}

.animate-fade-in {
  animation: fadeIn 0.3s ease-out;
}

.animate-slide-in {
  animation: slideIn 0.3s ease-out;
}

.animate-scale-in {
  animation: scaleIn 0.2s ease-out;
}
```

### Micro-interacciones
```typescript
// hooks/useHover.ts
import { useState } from 'react';

export const useHover = () => {
  const [isHovered, setIsHovered] = useState(false);

  const bind = {
    onMouseEnter: () => setIsHovered(true),
    onMouseLeave: () => setIsHovered(false),
  };

  return [isHovered, bind];
};

// Uso en componentes
const InteractiveCard: React.FC<{ children: React.ReactNode }> = ({ children }) => {
  const [isHovered, bind] = useHover();

  return (
    <div
      {...bind}
      className={`
        transition-all duration-200 ease-in-out
        ${isHovered ? 'scale-105 shadow-lg' : 'scale-100 shadow-md'}
      `}
    >
      {children}
    </div>
  );
};
```

---

## 📊 Data Visualization

### Gráficos Simples
```typescript
// components/charts/SimpleChart.tsx
interface ChartData {
  label: string;
  value: number;
  color?: string;
}

interface SimpleChartProps {
  data: ChartData[];
  type: 'bar' | 'line' | 'pie';
  height?: number;
}

const SimpleChart: React.FC<SimpleChartProps> = ({
  data,
  type,
  height = 200
}) => {
  const maxValue = Math.max(...data.map(d => d.value));
  
  return (
    <div className="w-full" style={{ height }}>
      {type === 'bar' && (
        <div className="flex items-end space-x-2 h-full">
          {data.map((item, index) => (
            <div
              key={index}
              className="flex-1 bg-primary rounded-t"
              style={{
                height: `${(item.value / maxValue) * 100}%`,
                backgroundColor: item.color
              }}
              title={`${item.label}: ${item.value}`}
            />
          ))}
        </div>
      )}
      
      {type === 'line' && (
        <svg className="w-full h-full" viewBox={`0 0 100 ${height}`}>
          <polyline
            fill="none"
            stroke="currentColor"
            strokeWidth="2"
            points={data.map((item, index) => 
              `${(index / (data.length - 1)) * 100},${100 - (item.value / maxValue) * 100}`
            ).join(' ')}
          />
        </svg>
      )}
    </div>
  );
};
```

---

## 🧪 Testing de UI

### Component Testing
```typescript
// __tests__/components/Button.test.tsx
import { render, screen, fireEvent } from '@testing-library/react';
import { Button } from '@/components/ui/Button';

describe('Button Component', () => {
  it('renders with correct text', () => {
    render(<Button>Click me</Button>);
    expect(screen.getByRole('button', { name: /click me/i })).toBeInTheDocument();
  });

  it('handles click events', () => {
    const handleClick = jest.fn();
    render(<Button onClick={handleClick}>Click me</Button>);
    
    fireEvent.click(screen.getByRole('button'));
    expect(handleClick).toHaveBeenCalledTimes(1);
  });

  it('applies variant classes correctly', () => {
    render(<Button variant="destructive">Delete</Button>);
    const button = screen.getByRole('button');
    expect(button).toHaveClass('bg-destructive');
  });

  it('shows loading state', () => {
    render(<Button loading>Loading</Button>);
    expect(screen.getByRole('button')).toBeDisabled();
    expect(screen.getByText('Loading')).toBeInTheDocument();
  });
});
```

### Visual Regression Testing
```typescript
// __tests__/visual/Button.visual.test.ts
import { test, expect } from '@playwright/test';

test.describe('Button Visual Tests', () => {
  test('primary button matches snapshot', async ({ page }) => {
    await page.goto('/test/button-primary');
    await expect(page.locator('[data-testid="primary-button"]')).toHaveScreenshot('primary-button.png');
  });

  test('all button variants render correctly', async ({ page }) => {
    await page.goto('/test/button-variants');
    await expect(page.locator('[data-testid="button-container"]')).toHaveScreenshot('button-variants.png');
  });
});
```

---

## 📚 Recursos y Referencias

### Herramientas de Diseño
- **Figma**: Diseño y prototipado
- **Storybook**: Documentación de componentes
- **Chromatic**: Visual regression testing
- **Framer**: Prototipado avanzado

### Bibliotecas de Componentes
- **shadcn/ui**: Componentes base
- **Radix UI**: Primitivos accesibles
- **Headless UI**: Componentes sin estilos
- **React Hook Form**: Manejo de formularios

### Guías de Accesibilidad
- [WCAG 2.1 Guidelines](https://www.w3.org/WAI/WCAG21/quickref/)
- [ARIA Authoring Practices](https://www.w3.org/WAI/ARIA/apg/)
- [Web Accessibility Initiative](https://www.w3.org/WAI/)

### Herramientas de Testing
- **Jest**: Testing unitario
- **React Testing Library**: Testing de componentes
- **Playwright**: Testing E2E
- **Percy**: Visual regression testing

---

## ✅ Checklist de Implementación

### Design System
- [ ] Paleta de colores definida
- [ ] Tipografía establecida
- [ ] Sistema de espaciado implementado
- [ ] Componentes base creados
- [ ] Documentación en Storybook

### Accesibilidad
- [ ] Contraste de colores verificado
- [ ] Navegación por teclado implementada
- [ ] ARIA labels agregados
- [ ] Screen reader testing completado
- [ ] WCAG 2.1 AA compliance

### Responsive Design
- [ ] Mobile-first approach implementado
- [ ] Breakpoints definidos
- [ ] Touch targets apropiados
- [ ] Performance optimizada
- [ ] Cross-browser testing

### Testing
- [ ] Component testing implementado
- [ ] Visual regression testing configurado
- [ ] Accessibility testing automatizado
- [ ] Performance testing establecido
- [ ] User testing completado 