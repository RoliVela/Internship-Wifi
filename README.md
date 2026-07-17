# Internship-Wifi

A one-page WiFi connect / review portal built during my internship at Toyota.

## Why this exists

At the location, WiFi name/password signs are posted around the store for
customers to join the guest network. Typing that password in by hand is
slow and a little tedious — especially for older customers — and signs
can't realistically be placed at every desk or corner of the building.

This page solves that: it's a simple link (or QR code) that can be put on a
sign at any desk. Customers open it, tap one button, and the WiFi password
is copied to their clipboard — no manual typing needed.

While building it, the marketing department mentioned the location needed
more Google reviews. So the page also includes a "Rate us on Google" button
that sends customers straight to the location's review form after they
connect to WiFi.

## What's in this repo

- `index.html` / `ToyotaLogo.png` — the original, live version of the portal.
- `duplicate/` — an exact copy of the same page, kept as an easy
  copy/paste starting point for future edits (e.g. adapting it for another
  location) without touching the original.

## How it works

Plain HTML/CSS/JS, no build step or framework — open `index.html` directly
in a browser, or edit it in any HTML editor.

- **Copy WiFi Password** — copies the network password to the clipboard via
  `navigator.clipboard`.
- **Rate us on Google** — links to the location's Google review form.
- **Visit counter** — tracks total portal opens using the free
  [CounterAPI](https://counterapi.dev) service.
