Limiting the number of messages encrypted with the same key version helps prevent brute-force attacks enabled by cryptanalysis. Key lifetime recommendations depend on the key's algorithm, as well as either the number of messages produced, or the total number of bytes encrypted with the same key version. For example, the recommended key lifetime for symmetric keys in Galois/Counter Mode (GCM) is based on the number of messages encrypted, as noted by NIST. If a key is compromised, regular rotation limits the number of actual messages vulnerable to compromise.

### Best Practices

- Implement key rotation/rolling into your architecture to prevent stale and predictable keys with your most critical data. A key rolling algorithm can complicate a reverse engineer's life by ensuring the keys are always changing, this along with PUF based keys will lock down any leaked data.
- Remove any static and developer keys before release.
- All keys required to authenticate to external services should expire on a regular cadence so that any leaked credentials are not valid indefinitely.
- Design in automated credential rotation from the beginning of a project so that the delivered solution can recover from a security breech quickly.
- Create integration checks to see if the key is compromised; if so, disable it and revoke access to it as soon as possible.
- We recommend that you rotate keys automatically on a regular schedule.
