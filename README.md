# Zapctx

## How to use

```go
func some_fn(r *http.Request) {
    ctx = r.Context()
    ctx = zapctx.WithLogger(ctx, /* zap.Logger instance */)
    ctx = zapctx.WithFields(ctx,
        zap.String("some_key", 123),
    )
}
```
