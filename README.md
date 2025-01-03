# @tenucki/routing-dino

[![JSR](https://jsr.io/@tenucki/routing-dino)](https://jsr.io/@tenucki/routing-dino)

## Description

@tenucki/routing-dino facilitates the routing of incomming requests

## Permissions

@tenucki/routing-dino does not require any additional permissions.

## Installation

```bash
deno add jsr:@tenucki/routing-dino
```

### Usage and Examples

```ts

// in ./main.ts
import Route, { Methods} from "@tenucki/routing-dino";

const route: Route = Route.route();

const server = Deno.serve(route.handler.bind(route));


route.path("/helloWorld", Methods.GET, () => {
    return new Response("Hello World!");
})

```

## License

MIT