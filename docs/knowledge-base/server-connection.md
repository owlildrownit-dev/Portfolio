# Application Cannot Connect to the Server

**Demonstration article.** The service on port 3000 and its `/health` endpoint are illustrative. This article is not an installation or troubleshooting reference for either supplied document. Use the actual application endpoint when adapting it.

## Problem

The application cannot reach its backend service.

## Symptoms

- the interface displays a connection error;
- requests remain pending or fail;
- authentication does not complete;
- the browser reports a network or server error.

## Possible causes

- the backend service is stopped;
- the configured server address or port is incorrect;
- a firewall, proxy, or VPN blocks the connection;
- name resolution fails;
- the service is listening only on a local interface.

## Resolution

1. Confirm the configured server URL.
2. Check whether the backend process is running.
3. Request the health endpoint:

    ```bash
    curl -i http://localhost:3000/health
    ```

4. Verify that the expected port is listening.
5. Test name resolution when a hostname is used.
6. Temporarily disconnect an optional proxy or VPN only if organizational policy permits it.
7. Retry the operation.

## Expected result

The health endpoint returns a successful HTTP response and the application completes its request.

## Escalation data

If the issue remains, provide:

- the exact error message;
- the date and time of the failure;
- the application and operating-system versions;
- the configured server URL without credentials or tokens;
- relevant client and server log excerpts with sensitive data removed;
- the steps already completed.
