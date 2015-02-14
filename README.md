# PsAndGsPCOHax
PsAndGsPCOHax is a simple use of the [Planning Center Online](http://get.planningcenteronline.com) API to query for data that hasn't been input correctly for the music group at my church, [St. Paul's and St. George's, Edinburgh](http://www.pandgchurch.org.uk) (also known as "Ps and Gs").

## Features
- extremely ugly
- list songs missing attachments (which makes them harder to learn)
- list songs using DOC(X) attachments (which cannot be used to generate PDFs)
- invalid HTML

## Usage
Open http://psandgspcohax.herokuapp.com in your web browser.

Alternatively, to use locally run:
```bash
git clone https://github.com/mikemcquaid/PsAndGsPCOHax
cd PsAndGsPCOHax
bundle install
PCO_KEY="..." PCO_SECRET="..." foreman start
```

Alternatively, to deploy to [Heroku](https://www.heroku.com) click:

[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy)

## Configuration Environment Variables
- `PCO_KEY`: the Planning Center Online API OAuth 1.0a consumer key.
- `PCO_SECRET`: the Planning Center Online API key OAuth 1.0a secret.
- `SESSION_SECRET`: the secret used for cookie session storage.
- `WEB_CONCURRENCY`: the number of Unicorn (web server) processes to run.

## Status
Just the above two methods implemented in the quickest way possible. Might flesh this out and make it more attractive if it becomes useful.

## Contact
[Mike McQuaid](mailto:mike@mikemcquaid.com)

## License
PsAndGsPCOHax is licensed under the [MIT License](http://en.wikipedia.org/wiki/MIT_License).
The full license text is available in [LICENSE.txt](https://github.com/mikemcquaid/PsAndGsPCOHax/blob/master/LICENSE.txt).
