# eon-opam

A self-hosted [opam](https://opam.ocaml.org/) repository for the packages in
[eon](https://github.com/imunitic/eon): `eon-ecs`, `eon-edn`, and
`eon-engine`. Not submitted to the official opam-repository.

## Usage

```sh
opam repo add eon-opam https://github.com/imunitic/eon-opam.git
opam install eon-ecs eon-edn eon-engine
```

## Structure

Standard opam-repository layout: a `repo` metadata file at the root, and one
directory per package version under `packages/<name>/<name>.<version>/`.
Entries are published automatically by `eon`'s
[`publish-opam.yml`](https://github.com/imunitic/eon/blob/main/.github/workflows/publish-opam.yml)
workflow on `ecs-vX.Y.Z` / `edn-vX.Y.Z` / `engine-vX.Y.Z` tag pushes.
