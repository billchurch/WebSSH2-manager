# WebSSH2-manager
Project to create a more full-featured interface for managing hosts and creating user defined favorites. For [WebSSH2](github.com/billchurch/WebSSH2)

The plan is to have two modes of operation.
1. Stateless server. All settings are stored client-side in browser storage with the ability to export/import a JSON to import into other clients/browsers/ what have you.
2. Stateful server. All settings are stored serverside (mongodb?) Settings may still be exported and imported for use in a stateless "server" option.

The initial seed for the servers to publish to the user could be saved as a JSON flat file, these could be "shared". The user can then personalize their view (filter out servers they don't care about and add additional ones).

Should support ssh per-server ciphers, headers, users, and eventually ssh host keys (for better security).

# External Dependencies
## [WebSSH2](github.com/billchurch/WebSSH2)
  - will need to be modified to take post variables from WebSSH2-manager instance (in progress)
  - do we require some sort of association betwene WebSSH2-manager and WebSSH2? Like a shared secret or some sort of certificate based authentication
