# ADR 001: Development Framework Selection

## Status
Accepted

## Subject Area
App Foundation

## Topic
React and Ionic

## Top of Interest
Development Process

## Context
### Issue/Problem
We need a framework compatible with Bootstrap, intuitive for the team, and well-supported.

### Assumptions
- The framework will be used for the entire project with no time to switch later.

### Motivations
- Bootstrap compatibility.
- Team familiarity with React.
- Access to Ionic’s pre-built UI components.

### Alternatives Considered
- Cordova
- Framework7
- Native Script

## Decision
**Use Ionic React (webview-based) with Cordova/Capacitor for Android, and Bootstrap for styling.**

## Justification
- The team is already comfortable with React.
- Ionic provides native-like features via webview while aligning with Bootstrap.
- Faster development cycle due to pre-built components.

## Consequences
- **Pros**: Faster development, cross-platform compatibility, team efficiency.
- **Cons**: Potential performance trade-offs compared to native frameworks.
