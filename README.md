# capability-keychain-text

Atomic authority package for `keychain/text`.

- imports: `#{:keychain-read :keychain-write}`
- effects: `#{:storage-read :secret :storage-write}`
- default policy: `:approval-required`
- provider status: `contract-only`

Importing this package does not grant runtime authority. Tamaki must
request it explicitly and Kototama must admit the sealed envelope.

```sh
clojure -M:test
```
