# Phase 02 — Local Angular Environment

## Objective

Validate the local development environment before generating the Angular application.

No application code is created in this phase.

## Required checks

Run these commands in PowerShell or the VS Code terminal:

```powershell
node --version
npm --version
git --version
```

Then check Angular CLI:

```powershell
ng version
```

If `ng` is not recognized, do not install anything yet. Report the exact error so the installation can be performed with versions appropriate to the existing Node.js environment.

## Validation rule

The next phase starts only after the command output has been reviewed.

## Repository workflow

For each development step:

1. Define a small change.
2. Implement only that change.
3. Run the relevant validation.
4. Review the result.
5. Commit the verified state to `main`.
6. Only then continue.

## User assistance

The user will provide local command output, screenshots of errors when necessary, Firebase Console actions, and manual verification of browser behaviour.

Passwords, tokens, API keys, browser cookies and session data must never be committed.
