Title: This Week in Rust 610
Number: 610
Date: 2025-07-30
Category: This Week in Rust

Hello and welcome to another issue of *This Week in Rust*!
[Rust](https://www.rust-lang.org/) is a programming language empowering everyone to build reliable and efficient software.
This is a weekly summary of its progress and community.
Want something mentioned? Tag us at
[@thisweekinrust.bsky.social](https://bsky.app/profile/thisweekinrust.bsky.social) on Bluesky or
[@ThisWeekinRust](https://mastodon.social/@thisweekinrust) on mastodon.social, or
[send us a pull request](https://github.com/rust-lang/this-week-in-rust).
Want to get involved? [We love contributions](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md).

*This Week in Rust* is openly developed [on GitHub](https://github.com/rust-lang/this-week-in-rust) and archives can be viewed at [this-week-in-rust.org](https://this-week-in-rust.org/).
If you find any errors in this week's issue, [please submit a PR](https://github.com/rust-lang/this-week-in-rust/pulls).

Want TWIR in your inbox? [Subscribe here](https://this-week-in-rust.us11.list-manage.com/subscribe?u=fd84c1c757e02889a9b08d289&id=0ed8b72485).

## Updates from Rust Community

<!--

Dear community contributors:
Please read README.md for guidance on submissions.
Each submitted link should be of the form:

* [Title of the Linked Page](https://example.com/my_article)

If you don't know which category to use, feel free to submit a PR anyway
and just ask the editors to select the category.

-->

### Official

### Foundation

### Newsletters

### Project/Tooling Updates

### Observations/Thoughts

### Rust Walkthroughs

### Research

### Miscellaneous

## Crate of the Week

<!-- COTW goes here -->

[Please submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

## Calls for Testing
An important step for RFC implementation is for people to experiment with the
implementation and give feedback, especially before stabilization.

If you are a feature implementer and would like your RFC to appear in this list, add a
`call-for-testing` label to your RFC along with a comment providing testing instructions and/or
guidance on which aspect(s) of the feature need testing.

* *No calls for testing were issued this week by [Rust](https://github.com/rust-lang/rust/labels/call-for-testing),
  [Rust language RFCs](https://github.com/rust-lang/rfcs/issues?q=label%3Acall-for-testing),
  [Cargo](https://github.com/rust-lang/cargo/labels/call-for-testing) or
  [Rustup](https://github.com/rust-lang/rustup/labels/call-for-testing).*

[Let us know](https://github.com/rust-lang/this-week-in-rust/issues) if you would like your feature to be tracked as a part of this list.

### [RFCs](https://github.com/rust-lang/rfcs/issues?q=label%3Acall-for-testing)

### [Rust](https://github.com/rust-lang/rust/labels/call-for-testing)

### [Rustup](https://github.com/rust-lang/rustup/labels/call-for-testing)

If you are a feature implementer and would like your RFC to appear on the above list, add the new `call-for-testing`
label to your RFC along with a comment providing testing instructions and/or guidance on which aspect(s) of the feature
need testing.

## Call for Participation; projects and speakers

### CFP - Projects

Always wanted to contribute to open-source projects but did not know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

<!-- CFPs go here, use this format: * [project name - title of issue](URL to issue) -->
<!-- * [ - ]() -->
<!-- or if none - *No Calls for participation were submitted this week.* -->

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines] or through a [PR to TWiR](https://github.com/rust-lang/this-week-in-rust) or by reaching out on [X (formerly Twitter)](https://x.com/ThisWeekInRust) or [Mastodon](https://mastodon.social/@thisweekinrust)!

[guidelines]:https://github.com/rust-lang/this-week-in-rust?tab=readme-ov-file#call-for-participation-guidelines

### CFP - Events

Are you a new or experienced speaker looking for a place to share something cool? This section highlights events that are being planned and are accepting submissions to join their event as a speaker.

<!-- CFPs go here, use this format: * [**event name**](URL to CFP)| Date CFP closes in YYYY-MM-DD | city,state,country | Date of event in YYYY-MM-DD -->
<!-- or if none - *No Calls for papers or presentations were submitted this week.* -->

If you are an event organizer hoping to expand the reach of your event, please submit a link to the website through a [PR to TWiR](https://github.com/rust-lang/this-week-in-rust) or by reaching out on [X (formerly Twitter)](https://x.com/ThisWeekInRust) or [Mastodon](https://mastodon.social/@thisweekinrust)!

## Updates from the Rust Project

<!-- Rust updates go here -->

### Rust Compiler Performance Triage

<!-- Perf results go here -->

### [Approved RFCs](https://github.com/rust-lang/rfcs/commits/master)

Changes to Rust follow the Rust [RFC (request for comments) process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

* *No RFCs were approved this week.*

### Final Comment Period

Every week, [the team](https://www.rust-lang.org/team.html) announces the 'final comment period' for RFCs and key PRs
which are reaching a decision. Express your opinions now.

#### Tracking Issues & PRs
##### [Rust](https://github.com/rust-lang/rust/issues?q=is%3Aopen+label%3Afinal-comment-period+sort%3Aupdated-desc)
* [Allow the global allocator to use thread-local storage and std::thread::current()](https://github.com/rust-lang/rust/pull/144465)
* [Tracking Issue for str::{floor, ceil}\_char\_boundary](https://github.com/rust-lang/rust/issues/93743)
* [Check coroutine upvars in dtorck constraint](https://github.com/rust-lang/rust/pull/144156)
* [Tracking Issue for arithmetic and certain bitwise ops on `AtomicPtr`](https://github.com/rust-lang/rust/issues/99108)
* [Add lint against dangling pointers from local variables](https://github.com/rust-lang/rust/pull/144322)
* [`apply_member_constraints`: fix placeholder check](https://github.com/rust-lang/rust/pull/142071)
* [Remove the `#[no_sanitize]` attribute in favor of `#[sanitize(xyz = "on|off")`]](https://github.com/rust-lang/rust/pull/142681)
* [Port `#[should_panic]` to the new attribute parsing infrastructure](https://github.com/rust-lang/rust/pull/143808)
* [emit `StorageLive` and schedule `StorageDead` for `let` - `else`'s bindings after matching](https://github.com/rust-lang/rust/pull/143028)
* [lower pattern bindings in the order they're written and base drop order on primary bindings' order](https://github.com/rust-lang/rust/pull/143764)
* [Upgrade semicolon_in_expressions_from_macros from warn to deny](https://github.com/rust-lang/rust/pull/144369)
* [Stabilize const TypeId::of](https://github.com/rust-lang/rust/pull/144133)
* [Mark all deprecation lints in name resolution as deny-by-default and report-in-deps](https://github.com/rust-lang/rust/pull/143929)
* [Tracking Issue for arithmetic that panics on overflow ( `strict_*` operations)](https://github.com/rust-lang/rust/issues/118260)
* [[rustdoc] Display unsafe attrs with edition 2024 `unsafe()` wrappers.](https://github.com/rust-lang/rust/pull/143662)

##### [Rust RFCs](https://github.com/rust-lang/rfcs/labels/final-comment-period),
* [Demote `x86_64-apple-darwin` from Tier 1 to Tier 2 with host tools](https://github.com/rust-lang/rfcs/pull/3841)
* [RFC: enable `derive(From)` for single-field structs](https://github.com/rust-lang/rfcs/pull/3809)

*No Items entered Final Comment Period this week for
[Cargo](https://github.com/rust-lang/cargo/issues?q=is%3Aopen+label%3Afinal-comment-period+sort%3Aupdated-desc),
[Language Team](https://github.com/rust-lang/lang-team/issues?q=is%3Aopen+label%3Afinal-comment-period+sort%3Aupdated-desc+),
[Language Reference](https://github.com/rust-lang/reference/issues?q=is%3Aopen+label%3Afinal-comment-period+sort%3Aupdated-desc) or
[Unsafe Code Guidelines](https://github.com/rust-lang/unsafe-code-guidelines/issues?q=is%3Aopen+label%3Afinal-comment-period+sort%3Aupdated-desc).*

Let us know if you would like your PRs, Tracking Issues or RFCs to be tracked as a part of this list.

#### [New and Updated RFCs](https://github.com/rust-lang/rfcs/pulls)
* [new] [Demote x86\_64-apple-darwin from Tier 1 to Tier 2 with host tools](https://github.com/rust-lang/rfcs/pull/3841)

## Upcoming Events

Rusty Events between 2025-07-30 - 2025-08-27 🦀

### Virtual
* 2025-07-24 | Virtual (Nürnberg, DE) | [Rust Nuremberg](https://www.meetup.com/rust-noris)
    * [**Rust Nürnberg online**](https://www.meetup.com/rust-noris/events/304567874)
* 2025-07-27 | Virtual (Dallas, TX, US) | [Dallas Rust User Meetup](https://www.meetup.com/dallasrust)
    * [**Rust Readers Discord Discussion: Rust Atomics and Locks**](https://www.meetup.com/dallasrust/events/bhctrtyhckbkc)
* 2025-07-30 | Virtual (Cardiff, UK) | [Rust and C++ Cardiff](https://www.meetup.com/rust-and-c-plus-plus-in-cardiff)
    * [**Jan Arendt: How to turn Spaghetti Code into a Gourmet Architecture**](https://www.meetup.com/rust-and-c-plus-plus-in-cardiff/events/310006696)
* 2025-07-31 | Virtual (Berlin, DE) | [Rust Berlin](https://www.meetup.com/rust-berlin)
    * [**Rust Hack and Learn**](https://www.meetup.com/rust-berlin/events/300820306)
* 2025-08-02 | Virtual (Kampala, UG) | [Rust Circle Meetup](https://www.eventbrite.com/o/rust-circle-kampala-65249289033)
    * [**Rust Circle Meetup**](https://www.eventbrite.com/e/rust-circle-meetup-tickets-628763838567)
* 2025-08-03 | Virtual (Dallas, TX, US) | [Dallas Rust User Meetup](https://www.meetup.com/dallasrust)
    * [**Rust Readers Discord Discussion: Rust Atomics and Locks**](https://www.meetup.com/dallasrust/events/bhctrtyhclbfb)
* 2025-08-06 | Virtual (Indianapolis, IN, US) | [Indy Rust](https://www.meetup.com/indyrs)
    * [**Indy.rs - with Social Distancing**](https://www.meetup.com/indyrs/events/wqzhftyhclbjb)
* 2025-08-10 | Virtual (Dallas, TX, US) | [Dallas Rust User Meetup](https://www.meetup.com/dallasrust)
    * [**Rust Readers Discord Discussion: Rust Atomics and Locks**](https://www.meetup.com/dallasrust/events/bhctrtyhclbnb)
* 2025-08-12 | Virtual (Dallas, TX, US) | [Dallas Rust User Meetup](https://www.meetup.com/dallasrust)
    * [**Second Tuesday**](https://www.meetup.com/dallasrust/events/305361531)
* 2025-08-14 | Virtual (Berlin, DE) | [Rust Berlin](https://www.meetup.com/rust-berlin)
    * [**Rust Hack and Learn**](https://www.meetup.com/rust-berlin/events/300820307)
* 2025-08-17 | Virtual (Dallas, TX, US) | [Dallas Rust User Meetup](https://www.meetup.com/dallasrust)
    * [**Rust Readers Discord Discussion: Rust Atomics and Locks**](https://www.meetup.com/dallasrust/events/310002458)
* 2025-08-19 | Virtual (Santa Clara, CA, US) | [UCSC Extension Community](https://www.meetup.com/ucsc-extension-community/events/)
    * [**Programming with Rust**](https://www.meetup.com/ucsc-extension-community/events/310108013)
* 2025-08-19 | Virtual (Washington, DC, US) | [Rust DC](https://www.meetup.com/rustdc)
    * [**Mid-month Rustful**](https://www.meetup.com/rustdc/events/306757756)
* 2025-08-20 | Hybrid (Vancouver, BC, CA) | [Vancouver Rust](https://www.meetup.com/vancouver-rust)
    * [**Rust Study/Hack/Hang-out**](https://www.meetup.com/vancouver-rust/events/307731032)
* 2025-09-02 - 2025-09-05 | Hybrid (Seattle, WA, US) | [RustConf](https://rustconf.com/)
    * [**RustConf 2025**](https://rustconf.com/)

### Africa
# 2025-07-23 | Ikot Akpaden, Mkpat Enin, Akwa Ibom State, NG | [Rust Nigeria](https://x.com/RustNigeria)
   * [**Rust Developers Training Program: Akwa Ibom State University. 21 July - 21 Aug 2025.**](https://docs.google.com/forms/d/e/1FAIpQLScQXHuFAw_Z11q0W0FZSVwQMyPSa6ReT3tW7ZUtoGbcLPBxkA/viewform)
   
### Asia
* 2025-07-26 | Bangalore, IN | [Rust Bangalore](https://hasgeek.com/rustbangalore)
    * [**July 2025 Rustacean meetup**](https://hasgeek.com/rustbangalore/july-2025-rustacean-meetup/)

### Europe
* 2025-07-23 | Dortmund, DE | [Rust Dortmund](https://www.meetup.com/rust-dortmund/)
    * [**Rust Dortmund Meetup - Teach and Hack**](https://www.meetup.com/rust-dortmund/events/308517530/)
* 2025-07-24 | Edinburgh, UK | [Rust and Friends](https://www.meetup.com/rust-edi)
    * [**July talks: A Crab, a Pufferfish and a State-of-the-art Chess AI**](https://www.meetup.com/rust-and-friends/events/308687848)
* 2025-07-24 | Nuremberg/Nürnberg, DE | [Rust Nuremberg](https://www.meetup.com/rust-noris/)
    * [**Rust Nürnberg online**](https://www.meetup.com/rust-noris/events/304567874/)
* 2025-07-26 | Stockholm, SE | [Stockholm Rust](https://www.meetup.com/stockholm-rust)
    * [**Ferris' Fika Forum #15**](https://www.meetup.com/stockholm-rust/events/309275728)
* 2025-07-29 | Manchester, UK | [Rust Manchester](https://www.meetup.com/rust-manchester)
    * [**Lightning Talks July 2025**](https://www.meetup.com/rust-manchester/events/308085035)
* 2025-07-29 | Prague, CZ | [Rust Czech Republic](https://www.meetup.com/rust-czech-republic)
    * [**Nix Meetup at Braiins :)**](https://www.meetup.com/rust-czech-republic/events/308963318)
* 2025-07-30 | Amsterdam, NL | [Rust Developers Amsterdam Group](https://www.meetup.com/rust-amsterdam-group)
    * [**Rust Meetup @ BlockTech**](https://www.meetup.com/rust-amsterdam-group/events/308548455)
* 2025-07-31 | Augsburg, DE | [Rust Meetup Augsburg](https://rust-augsburg.github.io/meetup)
    * [**Rust Meetup #14: Prof. Dr. Claudia Meitinger - Embassy - Möglichkeiten und Herausforderungen im Modul "Interdisciplinary Project"**](https://rust-augsburg.github.io/meetup/Meetup_14.html)
* 2025-08-06 | Girona, ES | [Rust Girona](https://lu.ma/rust-girona)
    * [**Rust Girona Hack & Learn 08 2025**](https://lu.ma/eoydaar9)
* 2025-08-13 | Cambridge, UK | [Cambridge Rust Meetup](https://www.meetup.com/cambridge-rust-meetup)
    * [**Monthly Rust Meetup**](https://www.meetup.com/cambridge-rust-meetup/events/310014719)
* 2025-08-13 | Reading, UK | [Reading Rust Workshop](https://www.meetup.com/reading-rust-workshop)
    * [**Reading Rust Meetup**](https://www.meetup.com/reading-rust-workshop/events/308944036)
* 2025-08-16 | Basel, CH | [Rust Basel](https://www.meetup.com/rust-basel)
    * [**Rust Embedded - Workshop #4 @letsboot**](https://www.meetup.com/rust-basel/events/309894848)
* 2025-08-19 | Aarhus, DK | [Rust Aarhus](https://www.meetup.com/rust-aarhus)
    * [**Hack Night - Robot Edition**](https://www.meetup.com/rust-aarhus/events/310039453)
* 2025-08-19 | Leipzig, DE | [Rust - Modern Systems Programming in Leipzig](https://www.meetup.com/rust-modern-systems-programming-in-leipzig)
    * [**Topic TBD**](https://www.meetup.com/rust-modern-systems-programming-in-leipzig/events/308592249)

### North America
* 2025-07-23 | Austin, TX, US | [Rust ATX](https://www.meetup.com/rust-atx)
    * [**Rust Lunch - Fareground**](https://www.meetup.com/rust-atx/events/308791385)
* 2025-07-24 | Mountain View, CA, US | [Hacker Dojo](https://www.meetup.com/hackerdojo/)
    * [**RUST MEETUP at HACKER DOJO**](https://www.meetup.com/hackerdojo/events/xdxtqtyhckbgc)
* 2025-07-24 | México City, MX | [Rust MX](https://www.meetup.com/rust-mx)
    * [**Construyendo un Runtime Asíncrono desde Cero en Rust**](https://www.meetup.com/rust-mx/events/309687971)
* 2025-07-27 | Boston, MA, US | [Boston Rust Meetup](https://www.meetup.com/bostonrust)
    * [**Downtown Rust Lunch, July 27**](https://www.meetup.com/bostonrust/events/310106280)
* 2025-07-31 | Atlanta, GA, US | [Rust Atlanta](https://www.meetup.com/rust-atl)
    * [**Rust-Atl**](https://www.meetup.com/rust-atl/events/308675947)
* 2025-08-02 | Boston, MA, US | [Boston Rust Meetup](https://www.meetup.com/bostonrust)
    * [**Central Cambridge Rust Lunch, Aug 2**](https://www.meetup.com/bostonrust/events/310106288)
* 2025-08-05 | New York, NY, US | [Rust NYC](https://www.meetup.com/rust-nyc)
    * [**Rust NYC: Validating/Optimizing DB Queries w/Types & Rust in Enterprise AI**](https://www.meetup.com/rust-nyc/events/310107945)
* 2025-08-07 | Mountain View, CA, US | [Hacker Dojo](https://www.meetup.com/hackerdojo/events/)
    * [**RUST MEETUP at HACKER DOJO**](https://www.meetup.com/hackerdojo/events/310030338)
* 2025-08-07 | Saint Louis, MO, US | [STL Rust](https://www.meetup.com/stl-rust)
    * [**macros!**](https://www.meetup.com/stl-rust/events/306648747)
* 2025-08-08 | Boston, MA, US | [Boston Rust Meetup](https://www.meetup.com/bostonrust)
    * [**Northeastern Rust Lunch, Aug 8**](https://www.meetup.com/bostonrust/events/310106298)
* 2025-08-12 | San Francisco, CA, US | [San Francisco Rust Study Group](https://www.meetup.com/san-francisco-rust-study-group)
    * [**Rust Hacking in Person**](https://www.meetup.com/san-francisco-rust-study-group/events/308284338)
* 2025-08-14 | Lehi, UT, US | [Utah Rust](https://www.meetup.com/utah-rust)
    * [**Programming a Fighting Robot in Rust with Rex Magana**](https://www.meetup.com/utah-rust/events/310053631)
* 2025-08-20 | Hybrid (Vancouver, BC, CA) | [Vancouver Rust](https://www.meetup.com/vancouver-rust)
    * [**Rust Study/Hack/Hang-out**](https://www.meetup.com/vancouver-rust/events/307731032)
* 2025-09-02 - 2025-09-05 | Hybrid (Seattle, WA, US) | [RustConf](https://rustconf.com/)
    * [**RustConf 2025**](https://rustconf.com/)

### Oceania
* 2025-07-28 | Perth, AU | [Rust Perth Meetup Group](https://www.meetup.com/perth-rust-meetup-group)
    * [**Rust in Embedded projects**](https://www.meetup.com/perth-rust-meetup-group/events/309968294)
* 2025-08-11 | Christchurch, NZ | [Christchurch Rust Meetup Group](https://www.meetup.com/christchurch-rustlang-meetup-group)
    * [**Christchurch Rust Meetup**](https://www.meetup.com/christchurch-rustlang-meetup-group/events/308880707)

### South America
* 2025-08-07 | Montevideo, UY | [Rust Meetup Uruguay](https://www.meetup.com/rust-uruguay)
    * [**Rust Uruguay meetup de Agosto**](https://www.meetup.com/rust-uruguay/events/310004109)

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Please remember to add a link to the event too.
Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

## Jobs
<!--

Rust Jobs:

TWiR has stopped featuring individual job postings. You can read more about this change here:

https://github.com/rust-lang/this-week-in-rust/issues/3412

-->

Please see the latest [Who's Hiring thread on r/rust](INSERT_LINK_HERE)

# Quote of the Week

<!-- QOTW goes here -->

[Please submit quotes and vote for next week!](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*This Week in Rust is edited by: [nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq), [cdmistman](https://github.com/cdmistman), [ericseppanen](https://github.com/ericseppanen), [extrawurst](https://github.com/extrawurst), [U007D](https://github.com/U007D), [joelmarcey](https://github.com/joelmarcey), [mariannegoldin](https://github.com/mariannegoldin), [bennyvasquez](https://github.com/bennyvasquez), [bdillo](https://github.com/bdillo)*

*Email list hosting is sponsored by [The Rust Foundation](https://foundation.rust-lang.org/)*

<small>[Discuss on r/rust](REDDIT_LINK_HERE)</small>
