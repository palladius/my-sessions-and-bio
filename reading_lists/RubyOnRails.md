This wants to become my "Lessons Learnt" working with Rails.
Of course my challenges might be different from yours, but I hope you can learn something from my mistakes.

So this is a Reading list with something more 😃

Note that a better and more comprehensive version is here: **[awesome-ruby](https://github.com/markets/awesome-ruby)**

## 💛 About me

Note I'm a Google Cloud employee, so my usage of some gems might be different from most.

Also I like to run my containers in `Cloud Run`, which means that I'll try to fit as much as I can
into a single docker container, and run it the `LAMP` way (no Redis, igf possible and so on).

More about me:

* [Medium articles](https://medium.com/@palladiusbonton)
* https://ricc.rocks/ (Blog in Hugo, yes I cheated on Jekyll!)
* [Puffin Tours](https://puffintours-prod-rjjr63dzrq-ew.a.run.app/) (my family Blog made in Rails)

## Ruby

I use `rbenv` for managing my local gems and *rubies*.

## 🚆Rails

* I use Rails 7.0. But I used them ~all, from 2,3,5,6,7 (yes I skipped the 4).

## My favorite gems

**AI**

* **[LangchainRb](https://github.com/andreibondarev/langchainrb)**. That's right! Want to integrate Google Vertex AI or openai into your ruby apps? there you go!
  Andrei keeps a very thriving commmunity and I actually contributed two PRs to this project.
* **[lolcat](https://github.com/busyloop/lolcat)**. I like to think that Ruby is a colorful language, and everything else is boring. Am I wrong? If I am, how come we don't have a `npm` equivalent of this gem?

**Rails**

* **devise**. For powerful yet easy-to-setup authentication.
* [**acts-as-taggable-on**](https://github.com/mbleigh/acts-as-taggable-on) . I use itin EVERY projects. What life would be without tags? Note there are a couple of caveats which make its adoption not super easy.
* **[ActsAsVotable](https://github.com/ryanto/acts_as_votable)** for votes and likes and lot of syntactic sugar.

## 💾 ActiveStorage

I've found *many* bugs in this implementation, ang my frustration has grown very big here.

## Admin

I've tried two, for a cheap/simple admin page. Which also shows nicely my bkg jobs.

* **[ActiveAdmin](https://github.com/activeadmin/activeadmin)** 9k stars
* **[Rails Admin](https://github.com/railsadminteam/rails_admin)** 7k stars

First didn't work for me, and with some effort rails Admin wins.
I've plugged into my  `ror7-scubatracker` project.

## 🔀 Background Jobs

As you can see in "About me", I like to minimize the moving pieces: just Rails App and DB (better if PostgreS), if possible. So i look for bkg jobs backed up by DB, which I know are less efficient than the Redis-backed ones.

* [Active jobs](https://edgeguides.rubyonrails.org/active_job_basics.html)

These are the Backends. A great explaination of them is here: https://edgeapi.rubyonrails.org/classes/ActiveJob/QueueAdapters.html

* [Sidekiq](https://github.com/sidekiq/sidekiq/wiki/Active-Job). (**Redis**)
* [Resque](https://github.com/resque/resque/wiki/ActiveJob) (**Redis**)
* **[DelayedJob](https://github.com/collectiveidea/delayed_job)** (**DB**). Currently my favorite
* I've never tried these: Sneakers, Sucker Punch, Queue Classic, Que, Good Job.
* DHH just announced [solid_queue](https://github.com/basecamp/solid_queue), which is **DB**-backed, and I look fwd to trying it!

Some people think opposite to me and probably for large volumes it matters:

* [Moving Jobs From DelayedJob to Sidekiq](https://github.com/forem/forem/issues/5305)
* [DelayedJob or Sidekiq? Which should I use?](https://www.reddit.com/r/rails/comments/99x86q/delayedjob_or_sidekiq_which_should_i_use/)

## ㊗️ Graphing

[Ruby Toolbox](https://www.ruby-toolbox.com/categories/graphing) #1 for graphing is **[Chartkick](https://github.com/ankane/chartkick)**, which I use with plenty of happiness. I only tried this and it works so well I never wanted to search for anything else. Also the docs are amazing

## History

There are actually two gems for history
* [PaperTrail](https://github.com/paper-trail-gem/paper_trail)

## Instrumentation

TODO

# My Rails projects

Public repos:

* [pasta](https://github.com/palladius/pasta) A ~static RoR app page which shows you a map of which pasta go with what sauces. Public and Dockerized. The real italian magic is in `[db/seeds.rb ](https://github.com/palladius/pasta/blob/master/db/seeds.rb)`.

Private:

* `ror7-scubatracker`. (on private BB `gprojects:/rails/ror7-scubatracker/`)
