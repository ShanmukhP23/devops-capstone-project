# Customer Accounts Microservice — User Stories

## US-001: Create an Account
**As a** user,
**I want** to create a customer account,
**So that** customer information can be stored in the system.

Acceptance Criteria:
- An account can be created with name, email, address and date joined.
- Phone number is optional.
- The API returns the created account and its identifier.
- Invalid account data is rejected.

## US-002: Read an Account
**As a** user,
**I want** to retrieve an account by its ID,
**So that** I can view the customer's information.

Acceptance Criteria:
- The API returns the account when the ID exists.
- The API returns HTTP 404 when the account does not exist.

## US-003: Update an Account
**As a** user,
**I want** to update an existing account,
**So that** customer information remains accurate.

Acceptance Criteria:
- Existing account fields can be updated.
- The updated account is returned.
- A missing account returns HTTP 404.

## US-004: Delete an Account
**As a** user,
**I want** to delete an account by its ID,
**So that** unwanted customer records can be removed.

Acceptance Criteria:
- An existing account can be deleted.
- Successful deletion returns HTTP 204.
- A missing account returns HTTP 404.

## US-005: List Accounts
**As a** user,
**I want** to retrieve all customer accounts,
**So that** I can view the accounts stored in the system.

Acceptance Criteria:
- The API returns a collection of accounts.
- An empty database returns an empty collection.
