# Pakistan Land Parcels & Khasra Lookup MCP (پنجاب، پاکستان)

[اردو](#اردو)

Connect your AI assistant (Claude, ChatGPT, Cursor) to [BumiAtlas](https://bumiatlas.com) for Pakistani land research through the Model Context Protocol (MCP).

This listing is a focused entry point for:

- ~878k urban plot parcels in Punjab, from the PULSE project (Punjab Urban Land Systems Enhancement, Board of Revenue)
- Coverage of development-authority scheme areas: Lahore (LDA schemes, cooperative societies), private housing societies province-wide (DHA, Bahria and others), PHATA, and the Faisalabad, Gujranwala, Multan and Rawalpindi authorities
- Parcel lookup by its PULSE parcel code (`uniParco`, e.g. `TXL-TEH-00C-000-0157-0000` — tehsil, mouza, block, muraba, khasra, sub-khasra), by housing society name, or by coordinates
- Khasra plot number, block/sector/phase, land use, area, PULSE's own anomaly flag, and district/tehsil/division
- Satellite and street map images of a parcel and its neighbours, labelled by khasra number

The data is **indicative property lines only, not legal boundaries** (the source viewer's own disclaimer). It covers urban Punjab only — no rural khasras, nothing outside Punjab — and carries no owner, title or price information.

## Connect

```
https://bumiatlas.com/mcp/pakistan
```

Add it as a custom connector in any MCP client and sign in with Google. Tools, examples and data notes: [bumiatlas.com/mcp-docs/pakistan](https://bumiatlas.com/mcp-docs/pakistan).

- **Claude:** Settings → Connectors → Add custom connector, paste the URL, then Connect.
- **ChatGPT:** Settings → Apps & Connectors → Advanced → Developer mode, then Create with the URL and OAuth authentication.

## Tools

| Tool | Description |
|---|---|
| `PK_parcel_search` | Find parcels by parcel code or prefix (a prefix lists that tehsil's or mouza's parcels), by society name, or by `latitude, longitude`; each result is the whole record, with the boundary as GeoJSON on request |
| `PK_parcel_image` | Satellite or street map image of a parcel or point, with every parcel in view outlined and labelled with its khasra number |

## Example prompts

- *"Which parcel is at 31.4726, 74.2728? What's its land use?"*
- *"Look up parcel MDT-TNS-0A1-000-0632-0000 and show it on satellite imagery."*
- *"List parcels in DHA phase 6 with their plot sizes."*
- *"Are there flagged (anomalous) parcels in Millat Town, Faisalabad?"*

## Data source

Parcels © PULSE, Board of Revenue, Government of Punjab — the backend of the public viewer at gis.pulse.gop.pk. A copy of public indicative linework for research, not a legal land record.

## اردو

اپنے AI اسسٹنٹ (Claude، ChatGPT یا Cursor) کو [BumiAtlas](https://bumiatlas.com) سے جوڑیں اور Model Context Protocol (MCP) کے ذریعے پنجاب، پاکستان کی اراضی کے بارے میں تحقیق کریں۔

- پنجاب کے شہری علاقوں میں تقریباً 8.78 لاکھ پلاٹ، PULSE پراجیکٹ (بورڈ آف ریونیو) سے
- LDA سکیمز، کوآپریٹو سوسائٹیاں، نجی ہاؤسنگ سوسائٹیاں (DHA وغیرہ)، PHATA اور فیصل آباد، گوجرانوالہ، ملتان اور راولپنڈی کے ترقیاتی ادارے
- پارسل کوڈ، سوسائٹی کے نام یا کوآرڈینیٹس سے تلاش؛ خسرہ نمبر، زمین کے استعمال اور رقبہ کے ساتھ
- سیٹلائٹ اور سٹریٹ میپ تصاویر

یہ لکیریں صرف اشاریاتی ہیں، قانونی حدود نہیں — نہ مالک کا نام، نہ عنوان، نہ قیمت۔ صوبہ پنجاب کے شہری علاقے تک محدود ہے۔

**رابطہ:** کسی بھی MCP کلائنٹ میں `https://bumiatlas.com/mcp/pakistan` کو custom connector کے طور پر شامل کریں اور Google سے سائن ان کریں۔ ٹولز کے نام انگریزی میں ہیں لیکن اسسٹنٹ اردو میں جواب دے سکتا ہے۔

مثال کے سوالات:

- *"کوآرڈینیٹس 31.4726, 74.2728 پر کون سا پلاٹ ہے؟ اس کا استعمال کیا ہے؟"*
- *"پارسل MDT-TNS-0A1-000-0632-0000 کو سیٹلائٹ تصویر پر دکھائیں۔"*
- *"DHA فیز 6 کے پلاٹس اور ان کے سائز دکھائیں۔"*
