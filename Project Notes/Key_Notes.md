# Key Notes for Development

## General Guidelines
- Always keep the `Project_info.md` file updated with any changes to the project structure, modules, or development phases.
- Refer to the `Templates/` directory for UI components and ensure consistency in design.
- Follow the development phases outlined in `Project_info.md` to maintain structured progress.
- Ensure all code changes are compliant with SOC-2 and SEC requirements.

## Coding Best Practices
- Use CodeIgniter 4 conventions for backend development.
- Maintain strict Role-Based Access Control (RBAC) for all modules.
- Implement Multi-Factor Authentication (MFA) where applicable.
- Ensure encryption for data at rest and in transit.
- Write unit tests for all new features and maintain test coverage.

## Modules to Prioritize
1. **Authentication & Authorization**
   - Role-based access control.
   - Audit logging for sensitive actions.
2. **Investor Profiles**
   - Legal profiles.
   - Share ownership summaries.
3. **Contracts & Agreements**
   - Secure document storage.
   - E-signature integration.
4. **Cap Table Engine**
   - Real-time ownership calculations.
   - Transaction-based updates.

## Database Considerations
- Use PostgreSQL or MySQL as specified.
- Maintain strict permission isolation for database access.
- Key tables to focus on:
  - `users`, `roles`, `permissions`, `activity_logs`
  - `investors`, `share_types`, `investor_shares`
  - `contracts`, `contract_versions`, `contract_signatures`

## Security & Compliance
- Ensure tamper-proof audit logs.
- Regularly test for vulnerabilities.
- Follow best practices for secure coding.

## Future Enhancements
- AI contract review.
- Mobile application development.
- Investor messaging system.

## Planned Features

### Azure AD Integration Module
- Integrate Azure Active Directory for authentication.
- Enable SAML-based authentication for Founder accounts.
- Provide seamless login experience for Azure AD users.
- Ensure secure and scalable authentication mechanisms.

### Admin Settings Page
- Create a dedicated UI for managing application settings.
- Features to include:
  - User role management.
  - Application-wide configurations.
  - Logs and monitoring tools.
  - Integration settings for external services (e.g., Azure AD).
- Ensure secure access restricted to Admin accounts.

### Notifications Module
- Implement a system-wide notifications module.
- Features to include:
  - Real-time notifications for users.
  - Support for different notification types (e.g., alerts, updates).
  - Configurable notification preferences.

### SMTP Emailing Module
- Integrate SMTP for email communication.
- Features to include:
  - Sending transactional emails.
  - Email templates for notifications and updates.
  - Configurable SMTP settings for different environments.

## Roles

### Admin Role
- Dedicated backend account.
- Full access to manage all aspects of the application.

### Founder Role
- Reserved for B4 Manga owners.
- Planned integration with Azure SAML for authentication.

### Stakeholders Role
- Built-in account managed by the application.
- Limited access based on stakeholder-specific permissions.

### Module Documentation
- For every module created, maintain a dedicated Markdown document.
- Document details to include:
  - Module purpose and functionality.
  - Dependencies and connections to other modules.
  - Configuration and setup instructions.
  - API endpoints (if applicable).
  - Any special considerations or limitations.

---

**Note:** Always keep this document updated with new insights, best practices, and changes to the project scope.