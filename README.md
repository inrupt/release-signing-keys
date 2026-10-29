# Inrupt release signing keys

Inrupt signs every release of Inrupt Enterprise Solid Server (ESS) software that it distributes through Git. Each release is a Git tag, and each tag carries a signature made with the key in this repository.

## Current key

| | |
| --- | --- |
| Identity | `releases@inrupt.com` |
| Key type | Ed25519 (SSH signature) |
| File | [`inrupt-release-signing-key.pub`](inrupt-release-signing-key.pub) |
| SHA-256 fingerprint | `SHA256:Ov56OjnIOQ41+6SY9CSPvZDgzeIZBgWXqdv8M5B7U7A` |

The reference for this key is <https://www.inrupt.com/security/release-signing-keys>. The address <https://www.inrupt.com/security/inrupt-release-signing-key.pub> serves the file in this repository.

## Check the key before you use it

```bash
ssh-keygen -lf inrupt-release-signing-key.pub
```

The `SHA256:` value it prints must be exactly the fingerprint above and on Inrupt's release signing keys page. If it differs, don't use it, and contact security@inrupt.com.

## Key changes

If Inrupt replaces this key, the new key is published here and on the release signing keys page before it is used, with the date it takes effect. The old key moves to a `retired/` folder, so that older releases can still be checked.

Retired keys: none.

## Contact

security@inrupt.com
