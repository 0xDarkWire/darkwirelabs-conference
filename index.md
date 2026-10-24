---
layout: default
---

<pre class="bbs-box">╔══════════════════════════════════════════════════╗
║  EVENT_NAME BBS · Node 1 · 28800          ONLINE  ║
╚══════════════════════════════════════════════════╝</pre>

<pre class="bbs-block">───────────────────────────── SYSTEM INFO ─────────────────────────────

What....: EVENT_NAME — an invite-only hacker thing
Where...: TOP_SECRET (address drops 24h before, figure it out)
Talks...: schedule drops 24h before, updates as people sign up
Signup..: signal bot · 4h notice before your slot, minimum
SysOp...: <a href="https://www.darkwirelabs.com">dark wire labs</a>

────────────────────────────── MAIN MENU ──────────────────────────────

 <a href="#rules">[1] the rules</a>        <a href="#activities">[3] what goes down</a>
 <a href="#signup">[2] get a slot</a>      <a href="#schedule">[4] schedule</a>
</pre>

<h2 id="rules">the rules</h2>

- **Invite only.** No randos. Don't bring your weird friend nobody knows.
- **Address drops 24h before.** Figure it out.
- **Talk schedule goes out 24h before** and keeps getting updated as people sign up. Sign up whenever — just give 4 hours notice before your slot. A Signal bot pings everyone before you go on.
- **One talk at a time.** Otherwise go do whatever, we don't care.
- **Smoking's fine.**

<h2 id="activities">what goes down</h2>

- **Hack on whatever.** Bring a project, break something, build something. Nobody's stopping you.
- **CTF.** Run one, play one, wreck one. Spin up challenges and watch people suffer.
- **Hardware hacking and soldering** (where permitted). Bring your irons, your routers, your cursed dev boards. Ask before you desolder the venue.
- **Whatever else you bring.** That's the point.

<h2 id="signup">get a slot</h2>

Message the Signal bot with your handle and talk title. Four hours notice before your slot, minimum. You'll get pinged before you go on.

<h2 id="schedule">schedule</h2>

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

<footer>
  a <a href="https://www.darkwirelabs.com">dark wire labs</a> thing · no randos
</footer>
