# Norton Down Methodist Church website

A prototype website for Norton Down Methodist Church, Stratton-on-the-Fosse, Somerset.

It is a single page (`index.html`) with six sections: Home, Your first visit, What's on, Weddings & baptisms, Our story, and Find us & contact. Photos are in `img/`. There is no build step: open `index.html` in a browser.

Live preview for review: https://kelz-roberts.github.io/Norton-Down-Methodist-Church/ (published with GitHub Pages from the `main` branch, so every push to `main` updates it).

## Design approach

- Written for an older congregation and for people in the local community who don't yet come to church.
- Built to WCAG 2.2 AA, with larger text and controls than the minimum.
- The aim is to bring people through the door: no streaming, no newsletter. Events are listed on the What's on page.
- The coffee morning is presented as a friendly social event open to anyone.

## Still to confirm with the church before going live

- Photo consent for Mendip Brass
- A real photo of the outside of the chapel
- The time of the Harvest Supper
- Whether to offer online giving

## Contact details (settled 9 October 2026)

Malcolm Barlow, church steward, is the primary contact: 07966 434623, m.barlow1942@gmail.com.
He is used for all general enquiries, first visits, lifts and the footer.
Rev Andrew Prout (01373 301092, andrew.prout@methodist.org.uk) stays as the contact for
weddings, baptisms and funerals.
The old steward@nortondownmethodistchurch.org.uk address has been removed: the church domain
has no mail records at all, so it could never receive email.

## New open questions

- The "Send us a message" form does not send anywhere yet. It shows a thank you and discards
  the message. Laron is hooking it up to email before go-live. It should send to Malcolm at
  m.barlow1942@gmail.com. Left as-is deliberately until then.
- Better long-term fix: set up malcolm@nortondownmethodistchurch.org.uk to forward to his
  Gmail. Needs access to the domain settings.

## Confirmed by the church (9 October 2026)

- Malcolm Barlow has confirmed he is happy for his phone number and email address to appear
  on the public website. He is also the key contact for this rebuild.
- Malcolm is the key contact because Rev Andrew Prout is slow to respond. The minister's
  details stay listed on the contact page, but nothing on the site routes people to him.
  Do not undo this: it is a deliberate decision by the church, not an oversight.
- Elaine Herbert, baptism secretary, 01761 412773, is shown for baptism bookings - on the
  baptisms card and on the contact page. Her number is already public on the church's
  current website.

## Corrected by the church (9 October 2026)

- No tea or coffee is served after the Sunday service. People do stay behind for a chat.
  Reworded in four places. The Wednesday coffee morning is unaffected and still serves
  tea, coffee and biscuits.
- The chapel does have a hearing loop. The accessibility FAQ previously said it did not.
- Malcolm Barlow is the primary contact for everything, weddings and funerals included.
  Those now point to him rather than to Rev Andrew Prout.

## The map (9 October 2026)

Malcolm reported that the hand-drawn sketch put the chapel in the wrong place. The sketch was
not based on real map data, so nothing stopped it being wrong. It has been replaced with a real
OpenStreetMap embed, chosen over a Google Maps embed because OSM sets no cookies and does no
tracking, so the site still needs no cookie banner or privacy policy.

The pin location was checked by Kelly on 9 October 2026 and is correct. The address shown
is Fosseway, Stratton-on-the-Fosse, Radstock, Somerset BA3 4QA.

## Lifts (confirmed 9 October 2026)

Lifts are offered. People arrange them through Malcolm on 07966 434623. The "to confirm"
badge has been removed from that FAQ answer and the wording now says so plainly.

## OUTSTANDING: safeguarding (removed 9 October 2026, must come back)

The footer carried a "Safeguarding" link that pointed at the contact page and did nothing,
with an "add policy" badge on it. It has been removed rather than left as a dead link, because
a dead link labelled Safeguarding is worse than none: someone with a real concern clicks it and
finds nothing.

**This must be put back before the site is considered finished.** The Methodist Church expects
every local church to have a published safeguarding policy and a named safeguarding officer.

Ask Malcolm which applies:
- the church has its own policy - publish it, and name the safeguarding officer
- only the Circuit has one - link to the Somerset Mendip Methodist Circuit policy and name the
  officer
- neither exists - this is a governance gap for the church to resolve, not a website problem

Kelly asked on 9 October 2026 to be reminded about this.

## Favicon (chosen 9 October 2026)

The icon is the chapel's Victorian arched window in cream on the site green, with the mullions
forming a cross, so it reads as both "our chapel" and "a church". Chosen over a plain cross
(too generic) and a chapel silhouette (the runner-up). A warm-lit open door was rejected: it
looked good large but lost all meaning at 16px.

Files, all generated from the same shape:
- `favicon.svg` - the browser tab icon, rounded corners
- `favicon-32.png` - fallback for older browsers that cannot use an SVG icon
- `apple-touch-icon.png` - 180px, square corners, for a phone home screen. iOS applies its own
  rounding, so this one must stay square.

The bars were deliberately thickened from the first draft: at 16px the thinner version washed
out. Check any redesign at actual tab size, not just enlarged.

The working sketches are in `favicon-options/`, kept on Kelly's Mac and excluded from the repo
by `.gitignore`.

## Coffee morning picture (9 October 2026) - PLACEHOLDER

The "A cuppa and a chat" card had an empty grey photo box. There is no photo of the coffee
morning yet, so it now holds a simple drawing of a teapot, two cups and biscuits, inline SVG
in the site palette.

A drawing was chosen over a stock photo on purpose: the design approach above says real local
photos, not stock, and a stock photo of strangers with mugs would undercut that.

**Still wanted: a real photo of the Wednesday coffee morning.** Swap it in when there is one.

The cups are a fixed cream (#F7F4EC) rather than var(--surface), because in dark mode
--surface is nearly black and the cups disappeared against the dark green. The steam uses
--muted, which flips with the theme. Keep that in mind if the drawing is ever edited.
