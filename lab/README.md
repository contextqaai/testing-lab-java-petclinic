# ContextQA learning lab: Java Spring PetClinic

This is a public educational fork of [spring-projects/spring-petclinic](https://github.com/spring-projects/spring-petclinic). Original source, history, licenses and attribution are retained. It is not a customer production application.

## Status

Source is available. Hosted full-stack sessions and ContextQA reports are not yet verified for this track. The exercises below are a test-design guide, not a passing test report. Upstream starting commit: `500158f732419217507c7656904b8e6aa1bcc0d6`.

## Run locally

Follow the upstream Maven or Gradle instructions and the checked-in build requirements. Use synthetic records. Disable H2 console/development endpoints before public hosting. Isolate each live session database. Do not imply this educational app represents a production clinical system.

See the [upstream setup guide](../README.md#upstream-project-documentation) for the project's original instructions.

## Exercises

| Scenario | Required assertion |
|---|---|
| Owner search | A seeded owner can be found by last name. |
| Owner validation | Invalid required fields prevent saving an owner. |
| Pet association | A new pet appears under the selected owner. |
| Visit association | A visit is recorded against the selected pet. |
| Persistence | Saved values remain visible after navigation and reload. |

## Reproduce the end-to-end workflow

1. Start your own local or hosted copy with synthetic fixtures. ContextQA's cloud runner needs a reachable address; localhost needs a separately supported connection.
2. Choose one scenario and write explicit expected results before generating the test.
3. Follow [ContextQA's getting-started guide](https://contextqa.com/tutorials/getting-started-with-contextqa-test-automation/) or the [MCP documentation](https://mcp.contextqa.com/docs/faq) using your own authenticated workspace.
4. Create/review the test steps, execute, and inspect the actual assertion and runner verdict.
5. Introduce one disclosed regression in a separate local branch. Repeat the same test, observe failure, fix the application and rerun.
6. Record the app commit, fixture/scenario version, browser, tool version, timestamp, step counts and evidence. Do not describe a recording as a fresh run.
7. Repeat on a URL you own or have permission to test. Use synthetic data and confirm actions that submit or alter records.

## Reports and limitations

No ContextQA report is included yet. Add only actual execution evidence. Public reports must contain synthetic data and explicit provenance. Private target results must stay private. Upstream tests remain upstream tests; they are not proof of a ContextQA run.

Recorded reports can be reused for the exact pinned fixture and version. Live runs need fresh isolated state and quotas. Code export, CI integration, automatic resets and embedded execution should be demonstrated only after independently verified.

## Teaching brief

Show the app, source and assertion; create and run the test; inspect evidence; reproduce a regression; show the fix; then test an authorized app of your own. Keep setup and execution time separate. Link the exact release and acknowledge upstream creators. Creator sponsorships should be disclosed.
