# age-keygen

> Generate `age` key pairs.
> See also: `age` for encrypting/decrypting files.
> More information: <https://manned.org/age-keygen>.

- Generate a key pair, save it to an unencrypted file, and print the public key to `stdout`:

`age-keygen {{[-o|--output]}} {{path/to/file}}`

- Convert an identit[y] to a recipient and print the public key to `stdout`:

`age-keygen -y {{path/to/file}}`
