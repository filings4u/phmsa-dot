# screenings4u PHMSA DOT Management Portal

Domain: https://phmsa-dot.screenings4u.com

Portal code: `phmsa_dot`

This portal is for Employers that purchase a PHMSA-specific plan directly from dot.screenings4u.com. It manages only the purchaser's own company. It is not a C/TPA client-management workspace.

Access is provisioned from the purchased plan and is restricted to `PHMSA`. The backend rejects attempts to enter a different agency portal or write another agency's regulated records.

Pricing tiers in Supabase / Stripe test mode:
- Essential — $85/month
- Professional — $145/month
- Enterprise — $245/month

Enterprise includes `white_label`; lower tiers do not. Customer/employee/driver relationship emails use neutral branding when white label is not enabled.

Turnstile site key: `0x4AAAAAAE4-F43E-viFsKat`. Cloudflare hostname management must include `phmsa-dot.screenings4u.com`.

Supabase Auth redirect allowlist should include `https://phmsa-dot.screenings4u.com/auth-handoff.html`.
