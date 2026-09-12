# Implementation Notes

## 1. Cloud Run Deployment

-   Deployed the application to Google Cloud Run.
-   Used Cloud Run revisions to manage different application versions.
-   Verified the deployed application through its Cloud Run URL.

## 2. Canary Deployment

-   Created multiple Cloud Run revisions.
-   Initially routed 90% of traffic to the existing revision and 10% to
    the new revision.
-   Used Cloud Run traffic splitting for a controlled canary release.
-   Promoted the new revision to 100% of production traffic after
    validation.

## 3. Event-Driven Processing

-   Configured Eventarc to trigger a Cloud Run service from cloud
    events.
-   Verified that the event reached the Cloud Run service.
-   Used Cloud Run Logs to inspect the incoming event and confirm
    processing.

## 4. Key Concepts

-   Cloud Run revisions
-   Traffic splitting
-   Canary releases
-   Progressive delivery
-   Event-driven architecture
-   Eventarc
-   Cloud Logging
-   Serverless deployment

## 5. Evidence

Screenshots in the repository demonstrate: - Cloud Run service
deployment - 90/10 canary traffic split - 100/0 production traffic
split - Running application - Event processing in Cloud Run logs
