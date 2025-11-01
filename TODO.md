# OAuth Authentication Implementation for NewsPulse App

## Backend Implementation

- [ ] Install required dependencies (passport, passport-google-oauth20, passport-github2, jsonwebtoken, mongoose, bcryptjs, express-rate-limit, cookie-parser)
- [ ] Create User mongoose model with schema (provider, providerId, email, name, avatar, preferences, bookmarks, refreshToken, linkedAccounts, timestamps)
- [ ] Set up Passport strategies for Google and GitHub OAuth
- [ ] Create auth middleware (requireAuth) to validate JWT cookie
- [ ] Create auth routes (/auth/google, /auth/google/callback, /auth/github, /auth/github/callback, /auth/me, /auth/logout)
- [ ] Create user routes (/user/preferences GET/POST)
- [ ] Update server.js to integrate auth routes, middleware, and database connection
- [ ] Add rate limiting to auth endpoints
- [ ] Implement error handling and logging

## Frontend Implementation

- [ ] Create AuthProvider context for managing user state
- [ ] Update or create useAuth hook to integrate with AuthProvider
- [ ] Add login buttons (Google and GitHub) to Navbar or Auth page
- [ ] Create ProtectedRoute component for route protection
- [ ] Update Auth page to include OAuth buttons
- [ ] Add user dropdown with logout functionality
- [ ] Handle post-OAuth redirect and session check on app load

## Configuration and Setup

- [ ] Create .env.example with required environment variables
- [ ] Provide step-by-step setup instructions for Google and GitHub OAuth apps
- [ ] Document redirect URIs for local development and production

## Testing and Deployment

- [ ] Test OAuth flows locally (login, logout, session persistence)
- [ ] Provide Postman test steps for backend endpoints
- [ ] Document deployment notes (env vars, cookie settings, security)
- [ ] Add CSRF protection explanation and implementation
- [ ] Include bonus features if time allows (account linking, migration script)

## Security and Best Practices

- [ ] Ensure httpOnly, Secure, SameSite cookies
- [ ] Implement state parameter for CSRF prevention
- [ ] Use PKCE if applicable or server-side flow
- [ ] Store refresh tokens securely in DB
- [ ] Validate all inputs and handle errors gracefully
