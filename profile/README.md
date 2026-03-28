# Nightwatch Astro

Open-source tools for astrophotography automation and observatory safety.

## Projects

| Repository | Description | Language |
|------------|-------------|----------|
| [ascom-alpaca-core](https://github.com/nightwatch-astro/ascom-alpaca-core) | ASCOM Alpaca protocol types and traits for Rust | Rust |
| [esp-idf-sse](https://github.com/nightwatch-astro/esp-idf-sse) | Server-Sent Events for ESP-IDF | Rust |
| [esp-idf-improv-wifi](https://github.com/nightwatch-astro/esp-idf-improv-wifi) | Improv WiFi provisioning for ESP-IDF | Rust |
| [esp-idf-smtp](https://github.com/nightwatch-astro/esp-idf-smtp) | SMTP email client for ESP-IDF | Rust |

## About

Nightwatch is an ESP32-based safety monitor and dead man's switch for astrophotography. It implements the ASCOM Alpaca protocol to integrate with imaging software like NINA, SGP, and Voyager.

The libraries in this org are standalone crates published to [crates.io](https://crates.io) — usable in any Rust project, not just Nightwatch.
