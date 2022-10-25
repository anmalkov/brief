Grouping Functions by their required privileges helps to erect a virtual wall between segments of your application, which make it difficult for an attacker to proceed if they find a single vulnerability available externally.

### Best Practices

- Isolate access by deploying multiple Functions, each with its own level of access to the underlying data store. Doing this will increase the difficulty of lateral movement if an attacker is able to compromise any single Function in your application.
