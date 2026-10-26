# JWT and security tools

**Security warning:** Never paste a real access token, refresh token, API key, password, or confidential payload into a public website. A signed JWT is usually readable, and online tools may retain submitted data. Use dummy tokens or trusted local software.

## JWT.io Debugger

- **Website:** [jwt.io](https://jwt.io/)
- **Category:** JWT inspection
- **Pricing:** Free to access; check current site terms.
- **Best for:** Learning JWT structure with non-sensitive examples.
- **Key features:** Token decoding and signing demonstrations.
- **Advantages:** Widely used educational reference.
- **Limitations:** Do not submit production tokens; decoding does not validate trust or authorization.
- **Official documentation:** [JWT.io introduction](https://jwt.io/introduction)

## OAuth 2.0 and OpenID Connect

- **Website:** [OpenID Foundation specifications](https://openid.net/developers/)
- **Category:** Identity and security reference
- **Pricing:** Free to read.
- **Best for:** Understanding authentication protocols and standards.
- **Key features:** Specification and developer resources.
- **Advantages:** Primary standards organization.
- **Limitations:** Standards require careful implementation; a decoder alone cannot secure an application.
- **Official documentation:** [OpenID specifications](https://openid.net/developers/specs/)

## SSL Labs Server Test

- **Website:** [ssllabs.com/ssltest](https://www.ssllabs.com/ssltest/)
- **Category:** TLS configuration assessment
- **Pricing:** Free to use; review current service terms.
- **Best for:** Checking the public TLS configuration of a web server you control or are authorized to assess.
- **Key features:** Public server configuration analysis.
- **Advantages:** Detailed, widely recognized TLS diagnostics.
- **Limitations:** Public hostname testing can disclose the target to the service; results are not a complete security audit.
- **Official documentation:** [SSL Labs](https://www.ssllabs.com/projects/ssllabs-apis/)

## Security Headers

- **Website:** [securityheaders.com](https://securityheaders.com/)
- **Category:** HTTP security headers
- **Pricing:** Free to use; check provider terms.
- **Best for:** Reviewing headers on a site you operate.
- **Key features:** Header inspection and configuration guidance.
- **Advantages:** Quick starting point for response-header hygiene.
- **Limitations:** A score is not a complete security assessment; scanning may be visible to the service.
- **Official documentation:** [OWASP Secure Headers Project](https://owasp.org/www-project-secure-headers/)

## Password guidance

- **Website:** [NIST Digital Identity Guidelines](https://pages.nist.gov/800-63-4/)
- **Category:** Password and identity guidance
- **Pricing:** Free.
- **Best for:** Learning current identity and authenticator recommendations.
- **Key features:** Authoritative digital identity guidance.
- **Advantages:** Avoids relying on arbitrary third-party password scoring.
- **Limitations:** Guidance must be applied in the context of a system's threat model.
- **Official documentation:** [NIST SP 800-63](https://pages.nist.gov/800-63-4/)
