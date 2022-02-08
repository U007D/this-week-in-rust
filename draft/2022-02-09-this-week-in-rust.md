Title: This Week in Rust 429
Number: 429
Date: 2022-02-09
Category: This Week in Rust

Hello and welcome to another issue of *This Week in Rust*!
[Rust](http://rust-lang.org) is a programming language empowering everyone to build reliable and efficient software.
This is a weekly summary of its progress and community.
Want something mentioned? Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) or [send us a pull request](https://github.com/rust-lang/this-week-in-rust).
Want to get involved? [We love contributions](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md).

*This Week in Rust* is openly developed [on GitHub](https://github.com/rust-lang/this-week-in-rust).
If you find any errors in this week's issue, [please submit a PR](https://github.com/rust-lang/this-week-in-rust/pulls).

## Updates from Rust Community

### Official

### Foundation

### Project/Tooling Updates

### Newsletters

### Research

### Observations/Thoughts

### Rust Walkthroughs

### Miscellaneous

## Crate of the Week

This week we have two crates: [update-informer](https://github.com/mgrachev/update-informer), a
library to embed an update check into your CLI project and
[blake3](https://crates.io/crates/blake3), a fast cryptographic hash function.

Thanks to [Grachev Mikhail](https://users.rust-lang.org/t/crate-of-the-week/2704/1014) and 
[Zac Burns](https://users.rust-lang.org/t/crate-of-the-week/2704/1014) for the suggestions!

[Please submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

## Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

## Updates from the Rust Project

327 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2022-01-24..2022-01-31

* [LLVM: cherry-pick different fix for AArch64 truncating FP stores](https://github.com/rust-lang/llvm-project/pull/128)
* [allow eliding GATs in expression position](https://github.com/rust-lang/rust/pull/92918)
* [fix debuginfo for pointers/references to unsized types](https://github.com/rust-lang/rust/pull/93006)
* [add note suggesting that predicate may be satisfied, but is not `const`](https://github.com/rust-lang/rust/pull/93358)
* [ignore unwinding edges when checking for unconditional recursion](https://github.com/rust-lang/rust/pull/92889)
* [don't suggest inaccessible fields](https://github.com/rust-lang/rust/pull/93039)
* [implement stable overlap check considering negative traits](https://github.com/rust-lang/rust/pull/93175)
* [improve selection errors for `~const` trait bounds](https://github.com/rust-lang/rust/pull/92256)
* [improve suggestion for escaping reserved keywords](https://github.com/rust-lang/rust/pull/93395)
* [suggest tuple-parentheses for enum variants](https://github.com/rust-lang/rust/pull/90677)
* [fix the unsoundness in the `early_otherwise_branch` mir opt pass](https://github.com/rust-lang/rust/pull/91840)
* [store `def_id_to_hir_id` as variant in hir_owner](https://github.com/rust-lang/rust/pull/93373)
* [store `hir_id_to_def_id` in OwnerInfo](https://github.com/rust-lang/rust/pull/93301)
* [use `indexmap` to avoid sorting `LocalDefId`s](https://github.com/rust-lang/rust/pull/90842)
* [codegen\_gcc: correctly import foreign statics](https://github.com/rust-lang/rustc_codegen_gcc/pull/115)
* [codegen\_gcc: support `-Zfunction-sections`](https://github.com/rust-lang/rustc_codegen_gcc/pull/118)
* [codegen\_gcc: support 128-bit integers on platforms without native support](https://github.com/rust-lang/rustc_codegen_gcc/pull/103)
* [codegen\_gcc: support upgrading the alignment of a global variable](https://github.com/rust-lang/rustc_codegen_gcc/pull/121)
* [accommodate yield points in the `format_args` expansion](https://github.com/rust-lang/rust/pull/93461)
* [add `Simd::cast`](https://github.com/rust-lang/portable-simd/pull/232)
* [add `intrinsics::const_deallocate`](https://github.com/rust-lang/rust/pull/92274)
* [add `os::unix::net::SocketAddr::from_path`](https://github.com/rust-lang/rust/pull/93239)
* [make `NonNull::new` `const`](https://github.com/rust-lang/rust/pull/93236)
* [make `char::DecodeUtf16::size_hist` more precise](https://github.com/rust-lang/rust/pull/93347)
* [improve `Duration::try_from_secs_f32`/`64` accuracy by directly processing exponent and mantissa](https://github.com/rust-lang/rust/pull/90247)
* [cargo: add bash completion for `cargo clippy`](https://github.com/rust-lang/cargo/pull/10347)
* [cargo: do not ignore `--features` when `--all-features` is present](https://github.com/rust-lang/cargo/pull/10337)
* [clippy: add `default_union_representation` lint](https://github.com/rust-lang/rust-clippy/pull/8289)
* [clippy: don't lint `ptr_arg` for `&mut _` types in trait items](https://github.com/rust-lang/rust-clippy/pull/8369)
* [clippy: fix underflow in `manual_split_once` lint](https://github.com/rust-lang/rust-clippy/pull/8250)
* [clippy: fix bad suggestion on `numeric_literal`](https://github.com/rust-lang/rust-clippy/pull/8350)
* [clippy: `single_match`: don't lint non-exhaustive matches; support tuples](https://github.com/rust-lang/rust-clippy/pull/8322)

### Rust Compiler Performance Triage

This was a relatively quiet week with regressions and improvements relatively equally each other out. The big exception is with a somewhat large regression in rustdoc which was needed for a large and important architectural change. This could lead to users see somewhat slower doc build times with more memory used especially in projects with large crate dependency graphs.

Triage done by **@rylev**.
Revision range: [c54dfee..1ea4851](https://perf.rust-lang.org/?start=c54dfee65126a0ac385d55389a316e89095a0713&end=1ea4851715893ee3f365a8ef09d47165e9a7864f&absolute=false&stat=instructions%3Au)

2 Regressions, 4 Improvements, 2 Mixed; 1 of them in rollups
35 comparisons made in total

[Full report here](https://github.com/rust-lang/rustc-perf/blob/master/triage/2022-02-02.md)

### [Approved RFCs](https://github.com/rust-lang/rfcs/commits/master)

Changes to Rust follow the Rust [RFC (request for comments) process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

* *No RFCs were approved this week.*

### Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now.

#### [RFCs](https://github.com/rust-lang/rfcs/labels/final-comment-period)

* *No RFCs entered final comment period this week.*

#### [Tracking Issues & PRs](https://github.com/rust-lang/rust/issues?q=is%3Aopen+label%3Afinal-comment-period+sort%3Aupdated-desc)

* [disposition: close] [Tracking issue for naked fns (RFC #1201)](https://github.com/rust-lang/rust/issues/32408)

### [New and Updated RFCs](https://github.com/rust-lang/rfcs/pulls)

* [new] [RFC: Add a process_group method to UNIX CommandExt](https://github.com/rust-lang/rfcs/pull/3228)

## Upcoming Events

Rusty Events between 2/2/2022 - 3/2/2022 🦀

### Online

* [February 3, 2022 | Cardiff, UK | **Rust Book Study Session - Smart Pointers** | Rust and C++ Cardiff](https://www.meetup.com/rust-and-c-plus-plus-in-cardiff/events/283480500/)
* [February 5 & 6, 2022 | Kyiv, UA | **Write a Game on Rust** | Rust Ukraine](https://dou.ua/calendar/42115/)
* [February 8, 2022 | Saarbrücken, DE | **Meetup: 17u16** | Rust-Saar](https://www.meetup.com/Rust-Saar/events/283617274)
* [February 8, 2022 | Seattle, WA, US | **Monthly meetup** | Seattle Rust Meetup](https://www.meetup.com/Seattle-Rust-Meetup/events/283213217/)
* [February 9, 2022 | Los Angeles, CA, US | **Raphael Tessmer & Celeste, finding craters on a rusty planet** (Virtual) | Rust Los Angeles](https://www.meetup.com/Rust-Los-Angeles/events/283232930/)
* [February 9, 2022 | Stuttgart, DE | **Rust-Meetup** | Rust Community Stuttgart](https://www.meetup.com/Rust-Community-Stuttgart/events/282545292)
* [February 15, 2022 | Indianapolis, IN, US | **Indy.rs - with Social Distancing** | Indy Rust](https://www.meetup.com/indyrs/events/283538948)
* [February 15, 2022 | Washington, DC, US| **Mid-month Rustful** | Rust DC](https://www.meetup.com/RustDC/events/283351974/)
* [February 16, 2022 | Vancouver, BC, CA | **Rust Study/Hack/Hang-out Night** | Vancouver Rust](https://www.meetup.com/Vancouver-Rust/events/283260386/)
* [February 17, 2022 | München, DE | **Rust - beyond "Hello World"**| Agile Softwareentwicklung München](https://www.meetup.com/maibornwolff-software-engineering-netzwerk/events/283379985)
* [February 17, 2022 | Nürnberg, DE | **Rust Nürnberg online #10**| Rust Nuremberg](https://www.meetup.com/rust-noris/events/283545751/)
* [February 17, 2022 | Stuttgart, DE | **Rust-Meetup** | Rust Community Stuttgart](https://www.meetup.com/Rust-Community-Stuttgart/events/282545308)
* [February 17, 2022 | Würzburg, DE | **Meet and chat about Rust** | Rust Würzburg Meetup Group](https://www.meetup.com/rust-wurzburg-meetup-group/events/283609518)
* [February 22, 2022 | Dublin, IE | **Rust Dublin February Meetup** - Rust Dublin](https://www.meetup.com/Rust-Dublin/events/283613610)
* [February 24, 2022 | Linz, AT | **Rust Meetup Linz - 19th Edition** | Rust Linz](https://www.meetup.com/Rust-Linz/events/283377693/)


If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Please remember to add a link to the event too.
Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

> * [`impl Not for !`](https://github.com/rust-lang/rust/pull/91122) (did you guess that "not never" is still "never"?)

– [llogiq on last week's TWiR](https://this-week-in-rust.org/blog/2022/01/26/this-week-in-rust-427)

Thanks to [scottmcm](https://users.rust-lang.org/t/twir-quote-of-the-week/328/1174) for the suggestion!

[Please submit quotes and vote for next week!](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*This Week in Rust is edited by: [nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq), [cdmistman](https://github.com/cdmistman), [ericseppanen](https://github.com/ericseppanen), [extrawurst](https://github.com/extrawurst), [andrewpollack](https://github.com/andrewpollack), [U007D](https://github.com/U007D), [kolharsam](https://github.com/kolharsam), [joelmarcey](https://github.com/joelmarcey), [mariannegoldin](https://github.com/mariannegoldin).*

*Email list hosting is sponsored by [The Rust Foundation](https://foundation.rust-lang.org/)*

<small>[Discuss on r/rust](https://www.reddit.com/r/rust/comments/k5nsab/this_week_in_rust_367/)</small>
