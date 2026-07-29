# Core Banking Platform — Frontend Applications

The Core Banking Platform frontend repository contains the web and mobile-facing applications used by bank staff, administrators, individual customers, corporate customers, agents, compliance teams, finance teams and other authorised users.

The frontend applications connect to approved backend APIs and provide secure, accessible and responsive interfaces for banking operations.

This project is currently under active development by a volunteer team and is not yet intended for production banking use.

---

## Project objectives

The frontend platform is designed to:

* Provide secure banking interfaces for different user groups
* Support role-based and institution-based access
* Maintain a consistent user experience across applications
* Reuse a shared design system and common components
* Support desktop, tablet and mobile layouts
* Integrate safely with backend banking services
* Handle complex financial workflows clearly
* Provide accessible interfaces
* Support multiple institutions and branding configurations
* Maintain strong performance and reliability
* Support automated testing and continuous delivery

---

## Frontend applications

The mature release of the platform contains eight primary frontend applications.

### 1. Bank Staff Operations Portal

Used by:

* Tellers
* Customer-service officers
* Branch operations staff
* Account officers
* Branch supervisors
* Operations managers

Main capabilities:

* Customer search
* Customer 360-degree view
* Individual onboarding
* Corporate onboarding
* KYC management
* Account opening
* Account maintenance
* Cash deposits
* Cash withdrawals
* Transfers
* Transaction enquiries
* Account restrictions
* Account freeze and unfreeze requests
* Service requests
* Complaints
* Maker-checker approvals
* Branch dashboards
* Operational work queues
* Teller balancing
* Statement generation
* Receipt generation

Recommended framework:

* Next.js
* React
* TypeScript
* Tailwind CSS

---

### 2. System Administration Portal

Used by:

* Platform administrators
* Institution administrators
* Security administrators
* Product administrators
* Operations administrators

Main capabilities:

* Institution configuration
* Branch configuration
* Region configuration
* Currency configuration
* Holiday and working-day configuration
* Product configuration
* Pricing configuration
* Fee configuration
* Limit configuration
* Policy configuration
* Roles and permissions
* User access management
* Workflow configuration
* Approval configuration
* Feature flags
* Country packs
* Integration credentials
* API-client registration
* Branding configuration
* Notification templates
* Audit settings
* Environment settings

Recommended framework:

* Next.js
* React
* TypeScript
* Tailwind CSS

---

### 3. Individual Internet Banking

Used by personal banking customers.

Main capabilities:

* Customer registration
* Login
* Multi-factor authentication
* Account overview
* Available balance
* Ledger balance
* Transaction history
* Internal transfers
* Interbank transfers
* Beneficiary management
* Scheduled transfers
* Bill payments
* Airtime purchase
* Mobile-data purchase
* Electricity payments
* Cable television payments
* Statement download
* Receipt download
* Card controls
* Loan applications
* Savings goals
* Profile management
* Security settings
* Notification preferences
* Support requests
* Secure messaging

Recommended framework:

* Next.js
* React
* TypeScript
* Tailwind CSS

---

### 4. Mobile Banking Application

Used by individual banking customers on mobile devices.

Main capabilities:

* Secure onboarding
* Login
* Biometric authentication
* Device binding
* Multi-factor authentication
* Account overview
* Transaction history
* Internal transfers
* Interbank transfers
* Beneficiary management
* Bill payments
* Airtime and data purchase
* QR payments
* Card controls
* Loan applications
* Savings goals
* Push notifications
* Statement and receipt access
* Profile management
* Security settings
* Secure support
* Session timeout
* Device management

Recommended framework:

* Flutter
* Dart

Target platforms:

* Android
* iOS

---

### 5. Corporate Internet Banking Portal

Used by:

* Corporate administrators
* Corporate payment initiators
* Corporate payment approvers
* Accountants
* Finance managers
* Payroll officers
* Business owners

Main capabilities:

* Corporate account overview
* Multiple company accounts
* Corporate-user management
* Role and mandate management
* Maker-checker payment workflows
* Bulk payments
* Payroll processing
* Payment-file upload
* Payment templates
* Beneficiary management
* Scheduled payments
* Virtual accounts
* Collection accounts
* Cash pooling
* Account sweeping
* Escrow account access
* Statements
* Reconciliation files
* Corporate limits
* API credentials
* Host-to-host configuration
* Approval queues
* Corporate support requests

