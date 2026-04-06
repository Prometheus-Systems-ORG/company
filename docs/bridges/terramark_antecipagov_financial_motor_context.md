# TerraMark / AntecipaGov / Financial Motor context

Secret-free contextual bridge derived from the attached Odoo production observation and field inventory supplied by the user.

## System reading

The observed runtime is no longer just a sales flow.
It already behaves like a public receivables origination and structuring engine with two layers living in the same body:

- Odoo operational layer: lead, quotation, sale order, order line, delivery, invoiceability, chatter, attachments, activities
- emergent financial layer: blockchain anchor, block, motor, cluster, RWA pool, token namespace, payment state, profit, margin, multi-year grouping

## Canonical interpretation

- `AntecipaGov` = operational product/front door
- `FinancialMotor` = canonical internal core
- `TerraMark` = public expression layer for pooling, RWA, tokenization and external presentation

## Minimum observed custom field nucleus

High-certainty observed nucleus:
- `Numero Empenho`
- `PKURL Lead`
- `Blockchain`
- `Bloco`
- `Status Pagamento`
- `Valor Pago`
- `Custo Total`
- `Lucro Total`
- `Margem (%)`
- `Situação da Fatura`
- `ID PNCP`
- `Parceiros/Stakeholders`

Medium-certainty inferred normalized nucleus:
- `block_id`
- `motor_id`
- `rwa_pool_code`
- `cluster_code`
- `financial_total`
- `expected_receivable_date`

## Required contract posture

- Odoo stays the operational writer of record.
- Public app layers must consume normalized entities instead of parsing semantic labels only.
- `block` and `motor` must be separated as entities even if the current runtime still displays merged labels.
- `blockchain_anchor` must be ratified semantically before external token logic depends on it.

## Surface targets

- `antecipagov.terramark.org`
- `terramark.org/app/v1/antecipagov`

## See also

- `contracts/apis/terramark_antecipagov_financial_motor_field_registry.yaml`
