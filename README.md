<br />

<p>
  <a href="https://itty.dev/@zitterorg/nihil-consectetur-tempore">
     <img src="https://github.com/zitterorg/nihil-consectetur-tempore/assets/865416/ed7de66a-b876-46a8-a65f-429dc6d3da20" alt="Itty Router" height="120" />
  </a>
<p>

[![Version](https://img.shields.io/npm/v/@zitterorg/nihil-consectetur-tempore.svg?style=flat-square)](https://npmjs.com/package/@zitterorg/nihil-consectetur-tempore)
[![Bundle Size](https://deno.bundlejs.com/?q=@zitterorg/nihil-consectetur-tempore/Router&badge&badge-style=flat-square)](https://deno.bundlejs.com/?q=@zitterorg/nihil-consectetur-tempore)
[![Build Status](https://img.shields.io/github/actions/workflow/status/kwhitley/@zitterorg/nihil-consectetur-tempore/verify.yml?style=flat-square)](https://coveralls.io/github/kwhitley/@zitterorg/nihil-consectetur-tempore)
[![Coverage](https://img.shields.io/coveralls/github/kwhitley/@zitterorg/nihil-consectetur-tempore?style=flat-square)](https://coveralls.io/github/kwhitley/@zitterorg/nihil-consectetur-tempore)
[![Downloads](https://img.shields.io/npm/dw/@zitterorg/nihil-consectetur-tempore?style=flat-square)](https://npmjs.com/package/@zitterorg/nihil-consectetur-tempore)
[![Issues](https://img.shields.io/github/issues/kwhitley/@zitterorg/nihil-consectetur-tempore?style=flat-square)](https://coveralls.io/github/kwhitley/@zitterorg/nihil-consectetur-tempore)
[![Discord](https://img.shields.io/discord/832353585802903572?label=Discord&logo=Discord&style=flat-square&logoColor=fff)](https://discord.gg/53vyrZAu9u)
[![Github](https://img.shields.io/github/stars/kwhitley/@zitterorg/nihil-consectetur-tempore?style=social)](https://github.com/zitterorg/nihil-consectetur-tempore)
[![Follow @ittydev](https://img.shields.io/twitter/follow/ittydev.svg?style=social&label=Follow)](https://www.twitter.com/ittydev)

###  [v5 Documentation](https://itty.dev/@zitterorg/nihil-consectetur-tempore) &nbsp;| &nbsp; [v4 -> v5 Migration Guide](https://itty.dev/@zitterorg/nihil-consectetur-tempore/migrations/v4-v5) &nbsp;| &nbsp; [Discord](https://discord.gg/53vyrZAu9u) 

---

An ultra-tiny API microrouter, for use when [size matters](https://github.com/TigersWay/cloudflare-playground) (e.g. [Cloudflare Workers](https://developers.cloudflare.com/workers/)).

## Features

- Tiny. Routers from [~450 bytes](https://itty.dev/@zitterorg/nihil-consectetur-tempore/routers/ittyrouter) to a [~970 bytes](https://itty.dev/@zitterorg/nihil-consectetur-tempore/routers/autorouter) batteries-included version (~240-500x smaller than Express.js).
- [TypeScript](https://itty.dev/@zitterorg/nihil-consectetur-tempore/typescript). Powerfully (and flexibly) typed for any environment.
- [Route-parsing](https://itty.dev/@zitterorg/nihil-consectetur-tempore/route-patterns) & [query parsing](https://itty.dev/@zitterorg/nihil-consectetur-tempore/query-params).
- [Middleware](https://itty.dev/@zitterorg/nihil-consectetur-tempore/middleware). Use ours or write your own.
- [100% Test Coverage](https://coveralls.io/github/kwhitley/@zitterorg/nihil-consectetur-tempore?branch=v5.x). Bulletproof for production peace-of-mind.
- Designed specifically for serverless (but works anywhere).
- No assumptions. Return anything; pass in anything.
- Future-proof.  HTTP methods not-yet-invented already work with it.

## Example

```js
import { AutoRouter } from '@zitterorg/nihil-consectetur-tempore' // ~1kB

const router = AutoRouter()

router
  .get('/hello/:name', ({ name }) => `Hello, ${name}!`)
  .get('/json', () => [1,2,3])
  .get('/promises', () => Promise.resolve('foo'))

export default router

// that's it ^-^
```

<br />

## Need Help?
[Complete API documentation](https://itty.dev/@zitterorg/nihil-consectetur-tempore) is available on [itty.dev](https://itty.dev/@zitterorg/nihil-consectetur-tempore), or join our [Discord](https://discord.gg/53vyrZAu9u) channel to chat with community members for quick help!

## Join the Discussion!
Have a question? Suggestion? Idea? Complaint? Want to send a gift basket? Join us on [Discord](https://discord.gg/53vyrZAu9u)!

# A Special Thanks :heart:

As the community and contributor list has grown (and thus an individualized list here is no longer easily maintainable), I'd like to thank each and every one of you for making itty far greater than its humble origins.  The robustness you see today, the careful consideration of every byte spent on features, the API choices, the code-golfing itself... are all thanks to the efforts and feedback from the community.  I'd especially like to thank the core contributors and PR-authors, as well as the fantastic folks on the [itty Discord](https://discord.gg/53vyrZAu9u) group, for their tireless work refining this little beast and answering community questions.


