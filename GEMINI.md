# Auth0 Gemini CLI Extension

## Overview

This extension connects the Gemini CLI to you Auth0 tenant using the MCP protocol. The MCP server will be started locally once you've intalled the extension.

Prior to using this extension, you must authenticate. This can be done by running !{/auth0:init}. This will open a browser window where you can login, and select a tenant, should you have multiple for you Auth0 account.

## Custom commands

- **/auth0:init**: Initialize the MCP server, and authenticate your Auth0 tenant. This will open a new browser window where you can login, and choose which tenant to connect to.
- **/auth0:session**: Check if there is a valid authentication session available.
- **/auth0:logout**: Logout from the Auth0 MCP server.

## Troubleshooting

Before using the Auth0 MCP server, you need a valid authentication session, you can check if you have an ongoing session by running !{/auth0:session}. If no session is available, run !{/auth0:init}.

IMPORTANT: If the MCP server fails to start or throws an error, make sure there's a valid session using !{/auth0:session}, if there's no session, start one using !{/auth0:init}
