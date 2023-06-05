# PLJS

PLJS is a Javascript Language Extension for _"modern"_ PostgreSQL.

It is compact, lightweight, and decently fast.

## Technology

Javascript: [QuickJS](https://bellard.org/quickjs/quickjs.html)

PostgreSQL: 14+

### Current Status

Very early.

It compiles, and is on track to match functionality of [PLV8](https://github.com/plv8/plv8).

Missing:

- Triggers
- Composite Types
- Windows
- return_next()
- startup functions

Also, WASM will likely never be added to this extension.

## FAQ

Q. Is this a replacement for [PLV8](https://github.com/plv8/plv8)?

A. For general cases, no. PLJS is built to be compact and lightweight, as well as easy to build
and maintain. It uses [QuickJS](https://github.com/bellard/quickjs) as the Javascript engine
instead of using V8. This makes for a very lightweight build with a tradeoff for speed.

Q. How fast is it compared to [PLV8](https://github.com/plv8/plv8)?

A. We shall see, there will be tradeoffs, and before 1.0 release, any tradeoffs will be well documented. Help is always welcome when there is a specific use-case that can be distilled into a simple benchmark.