Recommended framework:

* Next.js
* React
* TypeScript
* Tailwind CSS

---

### 6. Agent Banking Application

Used by:

* Banking agents
* Field officers
* Microfinance officers
* Agency supervisors

Main capabilities:

* Agent login
* Device binding
* Customer registration
* Customer verification
* Cash deposits
* Cash withdrawals
* Transfers
* Bill payments
* Airtime and data purchase
* Loan collections
* Loan disbursement support
* Agent float
* Agent commissions
* Transaction receipts
* Customer transaction history
* Offline transaction queue
* Background synchronisation
* Agent support
* Device and terminal status
* Daily activity summary

Recommended framework:

* Flutter
* Dart

The application should support unreliable network conditions and controlled offline operation.

---

### 7. Risk, Compliance and Fraud Portal

Used by:

* Compliance officers
* AML analysts
* Fraud analysts
* Risk officers
* Investigation teams
* Security teams

Main capabilities:

* Fraud alert dashboard
* AML alert dashboard
* Alert prioritisation
* Case assignment
* Customer risk profile
* Transaction investigation
* Sanctions screening
* PEP screening
* Watchlist screening
* Watchlist management
* Device-risk information
* Login-risk information
* Case notes
* Evidence upload
* Approval workflows
* Suspicious-activity review
* Regulatory reporting
* Model performance monitoring
* False-positive analysis
* Audit trail access

Recommended framework:

* Next.js
* React
* TypeScript
* Tailwind CSS

---

### 8. Finance, Reconciliation and Reporting Portal

Used by:

* Finance officers
* Reconciliation officers
* Settlement officers
* Accountants
* Auditors
* Management teams
* Regulatory reporting teams

Main capabilities:

* General-ledger reports
* Trial balance
* Profit-and-loss reports
* Balance-sheet reports
* Settlement dashboard
* Reconciliation workbench
* Suspense-account management
* Unmatched-entry investigation
* Nostro reconciliation
* Provider reconciliation
* Financial-close controls
* Regulatory reports
* Management reports
* Scheduled reports
* Audit-trail search
* Executive dashboards
* Report export
* Exception queues
* Period-end approval

Recommended framework:

* Next.js
* React
* TypeScript
* Tailwind CSS

---

## Recommended technology stack

### Web applications

Recommended stack:

* Next.js
* React
* TypeScript
* Tailwind CSS
* React Hook Form
* Zod
* TanStack Query
* TanStack Table
* Playwright
* Jest or Vitest
* Storybook
* OpenAPI-generated clients
* ESLint
* Prettier

### Mobile applications

Recommended stack:

* Flutter
* Dart
* Riverpod, Bloc or another approved state-management solution
* Dio or another approved HTTP client
* Secure storage
* Biometric authentication libraries
* Push-notification libraries
* Flutter integration tests
* Widget tests

### Design and collaboration

Recommended tools:

* Figma
* FigJam
* GitHub
* Storybook
* GitHub Issues
* GitHub Projects

---

## Suggested repository structure

```text
frontend/
├── apps/
│   ├── staff-operations-portal/
│   ├── admin-portal/
│   ├── internet-banking/
│   ├── corporate-banking/
│   ├── risk-compliance-portal/
│   └── finance-reporting-portal/
│
├── mobile/
│   ├── customer-banking-app/
│   └── agent-banking-app/
│
├── packages/
│   ├── ui/
│   ├── design-tokens/
│   ├── api-client/
│   ├── authentication/
│   ├── permissions/
│   ├── forms/
│   ├── tables/
│   ├── charts/
│   ├── validation/
│   ├── utilities/
│   ├── types/
│   └── testing/
│
├── docs/
│   ├── architecture/
│   ├── design-system/
│   ├── accessibility/
│   ├── authentication/
│   ├── permissions/
│   ├── testing/
│   └── deployment/
│
├── scripts/
├── .github/
├── CONTRIBUTING.md
├── CODE_OF_CONDUCT.md
├── SECURITY.md
├── LICENSE
└── README.md
```

The exact structure may change as the project architecture develops.

---

## Shared design system

All frontend applications should use a shared design system where practical.

The design system should include:

