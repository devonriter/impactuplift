# Impact Uplift

A free web app that helps high school students run fundraisers for Detroit nonprofits. A student presses **Run Fundraiser**, picks a partner and an idea, plans it, runs it, and gets credit and a celebration at the end.

Live at **https://impactuplift.org** (also https://crew-solve-for-tomorrow.web.app).

Impact Uplift is an open-source community benefit project. It is not a registered nonprofit and never handles money: donations go straight to each partner through the partner's own donation page. Our first partners are Better Way Detroit and Detroit Rescue Mission Ministries.

It was built by a high school CREW class in Detroit as an entry in Samsung Solve for Tomorrow (2026-27).

## How it is built

The students are the product team. They talk to the partners, decide what to build, and test what goes live. An AI builder writes the code:

1. **Decide.** The team agrees on what to build next and writes it as a Feature Request.
2. **Send.** The request is sent through a form and becomes an issue in this repo labeled `build`.
3. **Build.** An AI builder (a GitHub Action, instructions in [CLAUDE.md](CLAUDE.md)) makes the change and publishes it straight to the live site. The issue gets a comment with the link and a build number.
4. **Test.** The team opens the live site, checks that the footer shows their build number, and checks it against their request.
5. **Fix.** If something is wrong, the team sends a new Feature Request, and it publishes the same way.

## Running it yourself

The app is plain HTML, CSS and JavaScript with no build step. Clone the repo and open `index.html`, or serve the folder with any static file server (for example `npx serve .`). It deploys to Firebase Hosting as static files.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Ideas and bug reports are welcome as issues.

## Privacy and safety

- No real information about the people the partners serve, ever.
- Students are named by first name only.
- The app collects as little as possible: no sign-ups, and progress is saved only in the visitor's browser.
- Everything in this repo is public.

## License

[MIT](LICENSE). Partner names belong to the partners and are not covered by the license.
