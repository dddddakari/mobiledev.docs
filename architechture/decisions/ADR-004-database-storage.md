# ADR 004: Database Storage

## Status
Accepted

## Subject Area
Data Management

## Topic
MySQL

## Top of Interest
Scalability & Security

## Context
### Issue/Problem
Need reliable, scalable storage with offline access.

### Assumptions
- App requires real-time syncing and backup capabilities.

### Motivations
- MySQL’s widespread support and open-source nature.
- SQLite’s offline capabilities.

### Alternatives Considered
- Firebase
- Realm
- PostgreSQL

## Decision
**Use:**
- **Remote**: MySQL hosted on AWS/Azure.
- **Local**: Encrypted SQLite via `react-native-sqlite-storage`.

## Justification
- Team familiarity with MySQL.
- SQLite encryption ensures local data security.

## Consequences
- **Pros**: Scalable, offline-first support.
- **Cons**: Requires backend API development; adds complexity.
