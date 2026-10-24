---
layout: default
---

<header class="hero">
  <img class="logo" src="{{ '/Logo.png' | relative_url }}" alt="Dark Wire Labs logo">
  <h1 class="site-title">{{ site.title }}</h1>
  <p class="tagline">an invite-only thing. no randos.</p>
</header>

## the rules

- **Invite only.** No randos. Don't bring your weird friend nobody knows.
- **Address drops 24h before.** Figure it out.
- **Talk schedule goes out 24h before** and keeps getting updated as people sign up. Sign up whenever — just give 4 hours notice before your slot. You'll get pinged before you go on (Signal bot: TBD).
- **One talk at a time.** Otherwise go do whatever, we don't care.
- **Smoking's fine.**

## what goes down

- **Hack on whatever.** Bring a project, break something, build something. Nobody's stopping you.
- **CTF.** Run one, play one, wreck one. Spin up challenges and watch people suffer.
- **Hardware hacking and soldering** (where permitted). Bring your irons, your routers, your cursed dev boards. Ask before you desolder the venue.
- **Whatever else you bring.** That's the point.

## get a slot

Signup: TBD — Signal bot/channel getting set up. Once it's live: message the bot with your handle and talk title. Four hours notice before your slot, minimum. You'll get pinged before you go on.

## schedule

{% if site.data.schedule %}
| time | speaker | talk |
|------|---------|------|
{% for talk in site.data.schedule %}| {{ talk.time }} | {{ talk.speaker }} | {{ talk.title }} |
{% endfor %}
{% else %}
TBD — drops 24h before. Sign up whenever.
{: .note}
{% endif %}

## location

Address drops 24h before. Figure it out.
{: .note}

<footer>
  <nav aria-label="Site navigation">
    <ol class="footers">
      <li class="footer"><a href="https://www.darkwirelabs.com">[dark wire labs]</a></li>
    </ol>
  </nav>
</footer>
