#
laravel-shopify/
│
├── .github/                     # GitHub-specific files
│   └── copliot-instruction.md   # Instructions for GitHub Copilot
│
├── src/                         # Main package source code
│   ├── Actions/                 # Action classes implementing core functionality
│   │   ├── ActivatePlan.php     # Plan activation logic
│   │   ├── ActivateUsageCharge.php
│   │   ├── AfterAuthorize.php
│   │   ├── AuthenticateShop.php # Authentication logic
│   │   ├── CancelCharge.php
│   │   ├── CreateScripts.php    # ScriptTag creation
│   │   ├── CreateWebhooks.php   # Webhook creation
│   │   ├── DeleteWebhooks.php
│   │   ├── DispatchScripts.php
│   │   ├── DispatchWebhooks.php
│   │   ├── GetPlanUrl.php
│   │   ├── InstallShop.php      # Shop installation
│   │   └── VerifyThemeSupport.php
│   │
│   ├── Console/                 # Console commands
│   │   ├── AddVariablesCommand.php
│   │   ├── WebhookJobMakeCommand.php
│   │   └── stubs/               # Command templates
│   │
│   ├── Contracts/               # Interfaces defining package functionality
│   │   ├── ApiHelper.php
│   │   ├── ShopModel.php        # Shop model interface
│   │   ├── Commands/            # Command interfaces
│   │   ├── Objects/             # Value object interfaces
│   │   └── Queries/             # Query interfaces
│   │
│   ├── Directives/              # Blade directives
│   │   └── SessionToken.php
│   │
│   ├── Exceptions/              # Package-specific exceptions
│   │   ├── ApiException.php
│   │   ├── BaseException.php
│   │   ├── ChargeNotRecurringException.php
│   │   └── ...
│   │
│   ├── Http/                    # HTTP-related components
│   │   ├── Controllers/         # Controller templates
│   │   ├── Middleware/          # Package middleware
│   │   └── Requests/            # Form requests
│   │
│   ├── Macros/                  # Laravel macros
│   │   ├── TokenRedirect.php
│   │   ├── TokenRoute.php
│   │   └── TokenUrl.php
│   │
│   ├── Messaging/               # Event and job handling
│   │   ├── Events/              # Event definitions
│   │   └── Jobs/                # Background jobs
│   │
│   ├── Objects/                 # Value objects
│   │   ├── Enums/               # Enumeration values
│   │   ├── Transfers/           # Transfer objects
│   │   └── Values/              # Value objects
│   │
│   ├── resources/               # Package resources
│   │   ├── config/              # Configuration files
│   │   │   └── shopify-app.php  # Main config
│   │   ├── database/            # Database resources
│   │   │   └── migrations/      # Database migrations
│   │   ├── jobs/                # Job templates
│   │   ├── routes/              # Route definitions
│   │   └── views/               # Blade templates
│   │
│   ├── Services/                # Helper services
│   │   ├── ApiHelper.php        # API communication
│   │   ├── ChargeHelper.php     # Billing helpers
│   │   ├── CookieHelper.php     # Cookie helpers
│   │   └── ThemeHelper.php      # Theme helpers
│   │
│   ├── Storage/                 # Database interactions
│   │   ├── Commands/            # Database write operations
│   │   ├── Models/              # Eloquent models
│   │   │   ├── Charge.php       # Charge model
│   │   │   └── Plan.php         # Plan model
│   │   ├── Observers/           # Model observers
│   │   ├── Queries/             # Database read operations
│   │   └── Scopes/              # Query scopes
│   │
│   ├── Traits/                  # Reusable trait implementations
│   │   ├── ApiController.php
│   │   ├── AuthController.php   # Authentication controller methods
│   │   ├── BillingController.php
│   │   ├── HomeController.php
│   │   ├── ShopAccessible.php
│   │   ├── ShopModel.php        # Shop model