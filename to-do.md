# DOJO - Build Checklist

## ✅ Done
- [x] Colour palette
- [x] Icon set
- [x] Login screen
- [x] Badge assets

## Pages to build
- [x] Log In
- [ ] Sign Up
- [ ] Forgot/Reset Password
- [ ] Dashboard / Today's Tasks
- [ ] Task List (templates + custom)
- [ ] Task Detail
- [ ] New Custom Task (Groq decomposition flow)
- [ ] Step Execution
- [ ] Photo Capture (camera view)
- [ ] Verification Result
- [ ] Progress / Streaks & Badges screen
- [ ] Level-up / Milestone screen
- [ ] Profile / Settings
- [ ] History/Logs (optional)

## Small assets still needed
- [ ] App icon / favicon
- [ ] Splash screen
- [ ] Empty-state illustrations (no tasks, no custom tasks)
- [ ] Loading spinner (Groq wait, verification wait)
- [ ] Error states (camera permission denied, offline/API failure)
- [ ] Locked-badge treatment (grayscale filter over existing badge SVGs)
- [ ] Notification icon (if doing push reminders)

## Suggested build order
1. Dashboard
2. Task List / Task Detail
3. Step Execution (no camera)
4. Progress screen
5. Photo Capture
6. Verification Result
7. New Custom Task (Groq decomposition - last, since it's the most complex integration)
