# Lanko — Business Context Document

## Company Overview
- **Name**: Lanko (Polish window & door manufacturer)
- **Industry**: Window and door manufacturing (PVC, aluminum)
- **Employees**: ~120 people
- **Ownership**: Acquired by Marek Kuna 5 years ago from previous owner who underinvested
- **Export ratio**: 80%+ (primarily EU: Netherlands, France, Belgium, Germany)
- **Core system**: Wincon (ERP/production management software used by ~100 Polish window manufacturers)

## Products & Services
- PVC windows and doors (primary)
- Aluminum windows and doors (secondary, high-margin, bottleneck in quoting)
- Accessories: ventilators (nawietrzaki), handles, glass packages, steel reinforcements
- Currently trying to minimize installation/mounting services (liability and risk)

## Revenue & Financial Context
- Benchmark: Abacus (competitor) seen as role model for profitability and process optimization
- Price sensitivity: 6-7% variance between salespeople quoting the same job (standardization needed)
- Sales strategy: Lead with cheapest base configuration, upsell later (like car configurators)
- 80% of new internet inquiries don't convert — massive time wasted on quoting

## Team & Key Personnel
- **Marek Kuna** — CEO/Owner, strategic vision, acquired company 5 years ago
- **Krzysztof Korycki** — IoT/cybersecurity expert, building AI pricing tool prototype
- **Maciej Bogdalski** — DevOps/developer, deep Wincon database expertise, building analytics overlays
- **Miłosz Barczyński** — AI/ML specialist, co-founded Carlease Polska, runs AI automation consultancy
- **Mateusz Norberczak** — Business development, partners with Miłosz
- **~120 staff**: salespeople, technologists, logistics, warehouse, production, accounting, procurement

## Current Technology Stack
- **Wincon**: Core ERP — manages production, pricing, orders, invoicing, CMR generation
  - No official API available (major limitation)
  - Database access possible (Maciej has deep knowledge)
  - Performance issues: system is slow due to large unarchived database
  - Competitors: TrevSuite, WinPro, Elcia (French), Prodeli
- **Email**: home.pl hosting, 130 email accounts, ~1200 PLN/year
- **CRM**: None currently — major gap
- **Prototype AI pricing tool**: Built by Krzysztof, recognizes hand-drawn sketches, generates quotes from pricing tables (rastry)
- **Maciej's analytics app**: Python/Flask backend, Svelte frontend, pulls from Wincon database

## Current Pain Points
1. **Quoting is slow & manual**: Salespeople spend hours quoting jobs that never convert (90% of internet leads)
2. **Wincon is sluggish**: Large unarchived database causes slow response times
3. **No CRM**: No systematic customer relationship management
4. **Manual processes everywhere**: Invoice forwarding, procurement emails, ventilator ordering, pallet optimization — all done manually
5. **Price inconsistency**: Different salespeople quote different prices for same specs (6-7% variance)
6. **Aluminum quoting bottleneck**: Aluminum technologists are scarce industry-wide, long wait times
7. **Employee dependency**: Knowledge locked in individuals, no systematized processes
8. **After-hours availability**: No customer service outside business hours

## Automation Projects Under Discussion

### Project A: AI Pricing Tool (Wyceniarka)
- **Status**: MVP/prototype exists
- **What it does**: Recognizes hand-drawn sketches and competitor quotes, generates pricing from tables
- **Tech**: Uses Gemini API for image recognition, pricing tables (rastry) as knowledge base
- **Cost concern**: Analyzing HD images costs ~$2 per document via API
- **Next steps**: Better frontend, Wincon integration, automatic order creation
- **Market potential**: Could be sold to other window manufacturers (2,500+ in Poland)

### Project B: Wincon Integration
- **Status**: Maciej has database access and understanding
- **What it does**: Direct database queries instead of slow UI, price extraction, analytics
- **Key value**: Eliminates manual raster updates, enables real-time pricing
- **Challenge**: No official API, database-level integration only
- **Quick win**: Archive pre-2025 data to improve Wincon performance (Abacus does this annually)

### Project C: AI Customer Service Bots
- **Status**: Early testing with Miłosz
- **What it does**: Inbound/outbound phone calls, multi-language (Dutch, French, etc.), email handling
- **Features**: CRM integration, automatic follow-up, after-hours availability, call summaries
- **Use cases**: Secretary replacement, complaint handling, sales qualification, supplier communication

### Project D: Internal Process Automation
- **Status**: Planned — site visit next week for process audit
- **What it does**: Email workflow automation, invoice generation, procurement automation, logistics optimization
- **Examples identified**:
  - Automatic proforma invoice generation and sending
  - Pallet/transport optimization (Tetris-like loading)
  - Ventilator ordering automation
  - Supplier price monitoring and comparison
  - Invoice-to-order matching (currently done manually by accounting)
- **Tools considered**: N8N, Google Workspace workflows, custom agents

## Strategic Goals
- **Short-term (6 months)**: Get AI pricing tool production-ready, start internal automation audit, improve Wincon performance
- **Long-term (3-5 years)**: Full order-to-delivery automation, expand AI tools to other window manufacturers, build SaaS product for industry
- **Risk awareness**: AI technology moves fast — competitors or general-purpose AI could make custom solutions obsolete
- **Budget mindset**: ROI-conscious, even partial return on investment would be considered success

## Competitive Landscape
- **Direct competitors**: Other Polish window manufacturers (Oknoplast, Drutex, Eko Okna — much larger)
- **Software competitors**: Elcia (France), Prodeli — charge millions in licensing fees to both manufacturers and dealers
- **Differentiation opportunity**: AI-powered instant quoting from sketches/competitor PDFs — unique in market
- **Market size**: 2,500+ window manufacturers in Poland alone, plus EU market
