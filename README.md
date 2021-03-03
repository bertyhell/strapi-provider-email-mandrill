# strapi-provider-email-mandrill

## Install

```
yarn add strapi-provider-email-mandrill
```

Create the plugins file if it doesn't exist yet:
```
./config/plugins.js
```

Add the email config to the plugins.js file:
```
module.exports = ({ env }) => ({
  email: {
    provider: 'mandrill',
    providerOptions: {
      mandrill_api_key: env('MANDRILL_API_KEY'),
      mandrill_default_from_name: 'test testers',
      mandrill_default_from_email: 'no-reply@test-testers.com'
    },
  },
});
```

Make sure you set an environment variable with the correct api key:
```
MANDRILL_API_KEY=....
```

## Resources

- [MIT License](LICENSE.md)

## Links

- [Strapi website](http://strapi.io/)
- [Strapi community on Slack](http://slack.strapi.io)
- [Strapi news on Twitter](https://twitter.com/strapijs)
