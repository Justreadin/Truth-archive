# Production deployment checklist

## Before deployment
- [ ] Choose Render, Railway, or another Docker-capable host.
- [ ] Push this project to a Git repository.
- [ ] Confirm the start command uses the platform-provided `PORT`.
- [ ] Confirm `/api/health` returns HTTP 200.
- [ ] Verify email, Substack, GitHub and Payla destinations in the contact compass.

## Deploy
- [ ] Create a Docker web service from the repository.
- [ ] Deploy without provisioning a database.
- [ ] Attach `favourakintoye.com` and configure DNS as instructed by the host.
- [ ] Enable HTTPS and redirect HTTP to HTTPS if the host does not do so automatically.

## Verify on the live domain
- [ ] Homepage loads.
- [ ] CSS and JavaScript assets load without 404s.
- [ ] `/api/health` returns a healthy response.
- [ ] Test instruments, navigation, modals, and responsive layouts on desktop and mobile.
- [ ] Test each contact destination.
- [ ] Check browser console and server logs for errors.
