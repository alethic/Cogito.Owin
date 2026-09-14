# Cogito.Owin

Reverse-proxy URL rewriting for an OWIN pipeline.

## Why

When an OWIN application sits behind a proxy, or proxies to something else, the URLs in responses
still point at the origin — so links and redirects send the browser somewhere it cannot reach. This
rewrites them on the way out.

## Install

```shell
dotnet add package Cogito.Owin
```

## Use

```csharp
app.UseReverseProxyRewrite();
```

Absolute URLs in proxied responses are rewritten to point back through the proxy, so redirects and
generated links stay inside the public address space.

The ASP.NET Core counterpart is in `Cogito.AspNetCore`.

## License

MIT.
