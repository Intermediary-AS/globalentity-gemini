# GlobalEntity for Gemini CLI

Official company data in [Gemini CLI](https://github.com/google-gemini/gemini-cli): look up companies in
66 national business registers and the GLEIF LEI index, verify VAT, EORI and LEI numbers, see ownership
chains, check insolvency status, screen names against sanctions lists and get statutory VAT rates.
Every answer cites the official source.

Built by [Intermediary AS](https://www.globalentityapi.com) on the
[GlobalEntity API](https://www.globalentityapi.com) MCP server.

## Install

```bash
gemini extensions install https://github.com/Intermediary-AS/globalentity-gemini
```

Then start Gemini CLI and sign in once:

```text
/mcp auth globalentity
```

A browser window opens. Sign in with the email of your GlobalEntity workspace (or a
[free trial](https://www.globalentityapi.com/app)), approve access, and return to the terminal.
Gemini CLI stores the token and refreshes it automatically.

## Try it

```text
Find the Norwegian company with organisation number 925615471 and show its status and address.
Is the Danish VAT number DK22756214 valid, and who is it registered to?
Who owns A.P. Møller - Mærsk A/S (LEI 549300D2K6PKKKXVNN73)? Show the ownership chain.
Screen the name Rosneft against sanctions lists.
What are the current VAT rates in Finland?
```

## Tools

| Tool | What it does |
|------|--------------|
| `search_companies` | Search an official national company register by name or registration number |
| `verify_identifier` | Validate a VAT (EU VIES), EORI or LEI number |
| `resolve_company` | Merge register, LEI and VAT data into one golden record |
| `get_ownership` | Parent companies, subsidiaries and UBO candidates (GLEIF) |
| `check_insolvency` | Bankruptcy, liquidation and other distress status |
| `screen_sanctions` | Name screening against UN, EU, US OFAC and UK sanctions lists |
| `get_vat_rates` | Statutory VAT rates for 225 countries and territories |
| `get_profile` | Shows which GlobalEntity account is connected |

All tools are read-only. Sanctions results are name-based signals to confirm against the official
lists, and the identity Trust Score is not a credit rating.

## Links

- Product and pricing: <https://www.globalentityapi.com>
- MCP server documentation: <https://www.globalentityapi.com/docs#mcp>
- Privacy policy: <https://www.globalentityapi.com/privacy>
- Terms: <https://www.globalentityapi.com/terms>
- Support: <contact@intermediary.no>

The extension files in this repository are MIT licensed. Use of the GlobalEntity API is governed by
its [terms of service](https://www.globalentityapi.com/terms).
