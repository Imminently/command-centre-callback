# Command Centre sign-in return pages

Public pages that hand an online service's sign-in back to Imminently's Command Centre app on the computer that started it.

- `employment-hero/` : Employment Hero accepts only a public HTTPS return address, so it returns here, and this page forwards the one-time `code` and `state` to `http://localhost:4173/api/employment-hero/callback`.

The pages hold no data and no secrets, load nothing from elsewhere, and store nothing. The one-time code is useless without the app's client secret and PKCE verifier, which never leave the computer.
