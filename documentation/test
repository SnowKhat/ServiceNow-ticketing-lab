## Troubleshooting Workflow

```mermaid
flowchart TD
    A[User reports Windows account lockout] --> B[Verify user identity]
    B --> C[Confirm scope of issue]
    C --> D{Can user sign in on another workstation?}

    D -->|No| E[Issue likely tied to enterprise account]
    D -->|Yes| F[Investigate workstation-specific issue]

    E --> G[Check Active Directory account status]
    G --> H{Account active?}

    H -->|No| I[Escalate account status issue]
    H -->|Yes| J[Check password status]

    J --> K{Password expired or account locked?}
    K -->|No| L[Continue troubleshooting authentication issue]
    K -->|Yes| M[Attempt account recovery with registered security PIN]

    M --> N{User remembers PIN?}
    N -->|Yes| O[User completes account recovery]
    N -->|No| P[Reset Windows login password]

    P --> Q[Require password change at next login]
    Q --> R[User signs into workstation]
    R --> S{Access successful?}

    S -->|Yes| T[Verify Outlook and related applications]
    S -->|No| U[Escalate to higher support tier]

    T --> V{Applications working?}
    V -->|Yes| W[Resolve incident]
    V -->|No| X[Investigate cached credentials or application-specific login issue]
```
