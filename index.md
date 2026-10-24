---
layout: default
---

# {{ site.title }}

<p class="tagline">an invite-only thing. no randos.</p>

## the rules

- **Invite only.** No randos. Don't bring your weird friend nobody knows.
- **Address drops 24h before.** Figure it out.
- **Talk schedule goes out 24h before** and keeps getting updated as people sign up. Sign up whenever — just give 4 hours notice before your slot. A Signal bot pings everyone before you go on.
- **One talk at a time.** Otherwise go do whatever, we don't care.
- **Smoking's fine.**

## want a slot?

Message the Signal bot with your handle and talk title. Four hours notice before your slot, minimum. You'll get pinged before you go on.

## schedule

{% if site.data.schedule %}
<table class="schedule">
  <thead>
    <tr><th>time</th><th>speaker</th><th>talk</th></tr>
  </thead>
  <tbody>
    {% for talk in site.data.schedule %}
    <tr>
      <td class="time">{{ talk.time }}</td>
      <td>{{ talk.speaker }}</td>
      <td>{{ talk.title }}</td>
    </tr>
    {% endfor %}
  </tbody>
</table>
{% else %}
<p class="note">TBD — drops 24h before. Sign up whenever.</p>
{% endif %}

## location

<p class="note">Address drops 24h before. Figure it out.</p>

<footer>
  a <a href="https://www.darkwirelabs.com">dark wire labs</a> thing
</footer>
