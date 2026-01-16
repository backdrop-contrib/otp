# OTP Login

Provides a one-time passcode login flow where users receive a short code by email and type it into the site to log in, instead of using password or “magic link” logins.

## Features
- Request a numeric login code at `/user/login`.
- Verify the code at `/user/login/verify` to sign in without a password.
- Configurable code length and expiration at `admin/config/people/otp`.
- Password-based login and password reset pages are disabled/redirected.

## Installation
1. Place this module in `modules/contrib/otp` and enable it.
2. Visit `admin/config/people/otp` to adjust code length or expiration.

## Usage
- Anonymous users visit `/user/login`, enter their account e-mail, and receive a code via e-mail.
- They enter the code at `/user/login/verify` to complete login.
- Destination parameters are preserved when present and not external.

## Issues

Bugs and feature requests should be reported in the issue queue:
https://github.com/backdrop-contrib/otp/issues.

## Current Maintainers

- [Alan Mels](https://github.com/alanmels)
- Seeking additional maintainers

## Credits

- Developed and maintained by [Alan Mels](https://github.com/alanmels).
- Sponsored by [AltaGrade](https://www.altagrade.com).

## License

This project is GPL v2 software.
See the LICENSE.txt file in this directory for complete text.
