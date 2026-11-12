# PixNative website

Static site for GitHub Pages: https://cspixelmindstudios.github.io/pixnative/ (privacy policy at `privacy.html`).

- `index.html` and `style.css` are hand-written. `privacy.html`, `assets/` and the screenshot list in `index.html` are generated.
- Edit the policy in `docs/release/PRIVACY_POLICY.md`, never in `privacy.html`.

Update and publish (from the repo root):

```
python3 tools/build_site.py            # needs ffmpeg and `pip install markdown`
git add website && git commit -m "Update website"
GH_TOKEN=... bash tools/publish_site.sh  # pushes website/ to cspixelmindstudios/pixnative (public)
```

After the app is live, replace the "Coming soon on Google Play" span in `index.html` with a link to
`https://play.google.com/store/apps/details?id=com.pixnative.app`.
