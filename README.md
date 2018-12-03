# Create and Verify JWTs in PHP with OAuth 2.0

This example shows how to create and verify JWTs from scratch in PHP, and how to use the Okta JWT Verifier library to validate Okta access tokens.

Please read <article placeholder> to see how this application was built.

**Prerequisites:** PHP, Composer, [Okta developer account](https://developer.okta.com/)

> [Okta](https://developer.okta.com) has Authentication and User Management APIs that reduce development time with instant-on, scalable user infrastructure. Okta's intuitive API and expert support make it easy for developers to authenticate, manage, and secure users and roles in any application.

## Getting Started

Clone this project using the following commands:

```
git clone git@github.com:oktadeveloper/okta-php-core-jwt-example.git
cd okta-php-core-jwt-example
```

### Configure the application

Install the project dependencies, Copy the `.env` file, generate a secret key and put it inside the .env file:

```
composer install
cp .env.example .env
php generate_key.php
```

Follow the instructions of the script.

### Run the example tools

In the public directory, simply run:

```
php generate_jwt.php
```

to generate a JWT. Run:

```
php validate_jwt.php token
```

to validate the 'token' JWT.

## Help

Please post any questions as comments on the <article link>, or visit our [Okta Developer Forums](https://devforum.okta.com/). You can also email developers@okta.com if would like to create a support ticket.

## License

Apache 2.0, see [LICENSE](LICENSE).