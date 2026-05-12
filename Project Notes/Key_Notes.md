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

---

**Note:** Always keep this document updated with new insights, best practices, and changes to the project scope.