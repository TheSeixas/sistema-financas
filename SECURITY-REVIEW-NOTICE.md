# Maintainer review notice

This file is included with the proposed contribution so the security findings are not mistaken for a production certification.

The review identified an authorization-boundary concern around user-owned financial resources. The proposed fixes are intended to make ownership checks explicit.

**Important:** the contributor worked on these changes with the BDK engineering process, but did not run the application locally on their own computer. Please execute the Maven build/tests and application-level integration tests in your environment before merging or deploying.
