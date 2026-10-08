# Test cases: <feature name>

Ticket: 
Environment: 
Tested by:  · Date: 

## Conventions

- **ID**: area prefix plus number, e.g. `LOGIN-01`
- **Priority**: P1 must pass to ship, P2 should pass, P3 nice to have
- **Status**: ✅ pass · ❌ fail · ⛔ blocked · ➖ not run

## Cases

| ID | Priority | Title | Preconditions | Steps | Expected result | Status | Notes / bug |
|---|---|---|---|---|---|---|---|
| LOGIN-01 | P1 | Valid login | Active user exists | 1. Open /login 2. Enter valid email and password 3. Submit | Lands on dashboard, user name shown in header | | |
| LOGIN-02 | P1 | Wrong password | Active user exists | 1. Open /login 2. Enter valid email, wrong password 3. Submit | "Invalid email or password" shown, stays on /login, no session cookie | | |
| LOGIN-03 | P2 | Locked account | User is locked | 1. Log in with locked user | Locked message shown, no session | | |
| LOGIN-04 | P2 | Empty fields | None | 1. Submit empty form | Both fields marked required, no request sent | | |
| | | | | | | | |

## Edge cases worth a row

- Empty, very long, and unicode input (e.g. `Zoë`, emoji, RTL text)
- Leading/trailing spaces
- Double-submit and back-button after submit
- Slow network and request timeout
- Two tabs, two users, or an expired session
- Permissions: the same action as each role, and logged out
