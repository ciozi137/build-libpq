# build-libpq
GitHub Workflow to build PostgreSQL libpq.dll

## About
This is a repository for using GitHub actions to build libpq.dll, the PostgresSQL C library. This will build both 32 and 64 bit versions

## Downloads
Pre-built binaries are available on the [Releases](https://github.com/ciozi137/build-libpq/releases) page.

Each release includes:
- `libpq-win32.zip` - 32-bit DLLs
- `libpq-win64.zip` - 64-bit DLLs

### Included files
- `libpq.dll` - PostgreSQL client library
- `libssl-3.dll` / `libssl-3-x64.dll` - OpenSSL SSL library
- `libcrypto-3.dll` / `libcrypto-3-x64.dll` - OpenSSL crypto library

### Naming Convention

Releases are tagged `REL-<postgres version>-<build number>`. For example, `REL-18.1-1`.

## The Workflow

This project is largely based on workflow files from the [psqlODBC GitHub repository](https://github.com/postgresql-interfaces/psqlodbc).

Builds are triggered in three ways
1. manually
2. automatically on any push to `main`
3. pushing a tag beginning with 'REL-*' (see Naming Convention above)

## Contact
[Patrick](https://github.com/ciozi137)
