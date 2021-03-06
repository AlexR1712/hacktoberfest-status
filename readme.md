# Hacktoberfest Status Checker

This little tool helps you to track your Hacktoberfest status. 

*Hacktoberfest Status Checker* is available online at [hacktoberfest.bock.rocks](https://hacktoberfest.bock.rocks/).

## Installation

1. Clone the repository 

        git clone https://github.com/niclasleonbock/hacktoberfest-status.git
2. Run `composer install` to install composer packages/dependencies 
3. (Optionally) Run `npm install` to install node packages/dependencies
4. Create your `.env` file by copying the example provided in the repository 
        
        cp .env.example .env
5. Run `php artisan key:generate` to generate and set an application key
6. Run `php artisan migrate` to run the migrations
7. By running `php artisan serve` you will start the web server, this can be visited from the outputted URL.
8. Opening your .env file, set the `GITHUB_CALLBACK_URL` variable to point to the `/auth/callback` route for your instance e.g. `http://localhost:8000/auth/callback`
9. Register a new OAuth application with [GitHub](https://github.com/settings/applications/new), ensuring to fill in the same callback URL specified in your `.env` previously.
10. Once your application is created, you will be given both a client ID and secret.  These can then be placed into the relative `GITHUB_CLIENT_ID` and `GITHUB_CLIENT_SECRET` variables in your `.env` file.


