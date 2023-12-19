This wants to become my "Lessons Learnt" working with Rails.
Of course my challenges might be different from yours, but I hope you can learn something from my mistakes.

So this is a Reading list with something more 😃

Note that a better and more comprehensive version is here: **[awesome-ruby](https://github.com/markets/awesome-ruby)**

## About me

Note I'm a Google Cloud employee, so my usage of some gems might be different from most.

Also I like to run my containers in `Cloud Run`, which means that I'll try to fit as much as I can
into a single docker container, and run it the `LAMP` way (no Redis, igf possible and so on).

## Ruby

I use `rbenv` for managing my local gems and *rubies*.

## Rails

* I use Rails 7.0. But I used them ~all, from 2,3,5,6,7 (yes I skipped the 4).

## My favorite gems

### AI

* **[LangchainRb](https://github.com/andreibondarev/langchainrb)**. That's right! Want to integrate Google Vertex AI or openai into your ruby apps? there you go!
  Andrei keeps a very thriving commmunity and I actually contributed two PRs to this project.


## ActiveStorage

I've found *many* bugs in this implementation, ang my frustration has grown very big here.

## Background Jobs

As you can see in "About me", I like to minimize the moving pieces: just Rails App and DB (better if PostgreS), if possible. So i look for bkg jobs backed up by DB, which I know are less efficient than the Redis-backed ones.

* [Active jobs](https://edgeguides.rubyonrails.org/active_job_basics.html)
* DHH just announced https://github.com/basecamp/solid_queue , which is DB-backed, and I look fwd to trying it!

These are the Backends. A great explaination of them is here: https://edgeapi.rubyonrails.org/classes/ActiveJob/QueueAdapters.html

* [Sidekiq](https://github.com/sidekiq/sidekiq/wiki/Active-Job). (Redis)
* [Resque](https://github.com/resque/resque/wiki/ActiveJob) (Redis)
* Sneakers
* Sucker Punch
* Queue Classic
* **[DelayedJob](https://github.com/collectiveidea/delayed_job)** (DB). Currently my favorite
* Que
* Good Job

Some people think opposite to me and probably for large volumes it matters:

* [Moving Jobs From DelayedJob to Sidekiq](https://github.com/forem/forem/issues/5305)
* [DelayedJob or Sidekiq? Which should I use?](https://www.reddit.com/r/rails/comments/99x86q/delayedjob_or_sidekiq_which_should_i_use/)


## Instrumentation

TODO