* Colours
* Typography
* Spacing
* Breakpoints
* Shadows
* Border radii
* Icons
* Buttons
* Inputs
* Select fields
* Checkboxes
* Radio buttons
* Date fields
* Currency fields
* Search fields
* Data tables
* Pagination
* Tabs
* Navigation
* Sidebars
* Dialogs
* Drawers
* Alerts
* Toast notifications
* Cards
* Charts
* Status badges
* Loading indicators
* Empty states
* Error states
* Permission-restricted states
* Transaction summaries
* Approval components
* Confirmation screens

Components should support:

* Default state
* Hover state
* Focus state
* Active state
* Disabled state
* Loading state
* Error state
* Success state

---

## Design principles

The frontend should be:

* Clear
* Consistent
* Secure
* Accessible
* Responsive
* Easy to navigate
* Suitable for financial operations
* Efficient for frequent staff use
* Understandable to non-technical customers
* Reliable under slow network conditions

Banking interfaces should prioritise clarity over decoration.

Important financial information should be easy to locate and difficult to misunderstand.

---

## UI/UX requirements

Every feature should include the required user states.

Designs should cover:

* Default state
* Loading state
* Empty state
* Error state
* Success state
* Disabled state
* Restricted-access state
* Session-expired state
* Network-failure state
* Confirmation state
* Review state
* Completed state

Forms should include:

* Labels
* Instructions
* Validation messages
* Required-field indicators
* Error summaries
* Confirmation steps
* Accessible focus behaviour

High-risk transactions should include a clear review and confirmation stage.

---

## Responsive design

Web applications should support:

* Desktop
* Laptop
* Tablet
* Mobile web

The staff, administration, compliance and finance portals should be optimised primarily for desktop and laptop use.

Internet banking should support desktop, tablet and mobile browsers.

Avoid layouts that require unnecessary horizontal scrolling.

Large data tables should provide responsive alternatives where practical.

---

## Accessibility

Frontend applications should aim to meet WCAG 2.1 AA or a later approved accessibility standard.

Requirements include:

* Keyboard navigation
* Visible focus indicators
* Proper form labels
* Semantic HTML
* Screen-reader support
* Sufficient colour contrast
* Accessible error messages
* Accessible dialogs
* Accessible data tables
* Descriptive button labels
* Alternative text for meaningful images
* Reduced-motion support where applicable
* Logical heading structure

Colour should not be the only way status or meaning is communicated.

---

## Authentication

Frontend applications may support:

* Username and password
* Multi-factor authentication
* One-time passwords
* Biometric authentication
* Trusted-device registration
* Session timeout
* Refresh tokens
* Device management
* Password reset
* Account lockout
* Suspicious-login verification

Authentication should be implemented using approved identity services.

Frontend applications must not implement their own insecure token systems.

---

## Authorisation and permissions

Every application must respect role-based permissions.

Examples include:

* Customer
* Teller
* Branch supervisor
* Operations officer
* Compliance officer
* Fraud analyst
* Finance officer
* Auditor
* System administrator
* Corporate initiator
* Corporate approver
* Agent
* Relationship manager

The frontend may hide or disable unavailable actions, but backend services must always enforce permissions independently.

Frontend permission checks are for user experience, not final security enforcement.

---

## API integration

Frontend applications should communicate with backend services through approved APIs.

Use:

* Generated API clients where possible
* Shared request types
* Shared response types
* Consistent error handling
* Correlation IDs
* Retry rules
* Request cancellation
* Safe timeout handling

Frontend applications must never connect directly to backend databases.

Do not expose internal service credentials in client-side code.

---

## API error handling

Applications should handle errors such as:

* Validation errors
* Authentication errors
* Authorisation errors
* Network errors
* Timeouts
* Service unavailability
* Duplicate requests
* Insufficient balance
* Transaction-limit errors
* Account restrictions
* Provider failures
* Session expiration

Error messages should be useful without exposing sensitive technical details.

Do not display:

* Stack traces
* Database errors
* Internal service names
* Credentials
* Tokens
* Secret values

---

## Transaction user experience

Financial transactions should use a clear sequence.

Recommended flow:

1. Enter transaction details.
2. Validate input.
3. Display fees and charges.
4. Show available balance where permitted.
5. Present a review screen.
6. Request authentication or approval.
7. Submit the transaction once.
8. Show processing state.
9. Display the result.
10. Provide a transaction reference.
11. Provide a downloadable or shareable receipt where permitted.

The user interface must prevent accidental duplicate submissions.

Submit buttons should be disabled while a transaction is being processed.

---

## Financial display rules

Applications should:

