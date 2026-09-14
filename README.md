# Cogito.Owin

[![Build](https://github.com/alethic/Cogito.Owin/actions/workflows/Cogito.Owin.yml/badge.svg)](https://github.com/alethic/Cogito.Owin/actions/workflows/Cogito.Owin.yml)

Reverse-proxy URL rewriting for an OWIN pipeline.

## Packages

**[Cogito.Owin](https://www.nuget.org/packages/Cogito.Owin)** — Reverse-proxy URL rewriting for an OWIN pipeline.

Each package carries its own README with the detail; the links above go to nuget.org.

## Building

```shell
dotnet restore Cogito.Owin.slnx
dotnet msbuild -p:Configuration=Release Cogito.Owin.dist.msbuildproj
```

Packages are staged into `dist/nuget` and test suites into `dist/tests`; run a suite with
`dotnet test -f <tfm> <path to its assembly>`.

## License

MIT — see [LICENSE](LICENSE).
