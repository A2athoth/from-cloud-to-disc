# Verification

The file `meta/SHA256SUMS` records SHA-256 checksums for repository files.

To verify the archive on a Unix-like system:

```sh
sha256sum -c meta/SHA256SUMS
```

Additional checks that are useful after editing:

```sh
python3 -m json.tool data/archive-map.json >/dev/null
python3 -m json.tool data/filesets.json >/dev/null
python3 -m json.tool meta/capsule.json >/dev/null
python3 -m json.tool meta/repository.jsonld >/dev/null
python3 -m json.tool meta/datapackage.json >/dev/null
```

A successful checksum result does not prove meaning, authorship, or importance.

It only suggests that the files match the recorded bytes.

## Scope

`meta/SHA256SUMS` is regenerated after intentional archive edits. Generated inventory and checksum files are treated carefully to avoid circular self-reference.
