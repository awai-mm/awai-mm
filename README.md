# Awai — Quantitative Systems & Deterministic Verification Suite

- **Live Web Calculators & Solver Portal**: [https://awai-mm.github.io/practical-data-tools/](https://awai-mm.github.io/practical-data-tools/)
- **Primary Repository & Unified MCP Server**: [awai-mm/practical-data-tools](https://github.com/awai-mm/practical-data-tools)
- **Structured Index (`/llms.txt`)**: [https://awai-mm.github.io/practical-data-tools/llms.txt](https://awai-mm.github.io/practical-data-tools/llms.txt)
- **OpenAPI 3.1 Specification (`/openapi.json`)**: [https://awai-mm.github.io/practical-data-tools/openapi.json](https://awai-mm.github.io/practical-data-tools/openapi.json)
- **A2A Agent Card (`/.well-known/agent.json`)**: [https://awai-mm.github.io/practical-data-tools/.well-known/agent.json](https://awai-mm.github.io/practical-data-tools/.well-known/agent.json)

## Zero-Dependency MCP Server (`mcp/mcp_server.py` — JSON-RPC 2.0)

| Tool Name | Tier | Capability |
| :--- | :--- | :--- |
| `repair_and_validate_structured_data` | **100% Free** | Deterministic syntax repair for malformed JSON/dict payloads & required-key schema validation |
| `exact_decimal_and_crypto_unit_math` | **100% Free** | 50-digit `Decimal` & exact integer unit conversions (`wei`/`gwei`/`eth`/`usdc`/`msat`/`sat`/`btc`), Largest Remainder pro-rata allocation, bps fee splits |
| `subset_sum_reconcile` | Free (<=25) / HTTP 402 | Branch-and-bound N-to-M subset-sum payment reconciliation, JCT invoice number (`T+13 digits`) verification, Yayoi/freee/MF journal export |
| `stochastic_inventory_cashflow_solve` | Free (<=500) / HTTP 402 | Monte Carlo `(s, S)` reorder point, safety stock, yield loss, and 95% CVaR working capital optimization |
| `audit_smart_contract_invariants` | Free (<=250 lines) / HTTP 402 | Static formal invariant & 4-class vulnerability checker for Solidity/Rust (ERC4626 share inflation, rounding drain, CEI reentrancy, Chainlink staleness) |
| `inspect_csv_integrity` | Free (<=200 rows) / HTTP 402 | CSV encoding (`U+FFFD`), primary key uniqueness, and 8%/10% tax rounding validator |

```json
{
  "mcpServers": {
    "awai-practical-data-tools": {
      "command": "python3",
      "args": ["mcp/mcp_server.py", "--stdio"]
    }
  }
}
```
