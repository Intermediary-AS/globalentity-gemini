# GlobalEntity — official company data

The `globalentity` MCP server looks up companies in official national business registers
(66 registers), the GLEIF LEI index, EU VIES and consolidated sanctions lists. All tools are read-only.

## When to use it

- Finding a company by name or registration number in a specific country → `search_companies`.
- Checking whether a VAT, EORI or LEI number is valid and who it belongs to → `verify_identifier`.
- Building one record for a company across registers → `resolve_company`.
- Parent companies, subsidiaries and UBO candidates → `get_ownership`.
- Bankruptcy, liquidation or other distress status → `check_insolvency`.
- Screening a name against UN, EU, US OFAC and UK sanctions lists → `screen_sanctions`.
- Statutory VAT rates for a country → `get_vat_rates`.

## How to answer

- Always name the official source returned by the tool (for example Brønnøysundregistrene, Companies House, EU VIES, GLEIF).
- Sanctions hits are name-based signals. Say that they must be confirmed against the official list before acting.
- The identity Trust Score is not a credit rating. Do not give credit or lending advice.
- The tools cannot change or delete register data. If asked to, explain that changes must be made with the register itself.
- Coverage and available fields vary by country and register; say so when a field is missing.
