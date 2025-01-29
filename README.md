# NextAuth Session Unavailable in API Routes

This repository demonstrates a common issue when using NextAuth.js with API routes: the session object is sometimes unavailable, resulting in a 401 Unauthorized error. This is often due to incorrect configuration or missing dependencies.

## Problem
The provided `bug.js` file showcases an API route that attempts to access the NextAuth session using `unstable_getServerSession`.  However, due to a common oversight (demonstrated in the code), the session is often undefined, leading to the 401 error.

## Solution
The `bugSolution.js` file provides the corrected code. The solution addresses the root cause of the issue, ensuring the session is correctly accessed.