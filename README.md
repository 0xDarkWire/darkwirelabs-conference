# EVENT_NAME — conference site

Static Jekyll site for https://conference.darkwirelabs.com (placeholder subdomain — rename when the event has a name).

## Placeholders to replace

- `EVENT_NAME` in `_config.yml` — the event's real name.
- `conference.darkwirelabs.com` in `CNAME` and `url` in `_config.yml` — the real subdomain.
- "Message the Signal bot" in `index.md` — real signup contact/bot handle.

## Updating the schedule

Edit `_data/schedule.yml` and push. The homepage renders it automatically:

```yaml
- time: "14:00"
  speaker: "handle"
  title: "Talk title"
```

## DNS (one-time setup)

At the DNS provider for `darkwirelabs.com`, add:

- Type: `CNAME`, Name: `conference`, Value: `0xDarkWire.github.io`

GitHub Pages provisions the HTTPS cert automatically once DNS resolves.

## Local preview

```
bundle install
bundle exec jekyll serve
```