* Display currency clearly
* Use consistent decimal places
* Separate thousands appropriately
* Distinguish available balance from ledger balance
* Show debit and credit information clearly
* Show fees before confirmation
* Show transaction status
* Show transaction references
* Show posting date and transaction date where required
* Avoid misleading rounded figures

Never perform authoritative financial calculations only in the browser.

The backend remains the source of truth for balances, fees, interest and transaction results.

---

## Forms and validation

Recommended tools:

* React Hook Form
* Zod
* Approved shared validators

Forms should:

* Validate required fields
* Validate field formats
* Display clear messages
* Prevent invalid submission
* Preserve safe values after recoverable errors
* Clear sensitive fields where appropriate
* Prevent repeated submission
* Support keyboard navigation
* Support screen readers

Frontend validation improves usability.

Backend validation remains mandatory.

---

## State management

Use the simplest approved state-management approach that meets the application’s needs.

Recommended categories:

* Server state: TanStack Query
* Form state: React Hook Form
* Local component state: React state
* Shared application state: approved lightweight store
* Authentication state: shared authentication package
* Permissions: shared permission package

Avoid placing all state in one global store.

Avoid duplicating backend server state unnecessarily.

---

## Data tables

Banking applications often require complex data tables.

Tables may support:

* Pagination
* Search
* Filtering
* Sorting
* Column visibility
* Export
* Row selection
* Bulk actions
* Status indicators
* Date ranges
* Saved filters

Large datasets should use server-side pagination and filtering.

Do not load unlimited transaction records into the browser.

---

## Dashboard guidelines

Dashboards should show information relevant to the user’s role.

Examples include:

* Assigned tasks
* Pending approvals
* Failed transactions
* Open cases
* Reconciliation exceptions
* Teller position
* Agent float
* Fraud alerts
* AML alerts
* Settlement status
* Loan delinquency
* System health

Avoid overcrowded dashboards.

Users should be able to move from a summary to the underlying details.

---

## Security requirements

Frontend security is the responsibility of every contributor.

Do not store sensitive information unnecessarily.

Never commit:

* Passwords
* API keys
* Access tokens
* Refresh tokens
* Private certificates
* Production endpoints containing secrets
* Real customer data

Use secure storage for sensitive mobile data.

Avoid storing sensitive information in:

* Local storage
* Session storage
* Browser logs
* Analytics tools
* Error messages
* URLs
* Query strings

Protect against:

* Cross-site scripting
* Cross-site request forgery
* Clickjacking
* Open redirects
* Insecure token storage
* Session fixation
* Sensitive data exposure
* Dependency vulnerabilities

---

## Logging and analytics

Frontend logs should not contain:

* Passwords
* One-time passwords
* Full card numbers
* CVVs
* Full BVNs
* Full NINs
* Access tokens
* Refresh tokens
* Private account information
* Real customer documents

Analytics should not capture sensitive financial or identity information.

Use correlation IDs to help trace errors safely.

---

## Environment variables

Provide safe example files such as:

```text
.env.example
```

Example:

```env
NEXT_PUBLIC_APP_NAME=Core Banking Platform
NEXT_PUBLIC_API_BASE_URL=http://localhost:5000
NEXT_PUBLIC_IDENTITY_URL=http://localhost:8080
NEXT_PUBLIC_ENVIRONMENT=development
```

Do not place secrets in variables exposed to the browser.

In Next.js, values prefixed with `NEXT_PUBLIC_` are available to client-side code.

Only public configuration should use that prefix.

---

## Local development requirements

Recommended tools:

* Git
* Node.js
* npm, pnpm or yarn
* Flutter SDK
* Dart SDK
* Android Studio
* Xcode for iOS development
* Visual Studio Code or another IDE
* Docker, where required
* Figma access

Recommended versions:

```text
Node.js: current supported LTS
TypeScript: current approved version
Next.js: current approved stable version
Flutter: current approved stable version
Dart: version bundled with Flutter
```

Use the versions defined by the repository configuration.

---

## Installing dependencies

For a pnpm workspace:

```bash
pnpm install
```

For npm:

```bash
npm install
```

For Flutter applications:

```bash
flutter pub get
```

Do not switch package managers without approval.

Commit the correct lock file.

---

## Running web applications locally

Example:

```bash
pnpm dev
```

To run a specific application in a workspace:

```bash
pnpm --filter staff-operations-portal dev
```

