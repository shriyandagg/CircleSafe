# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users
Everyone who posts on social media to more than one group of people: friends, family, school, and work. The user's job is to send each post to the right people and know who can see it before it goes out.

The DP4 slides name high school students as the research target. The team has since widened the audience to everyone, so design must not assume a teen-only user.

In practice the prototype is opened on a phone browser, starting in the Feed, during usability tests and class demos for CS 4351 Design Project 4 (Team 13).

## Product Purpose
CircleSafe is a mobile social privacy prototype. People sort contacts into circles, choose which circles see each post, check exactly who that is before publishing, and control whether each circle can be used for account discovery (profile suggestions).

Success means a user can complete the three tasks without help:
1. **Simple:** open a feed post's audience details and identify its circle and members.
2. **Moderate:** name a new circle, select members, save it, and reopen it to edit membership.
3. **Complex:** change a circle's sharing and discovery settings, then preview and publish a post to an eligible audience.

## Positioning
Every post's audience is visible and checkable down to the individual people, before and after publishing. A required preview step lists the circles and recipients, and circles with sharing paused cannot be selected.

## Operating Context
- Mobile web prototype, used on a phone, starting in the Feed.
- Posting and account discovery are simulated. Reloading resets all changes.
- The team presents it in a Google Slides deck (CircleSafe_DP4_Implementation) that has screenshots of each flow on slides 7–11. Design changes must not invalidate that deck's described screens, flows, or labels.
- Source: github.com/shriyandagg/CircleSafe. Hosted at social-circles-ochre.vercel.app.

## Capabilities and Constraints
Fixed (confirmed by user):
- Four bottom tabs, in order: **Feed, Circles, Post, Privacy**.
- Circles manages circle names and members. Privacy manages sharing and discovery per circle. They stay separate (DP3 usability issue 2).
- The three tasks above and their flows.
- Labels quoted in the slides: "View audience details" on every post; the circle audience badge beside the profile name on each post; save banners naming the circle when returning to Circles; "Edit privacy settings"; "Preview" as a required step before "Confirm & publish"; paused circles disabled when choosing an audience.
- Sample data: 8 contacts, 4 circles (Close Friends, Family, School, Work), 2 starter posts.
- A single HTML file (HTML, CSS, JavaScript, no build step) hosted on Vercel.

Listed as "Partial" in the slides (proposed, not built yet; building any of them is a team decision):
- Issue 8: a running count of selected members in the circle editor.
- Issue 10: a plain-language label for "discoverability".
- Issue 11: inline field feedback for a blank circle name instead of an `alert()`.

## Brand Commitments
- Name: **CircleSafe**.
- Voice: plain and reassuring. Wording explains what will happen in everyday language and is never alarming or legalistic.
- No binding logo or other brand assets.

## Evidence on Hand
- The DP3 usability findings (11 issues and responses) are in the slides.
- No real users, testimonials, metrics, or production data exist. Never invent any.

## Product Principles
1. Show who can see it. Every post's audience is visible and checkable down to individual people.
2. Confirm before sharing. Publishing always passes through an audience preview.
3. Keep settings where users look for them. Membership lives in Circles and privacy lives in Privacy, each easy to find.
4. Plain words over jargon. Privacy terms are explained in place.
5. Prototype honesty. Simulated behavior is labeled as simulated.

## Accessibility & Inclusion
Built for a general audience on phones: readable contrast, tap targets at least 44px, keyboard focus states, and screen-reader status announcements for saves (already present via `role="status"`).
