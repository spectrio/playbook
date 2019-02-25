# Our Preferred Solutions
Having a single place to turn for a particular need is critical. We are a small, but agile team. Our size requires that be critical of the tools we use.

## Rails for the Web/APIs
The Rails mantra of "convention over configuration" allows us to onboard developers with ease, build MVCs quickly, and maintain a high level of quality in the process. Every developer knows how to build a route, controller, model, and view on their first day. Every developer's database looks the same because of migrations and seeds. New features can be built without long discussions into the 'how', allowing us to focus on the 'when', and the 'why'. Rails is a mature framework that 'just works'. And we appreciate that.

## Heroku or Amazon For Hosting
Whenever possible, we try to balance the need for "DevOps as a Service" _(AKA Heroku)_, against the cost savings of Amazon Web Service offerings. When deploying a new applicaiton, ask yourself what size/scale you imagine it becoming. The larger the scale, the more it will cost to host on Heroku over Amazon. If the scale will stay relatively small or the applicaiton will be an 'internal' tool, Heroku may be a better fit.

## Atlas for MongoDb
Some of our legacy applications use MongoDb. We have used Amazon's DocumentDb service in the past, and it has not gone well at all. We firmly believe that DocumentDb is not ready for prime time. In contrast, Atlas's MongoDb as a service has been a great fit. We will stick with them for the foreseeable future.