Example development URLs may include:

```text
http://localhost:3000
http://localhost:3001
http://localhost:3002
```

Actual ports should be documented in each application README.

---

## Running Flutter applications locally

Check the Flutter environment:

```bash
flutter doctor
```

List connected devices:

```bash
flutter devices
```

Run the application:

```bash
flutter run
```

Run using a specific environment:

```bash
flutter run --dart-define=APP_ENVIRONMENT=development
```

Each mobile application should provide its own setup instructions.

---

## Code quality

Frontend contributors should:

* Use TypeScript strictly
* Avoid unnecessary use of `any`
* Follow the repository linting rules
* Use shared components
* Use meaningful component names
* Keep components focused
* Separate presentation from business logic
* Avoid duplicated API calls
* Handle loading and error states
* Write tests for critical flows
* Remove debugging code
* Document complex behaviour
* Keep pull requests focused

Use the configured formatter and linter before submitting work.

---

## Component guidelines

Components should:

* Have a clear purpose
* Be reusable where appropriate
* Accept typed properties
* Handle accessibility
* Avoid unnecessary internal state
* Support loading and disabled states
* Avoid hidden side effects
* Be documented when shared

Shared components should be added only when they are genuinely reusable.

Do not place application-specific business logic inside the shared UI package.

---

## Naming conventions

Recommended React component naming:

```text
CustomerSearch.tsx
AccountSummary.tsx
TransferReview.tsx
ApprovalQueue.tsx
TransactionTable.tsx
```

Recommended hook naming:

```text
useCustomer.ts
usePermissions.ts
useTransferForm.ts
useTransactionStatus.ts
```

Recommended utility naming:

```text
formatCurrency.ts
formatAccountNumber.ts
mapApiError.ts
validateTransactionReference.ts
```

Use names that describe business purpose rather than appearance alone.

---

## Testing strategy

Frontend applications should include the following testing layers.

### Unit tests

Used for:

* Utility functions
* Validators
* Formatters
* Hooks
* Permission checks
* State transitions

### Component tests

Used for:

* Forms
* Tables
* Dialogs
* Navigation
* Transaction summaries
* Error states
* Loading states

### Integration tests

Used for:

* API integration
* Authentication flows
* Permission behaviour
* Form submission
* Multi-step workflows

### End-to-end tests

Used for critical journeys such as:

* Customer login
* Customer onboarding
* Account opening
* Internal transfer
* Interbank transfer
* Bill payment
* Corporate payment approval
* Agent cash deposit
* Fraud-case review
* Reconciliation exception handling

### Accessibility tests

Used for:

* Keyboard navigation
* Form labels
* Focus management
* Colour contrast
* Screen-reader behaviour
* Dialog accessibility

### Visual regression tests

May be used for:

* Shared components
* Key banking pages
* Responsive layouts
* Design-system changes

---

## Required transaction test scenarios

Transaction interfaces should test:

* Successful submission
* Invalid input
* Insufficient balance
* Limit exceeded
* Restricted account
* Duplicate submission
* Provider timeout
* Network interruption
* Session expiration
* Authorisation failure
* Retry
* Reversal result
* Partial failure
* Unknown processing status
* Successful receipt generation

---

## Performance

Frontend performance should be monitored.

Consider:

* Bundle size
* Code splitting
* Lazy loading
* Image optimisation
* API caching
* Request deduplication
* Pagination
* Virtualised tables
* Route-level loading
* Server rendering
* Client rendering
* Mobile network conditions

Do not load large reports or transaction histories into memory unnecessarily.

---

## Browser support

The supported browser list should be defined by the project.

Expected support may include recent versions of:

* Google Chrome
* Microsoft Edge
* Mozilla Firefox
* Safari

Internet banking should be tested on common desktop and mobile browsers.

Internal staff applications may use a more restricted supported-browser policy.

---

## Mobile support

The mobile team should define supported versions of:

* Android
* iOS

Testing should cover:

* Small screens
* Large screens
* Low-memory devices
* Slow networks
* Offline conditions
* App backgrounding
* Session expiration
* Device rotation where supported
* Biometric failures
* Notification permissions

---

## Internationalisation

The platform should be prepared for multiple institutions and countries.

Applications may need to support:

* Multiple languages
* Multiple currencies
* Date formats
* Time zones
* Number formats
* Right-to-left layouts
* Country-specific terminology
* Institution-specific branding

