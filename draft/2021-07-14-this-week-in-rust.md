Title: This Week in Rust 399
Number: 399
Date: 2021-07-14
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

### Project/Tooling Updates

* [Announcing Arti, a pure-Rust Tor implementation](https://blog.torproject.org/announcing-arti)
* [Programmatic stream filtering using WebAssembly](https://www.infinyon.com/blog/2021/06/smartstream-filters/)
* [Filecoin Rust implementation "Forest" project update](https://medium.com/chainsafe-systems/forest-growth-d26998a3da61)
* [Mina Rust implementation update: Web 3.0 with Rust x Wasm](https://medium.com/chainsafe-systems/mina-wasm-benefits-for-web-3-0-3d25991c3b75)
* [This Week In TensorBase 11](https://tensorbase.io/thisweek/2021-07-14-tw_11/)

### Observations/Thoughts

* [series] [Why and how we wrote a compiler in Rust: Part 2](https://bnjjj.medium.com/why-and-how-we-wrote-a-compiler-in-rust-blog-post-series-2-x-the-stack-548dad1919d0)

### Rust Walkthroughs

* [Rust Nibbles : Gazebo - An introduction to the Gazebo library](https://developers.facebook.com/blog/post/2021/07/06/rust-nibbles-gazebo-dupe/)
* [Host a wasm module on Raspberry Pi easily Part 1](https://blog.knoldus.com/host-a-wasm-module-on-raspberry-pi-easily-part-1/)
* [Hello, Video Codec! - Demystify video codecs by writing one in ~100 lines of Rust](https://medium.com/tempus-ex/hello-video-codec-9937f64835bd)

* [Learning Idiomatic Rust with FizzBuzz](https://www.fotonixx.com/posts/rust-fizzbuzz/)

### Miscellaneous

## Crate of the Week

This week's crate is [endbasic](https://www.endbasic.dev), an emulator friendly DOS / BASIC environment running on small hardware and the web.

Thanks to [Julio Merino](https://users.rust-lang.org/t/crate-of-the-week/2704/935) for the suggestion.

[Submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

## Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

## Updates from Rust Core

254 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2021-07-05..2021-07-12

* [improve opaque pointers support](https://github.com/rust-lang/rust/pull/86873)
* [recover from `&dyn mut` ... parse errors](https://github.com/rust-lang/rust/pull/86812)
* [improve error reporting for modifications behind `&` references](https://github.com/rust-lang/rust/pull/86815)
* [do not suggest adding a semicolon after ?](https://github.com/rust-lang/rust/pull/87061)
* [use `#[track_caller]` in const panic diagnostics](https://github.com/rust-lang/rust/pull/87000)
* [query-ify global limit attribute handling](https://github.com/rust-lang/rust/pull/86674)
* [support forwarding caller location through trait object method call](https://github.com/rust-lang/rust/pull/81360)
* [shrink the deprecated span](https://github.com/rust-lang/rust/pull/86320)
* [report an error if resolution of closure call functions failed](https://github.com/rust-lang/rust/pull/86249)
* [stabilize `RangeFrom` patterns in 1.55](https://github.com/rust-lang/rust/pull/83918)
* [account for capture kind in auto traits migration](https://github.com/rust-lang/rust/pull/86869)
* [stop generating `alloca`s & `memcmp` for simple short array equality](https://github.com/rust-lang/rust/pull/85828)
* [inline `Iterator as IntoIterator`](https://github.com/rust-lang/rust/pull/84560)
* [optimize unchecked indexing into `chunks` and 'chunks_mut`](https://github.com/rust-lang/rust/pull/86823)
* [add `Integer::log` variants](https://github.com/rust-lang/rust/pull/80918)
* [special case for integer log10](https://github.com/rust-lang/rust/pull/869309)
* [cargo: unify cargo and rustc's error reporting](https://github.com/rust-lang/cargo/pull/9655)
* [rustdoc: fix rendering of reexported macros 2.0 and fix visibility of reexported items](https://github.com/rust-lang/rust/pull/86841)

### Rust Compiler Performance Triage

Mostly quiet week; improvements outweighed regressions.

Triage done by **@simulacrum**.
Revision range: [9a27044f4..5aff6dd](https://perf.rust-lang.org/?start=9a27044f42ace9eb652781b53f598e25d4e7e918&end=5aff6dd07a562a2cba3c57fc3460a72acb6bef46&absolute=false&stat=instructions%3Au)

1 Regressions, 4 Improvements, 0 Mixed; 0 of them in rollups

[Full report here](https://github.com/rust-lang/rustc-perf/blob/master/triage/2021-07-13.md).

### Approved RFCs

Changes to Rust follow the Rust [RFC (request for comments) process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

*No RFCs were approved this week.*

### Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now.

### [RFCs](https://github.com/rust-lang/rfcs/labels/final-comment-period)

* [disposition: merge] [RFC: let-else statements](https://github.com/rust-lang/rfcs/pull/3137)
* [disposition: merge] [RFC: I/O Safety](https://github.com/rust-lang/rfcs/pull/3128)
* [disposition: merge] [`#[derive(Default)]` on enums with a `#[default]` attribute](https://github.com/rust-lang/rfcs/pull/3107)

### [Tracking Issues & PRs](https://github.com/rust-lang/rust/labels/final-comment-period)

* [disposition: merge] [Stabilize const_fn_transmute, const_fn_union](https://github.com/rust-lang/rust/pull/85769)
* [disposition: merge] [Stabilize bindings_after_at](https://github.com/rust-lang/rust/pull/85305)
* [disposition: close] [Add expr202x macro pattern](https://github.com/rust-lang/rust/pull/84364)
* [disposition: merge] [Stabilize `impl From<[(K, V); N]>` for HashMap (and friends)](https://github.com/rust-lang/rust/pull/84111)
* [disposition: merge] [Stabilize "RangeFrom" patterns in 1.55](https://github.com/rust-lang/rust/pull/83918)
* [disposition: merge] [Remove P: Unpin bound on impl Future for Pin](https://github.com/rust-lang/rust/pull/81363)
* [disposition: merge] [Tracking Issue for IntoInnerError::into_parts etc. (io_into_inner_error_parts)](https://github.com/rust-lang/rust/issues/79704)
* [disposition: merge] [Tracking Issue for array_map](https://github.com/rust-lang/rust/issues/75243)
* [disposition: merge] [Tracking issue for #![feature(maybe_uninit_extra)](https://github.com/rust-lang/rust/issues/63567)

### New RFCs

*No new RFCs were proposed this week.*

## Upcoming Events

### Online

* [July 7, 2021, Denver, CO, US - End-to-end Encrypted Messaging in Rust, with Ockam by Mrinal Wadhwa - Rust Denver](https://www.meetup.com/Rust-Boulder-Denver/events/277633525/)
* [July 8, 2021, Berlin, DE - Rust Hack and Learn - Berline.rs](https://berline.rs/)
* [July 13, 2021, Seattle, WA, US - Monthly meetup - Seattle Rust Meetup](https://www.meetup.com/Seattle-Rust-Meetup/events/gskksrycckbrb/)
* [July 14, 2021, Malaysia - Rust Meetup July 2021 - Golang Malaysia, feat Rustlang, Erlang, Haskelllang and `.*-?(lang|script)\`](https://docs.google.com/forms/d/e/1FAIpQLSdoVbexvU3TZox1D9yLKPUggeTuih7TEDR6eaFQGTEgJtXZ5g/viewform)
* [July 14, 2021, Dublin, IE - Rust Dublin July Remote Meetup - Rust Dublin](https://www.meetup.com/Rust-Dublin/events/278698763/)
* [July 20, 2021, Washington, DC, US - Mid-month Rustful - Rust DC](https://www.meetup.com/RustDC/events/vdhxgsycckbbc/)
* [July 21, 2021, Vancouver, BC, CA - Rust Adoption at Huawei - Vancouver Rust](https://www.meetup.com/Vancouver-Rust/events/zkqvjsycckbcc/)

### North America

* [July 14, 2021, Atlanta, GA, US - Grab a beer with fellow Rustaceans - Rust Atlanta](https://www.meetup.com/Rust-ATL/events/qxqdgrycckbsb/)

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Please remember to add a link to the event too.
Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

**NZXT**

* [Senior Software Engineer for CAM (Remote)](https://nzxt.bamboohr.com/jobs/view.php?id=259)
* [Senior Software Engineer for Streaming Software (Remote)](https://nzxt.bamboohr.com/jobs/view.php?id=317)

**Kollider**

* [Junior Backend Engineer (Remote)](https://kollider.homerun.co/junior-backend-engineer/en)
* [Senior Backend Engineer (Remote)](https://kollider.homerun.co/senior-backend-engineer/en)
* [DevOps Engineer (Remote)](https://kollider.homerun.co/devops-engineer/en)

**Tempus Ex**

* [Several positions available (San Francisco, Atlanta, and Remote)](https://tempus-ex.com/careers)

**ChainSafe Systems**

* [Rust Developer (Remote)](https://jobs.smartrecruiters.com/ChainSafeSystemsInc/743999739358248-rust-developer)

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

> Beginning Rust: Uh why does the compiler stop me from doing things this is horrible
>
> Advanced Rust: Ugh why doesn't the compiler stop me from doing things this is horrible

– [qDot on twitter](https://twitter.com/qDot/status/1412536312150716416)

Thanks to [Nixon Enraght-Moony](https://users.rust-lang.org/t/twir-quote-of-the-week/328/1074) for the self-suggestion!

[Please submit quotes and vote for next week!](https://users.rust-lang.org/t/twir-quote-of-the-week/328)

*This Week in Rust is edited by: [nellshamrell](https://github.com/nellshamrell), [llogiq](https://github.com/llogiq), and [cdmistman](https://github.com/cdmistman).*

<small>[Discuss on r/rust](https://www.reddit.com/r/rust/comments/k5nsab/this_week_in_rust_367/)</small>