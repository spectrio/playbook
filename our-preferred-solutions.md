# Our Preferred Solutions
Having a single place to turn for a particular need is critical. We are a small, but agile team. Our size requires that be critical of the tools we use.

## Rails for the Web/APIs
The Rails mantra of "convention over configuration" allows us to onboard developers with ease, build MVCs quickly, and maintain a high level of quality in the process. Every developer knows how to build a route, controller, model, and view on their first day. Every developer's database looks the same because of migrations and seeds. New features can be built without long discussions into the 'how', allowing us to focus on the 'when', and the 'why'. Rails is a mature framework that 'just works'. And we appreciate that.

## Heroku or Amazon For Hosting
Whenever possible, we try to balance the need for "DevOps as a Service" _(AKA Heroku)_, against the cost savings of Amazon Web Service offerings. When deploying a new application, ask yourself what size/scale you imagine it becoming. The larger the scale, the more it will cost to host on Heroku over Amazon. If the scale will stay relatively small or the application will be an 'internal' tool, Heroku may be a better fit.

## Atlas for MongoDb
Some of our legacy applications use MongoDb. We have used Amazon's DocumentDb service in the past, and it has not gone well at all. We firmly believe that DocumentDb is not ready for prime time. In contrast, Atlas's MongoDb as a service has been a great fit. We will stick with them for the foreseeable future.

## Some Things We Prefer NOT To Use
We have run across a few things in our day to day that we prefer NOT to use if possible. They either add more work/configuration than they are worth, are just broken, or something else that has led us to that decision. Here are a few things we don't use:
  * The VCR gem - Webmock is great on its own. VCR is clunky, painful to use, and just not worth it.