Avoid hard-coding institution names, currencies and country-specific values.

---

## Branding and multi-tenancy

The frontend may support institution-specific:

* Logos
* Colours
* Typography
* Product names
* Contact information
* Legal text
* Support channels
* Feature availability

Branding configuration should come from an approved configuration service where practical.

Avoid creating separate codebases for every institution.

---

## Deployment

Web applications may be deployed using:

* Docker
* Kubernetes
* Nginx
* Cloud application platforms
* Static and server-rendered hosting

Mobile applications may be distributed through:

* Google Play
* Apple App Store
* Approved enterprise distribution channels

Environment promotion may include:

* Development
* Test
* Staging
* User acceptance testing
* Production
* Disaster recovery

---

## CI/CD

Frontend pipelines may include:

* Dependency installation
* Formatting checks
* Linting
* Type checking
* Unit tests
* Component tests
* End-to-end tests
* Accessibility checks
* Build
* Dependency scanning
* Security scanning
* Container build
* Deployment
* Smoke testing

Pull requests should not be merged when required checks fail.

---

## Branching convention

Do not commit directly to `main`.

Recommended branch formats:

```text
feature/TASK-0301-customer-dashboard
fix/TASK-0302-transfer-confirmation
design/TASK-0303-corporate-payment-flow
test/TASK-0304-internet-banking-login
refactor/TASK-0305-shared-table-component
docs/TASK-0306-frontend-setup
```

---

## Commit convention

Recommended format:

```text
type: short description
```

Examples:

```text
feat: add customer account dashboard
fix: prevent duplicate transfer submission
test: add corporate approval flow tests
docs: document frontend environment variables
refactor: simplify transaction table filters
style: align form spacing with design system
```

---

## Pull request requirements

Every pull request should include:

* Related Issue or task
* Summary
* Screens or modules changed
* Testing performed
* Screenshots
* Mobile screenshots where applicable
* Responsive behaviour
* Accessibility considerations
* API dependencies
* Known limitations
* Security considerations

Visual changes should include before-and-after screenshots where useful.

---

## Definition of done

A frontend task is complete only when:

* The approved design has been implemented
* Acceptance criteria are satisfied
* The interface is responsive
* Loading states are implemented
* Error states are implemented
* Empty states are implemented
* Permission rules are implemented
* Forms are validated
* API integration is complete
* Relevant tests pass
* Accessibility has been reviewed
* Security concerns have been addressed
* Documentation is updated
* The pull request has been reviewed
* The task tracker has been updated
* The change has been merged

---

## Contribution guide

Read `CONTRIBUTING.md` before starting work.

Contributors must follow:

* Task assignment rules
* Branching rules
* Commit conventions
* Pull-request requirements
* Design-system standards
* Accessibility requirements
* Security requirements
* Testing requirements
* Documentation standards
* Code of Conduct

---

## Volunteer participation

This is currently an unpaid volunteer project.

Participation does not create an employment relationship or guarantee future payment.

Contributors participate to:

* Learn
* Gain practical experience
* Build portfolio evidence
* Collaborate with others
* Understand financial applications
* Contribute to an open-source banking platform

Contributors should communicate honestly about availability, progress and blockers.

---

## Licence

This project is distributed under the licence included in the `LICENSE` file.

Unless otherwise agreed in writing, contributions submitted to this repository will be licensed under the same licence.

Do not submit proprietary designs, source code, assets or components without permission.

---

## Disclaimer

This project is under development and is provided for learning, research and engineering collaboration.

It must not be used for real banking operations, customer funds or sensitive financial information without:

* Security assessment
* Legal review
* Regulatory review
* Accessibility review
* Performance testing
* Penetration testing
* Production-readiness approval
* Disaster-recovery validation

---

## Getting help

Use the approved project communication channels for:

* Onboarding
* Design questions
* Task assignment
* API questions
* Architecture discussions
* Progress updates
* Blockers
* Security concerns
* Accessibility questions

When requesting help, include:

* Application name
* Task ID
* Page or component
* Expected behaviour
* Actual behaviour
* Screenshot where safe
* Error message
* Browser or device
* Steps already attempted

Do not share passwords, tokens or sensitive customer information when requesting help.

---

## Acknowledgements

Thank you to every volunteer contributing frontend development, mobile development, UI/UX design, testing, documentation and engineering effort to the Core Banking Platform.
