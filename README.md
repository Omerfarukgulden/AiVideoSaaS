# AiVideoSaaS
📁 ai-video-saas-platform/
│
├── 📁 frontend/                                # Next.js 15 + TypeScript
│   │
│   ├── 📁 src/
│   │
│   ├── 📁 app/
│   │   ├── 📁 (public)                         # Landing, Blog, Pricing
│   │   │   ├── page.tsx
│   │   │   ├── pricing/
│   │   │   └── blog/
│   │   │
│   │   ├── 📁 (auth)
│   │   │   ├── login/
│   │   │   ├── register/
│   │   │   ├── forgot-password/
│   │   │   └── verify-email/
│   │   │
│   │   ├── 📁 (dashboard)
│   │   │   ├── layout.tsx
│   │   │   ├── page.tsx
│   │   │   ├── profile/
│   │   │   ├── billing/
│   │   │   ├── history/
│   │   │   ├── face-swap/
│   │   │   ├── talking-photo/
│   │   │   └── text-to-video/
│   │   │
│   │   ├── 📁 api/
│   │   │   └── proxy/
│   │   │
│   │   ├── layout.tsx
│   │   └── page.tsx
│   │
│   ├── 📁 components/
│   │   ├── ui/
│   │   ├── shared/
│   │   └── features/
│   │       ├── auth/
│   │       ├── billing/
│   │       ├── profile/
│   │       ├── face-swap/
│   │       ├── talking-photo/
│   │       └── text-to-video/
│   │
│   ├── 📁 hooks/
│   │   ├── useAuth.ts
│   │   ├── useCredits.ts
│   │   ├── useSignalR.ts
│   │   └── useUpload.ts
│   │
│   ├── 📁 services/
│   │   ├── auth.service.ts
│   │   ├── billing.service.ts
│   │   ├── video.service.ts
│   │   └── user.service.ts
│   │
│   ├── 📁 lib/
│   │   ├── axios.ts
│   │   ├── queryClient.ts
│   │   └── utils.ts
│   │
│   ├── 📁 context/
│   │   ├── AuthContext.tsx
│   │   └── SignalRContext.tsx
│   │
│   ├── 📁 schemas/
│   │
│   ├── 📁 types/
│   │
│   ├── 📁 constants/
│   │
│   └── 📁 styles/
│
├── 📁 backend/
│
│   ├── 📁 SASS.WebApi/
│   │
│   │   ├── Controllers/
│   │   │   ├── AuthController.cs
│   │   │   ├── UserController.cs
│   │   │   ├── BillingController.cs
│   │   │   ├── CreditController.cs
│   │   │   ├── VideoController.cs
│   │   │   └── WebhookController.cs
│   │
│   │   ├── Hubs/
│   │   │   └── NotificationHub.cs
│   │
│   │   ├── Middlewares/
│   │   │   ├── ExceptionHandlingMiddleware.cs
│   │   │   ├── RequestLoggingMiddleware.cs
│   │   │   ├── CorrelationIdMiddleware.cs
│   │   │   ├── SecurityHeadersMiddleware.cs
│   │   │   └── PerformanceMiddleware.cs
│   │
│   │   ├── Extensions/
│   │   │   ├── ServiceCollectionExtensions.cs
│   │   │   └── ApplicationBuilderExtensions.cs
│   │
│   │   ├── Filters/
│   │   │
│   │   ├── Program.cs
│   │   └── appsettings.json
│
│   ├── 📁 SASS.Application/
│   │
│   │   ├── Common/
│   │   │   ├── Interfaces/
│   │   │   ├── Behaviors/
│   │   │   ├── Exceptions/
│   │   │   └── Mapping/
│   │
│   │   ├── Features/
│   │   │
│   │   ├── Auth/
│   │   │   ├── Commands/
│   │   │   ├── Queries/
│   │   │   ├── Validators/
│   │   │   └── DTOs/
│   │   │
│   │   ├── Users/
│   │   │
│   │   ├── Credits/
│   │   │
│   │   ├── Billing/
│   │   │
│   │   ├── Notifications/
│   │   │
│   │   └── VideoJobs/
│   │       ├── Commands/
│   │       ├── Queries/
│   │       ├── Validators/
│   │       └── DTOs/
│
│   ├── 📁 SASS.Domain/
│   │
│   │   ├── Entities/
│   │   │   ├── User.cs
│   │   │   ├── VideoJob.cs
│   │   │   ├── CreditTransaction.cs
│   │   │   └── RefreshToken.cs
│   │
│   │   ├── Enums/
│   │
│   │   ├── Events/
│   │
│   │   ├── ValueObjects/
│   │
│   │   ├── Specifications/
│   │
│   │   └── Exceptions/
│
│   ├── 📁 SASS.Infrastructure/
│   │
│   │   ├── Persistence/
│   │   │   ├── Configurations/
│   │   │   ├── Migrations/
│   │   │   ├── Seed/
│   │   │   └── ApplicationDbContext.cs
│   │
│   │   ├── Authentication/
│   │
│   │   ├── AI/
│   │   │   ├── Providers/
│   │   │   │   ├── ReplicateProvider.cs
│   │   │   │   ├── FalProvider.cs
│   │   │   │   ├── KlingProvider.cs
│   │   │   │   └── RunwayProvider.cs
│   │   │   │
│   │   │   ├── Factory/
│   │   │   │   └── AiProviderFactory.cs
│   │   │   │
│   │   │   └── Models/
│   │
│   │   ├── Storage/
│   │   │   └── CloudflareR2StorageService.cs
│   │
│   │   ├── Payments/
│   │   │   ├── StripeService.cs
│   │   │   └── IyzicoService.cs
│   │
│   │   ├── Cache/
│   │   │   └── RedisCacheService.cs
│   │
│   │   ├── SignalR/
│   │
│   │   ├── Logging/
│   │
│   │   └── BackgroundJobs/
│   │       ├── VideoStatusCheckerJob.cs
│   │       └── CreditRefundJob.cs
│
│   └── 📁 Tests/
│       ├── UnitTests/
│       └── IntegrationTests/
│
├── 📁 deployment/
│   ├── nginx/
│   ├── docker/
│   ├── kubernetes/
│   └── github-actions/
│
├── 📁 docs/
│   ├── api.md
│   ├── architecture.md
│   └── database.md
│
├── docker-compose.yml
├── .env
├── .env.example
├── README.md
└── .gitignore
