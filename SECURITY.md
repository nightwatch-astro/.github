# Security Policy

## Supported Versions

| Repository | Supported |
|------------|-----------|
| ascom-alpaca-core | Latest release |
| esp-idf-sse | Latest release |
| esp-idf-improv-wifi | Latest release |
| esp-idf-smtp | Latest release |

## Reporting a Vulnerability

If you discover a security vulnerability in any nightwatch-astro repository, please report it responsibly:

1. **Do NOT open a public issue**
2. Email security concerns to the maintainers via GitHub's [private vulnerability reporting](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing-information-about-vulnerabilities/privately-reporting-a-security-vulnerability) feature on the affected repository
3. Include:
   - Description of the vulnerability
   - Steps to reproduce
   - Potential impact
   - Suggested fix (if any)

## Response Timeline

- **Acknowledgment**: Within 48 hours
- **Assessment**: Within 1 week
- **Fix**: Dependent on severity, typically within 2 weeks for critical issues

## Scope

These libraries run on embedded devices (ESP32) and desktop systems. Security considerations include:

- **Network protocol safety**: ASCOM Alpaca runs over HTTP; credential handling, input validation
- **Memory safety**: Rust's type system handles most concerns, but `unsafe` blocks and FFI boundaries need scrutiny
- **Dependency supply chain**: We use Dependabot to monitor dependency vulnerabilities
