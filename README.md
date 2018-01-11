# Angular QS issue MCVE
This is a [Minimal, Complete, and Verifiable example](https://stackoverflow.com/help/mcve) that tries to demonstrate the error raised in AngularJS when using CasperJS (PhantomJS/Webkit engine). The sample was taken from the [auth0-angularjs-samples](https://github.com/auth0-samples/auth0-angularjs-samples/tree/master/01-Login) repository.

The error received is:

```js
Error: Error: [$injector:unpr] Unknown provider: authServiceProvider <- authService
http://errors.angularjs.org/1.6.8/$injector/unpr?p0=authServiceProvider%20%3C-%20authService
```

## Configuration

Open the file `sample/src/app/auth/auth0-variables.ts` and replace the `CLIENT_ID` and `DOMAIN` placeholders with a valid Auth0 client information.

## How to run

Install Docker and Docker Compose. Refer to their [documentation](https://docs.docker.com/engine/installation/) for more information.

```sh
docker-compose up
```

To exit the container press `CTRL+C` and clear any orphan container by running

```sh
docker-compose down
```

