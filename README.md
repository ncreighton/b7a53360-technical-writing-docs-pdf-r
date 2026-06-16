# Technical Writing & Docs PDF Report Generation and Branding API

> Stop wasting hours manually formatting and branding your technical PDFs — this API turns raw documentation into polished, on-brand reports with a single call.

The Technical Writing & Docs PDF Report Generation and Branding API automates the tedious process of converting your technical content into professional, branded PDFs. It eliminates formatting inconsistencies and ensures every report matches your company’s visual identity, saving you time and reducing errors.

## What's Included

- Generate branded PDFs from any JSON or Markdown input with a single API endpoint
- Customize headers, footers, logos, color schemes, and fonts to match your brand
- Automatic table of contents, page numbering, and cross-references for long documents
- Supports code blocks, diagrams, and technical formatting (syntax highlighting, inline math)
- Batch processing for multi-document generation with consistent styling

## Who Is This For

- Technical writers who need to produce branded user manuals, API docs, or release notes
- Documentation teams at SaaS companies automating monthly/quarterly report generation
- Developers building internal tools that require on-brand PDF output from technical content
- Product managers creating branded whitepapers or technical proposals from existing docs

## How It Works

Sign up to get your unique API key. Send a POST request with your content (JSON or Markdown) and branding parameters (logo URL, colors, fonts). The API returns a ready-to-download PDF with consistent formatting and your brand applied.

## Frequently Asked Questions

**What input formats does the API accept?**
It accepts both JSON (structured sections with markdown content) and plain Markdown. You can also pass metadata like document title, author, and version.

**How do I customize the branding?**
Include parameters in your request: logo URL, primary/secondary colors (hex codes), font family (from a supported list), and header/footer text. You can also upload a custom CSS template for advanced control.

**Is there a limit on document length or file size?**
The API supports documents up to 500 pages or 50 MB per request. For larger projects, use batch processing or pagination endpoints.

**Can I integrate this with my existing documentation workflow?**
Yes, it works with any language (Python, JavaScript, curl, etc.) via REST API. You can chain it with your CI/CD pipeline or static site generators like Docusaurus or Hugo.

**What happens if I need to change branding later?**
Simply update the branding parameters in your API call. The API applies the new styles to future PDFs. You can also store a default brand profile in your account settings.

## What You Get

- Instant digital download
- Complete REST API with full documentation
- Free updates for life — pay once, own forever
- Setup guide and usage instructions

**Get instant access to the Technical Writing & Docs PDF Report Generation and Branding API for just $32.49 and deliver polished, branded reports in seconds.**

## Features

- Full REST API

## Quick Start

```bash
# 1. Install dependencies
pip install -r requirements.txt

# 2. Configure environment
cp .env.example .env
# Edit .env with your settings

# 3. Run locally
uvicorn main:app --reload --port 8000

# 4. View interactive docs
open http://localhost:8000/docs
```

## Docker Deployment

```bash
# Build and run
docker compose up -d

# Check health
curl http://localhost:8000/health
```

## Authentication

Get a token first:
```bash
curl -X POST "http://localhost:8000/auth/token?username=admin&password=admin123"
```

Use the token in subsequent requests:
```bash
curl -H "Authorization: Bearer YOUR_TOKEN" http://localhost:8000/items
```

## API Endpoints

| Method | Path | Description |
|--------|------|-------------|
| GET | `/health` | System health |
| POST | `/auth/token` | Get JWT token |
| GET | `/items` | List all items |
| POST | `/items` | Create item |
| GET | `/items/{id}` | Get item |
| PATCH | `/items/{id}` | Update item |
| DELETE | `/items/{id}` | Delete item |
| GET | `/stats` | API statistics |

Full interactive docs: `http://localhost:8000/docs`

## Rate Limits

| Endpoint | Limit |
|----------|-------|
| `/auth/token` | 10/minute |
| `GET /items` | 60/minute |
| `POST /items` | 30/minute |
| `DELETE /items` | 20/minute |

## Running Tests

```bash
pip install pytest httpx
pytest tests/ -v
```

## Production Notes

- Change `SECRET_KEY` in `.env` before deploying
- Replace in-memory `_db` with a real database
- Add proper user management to `auth.py`
- Configure `ALLOWED_ORIGINS` for CORS
- Use Nginx/Traefik as reverse proxy

## License

MIT


---

## Free vs Pro

| Feature | Free | Pro |
|---------|:----:|:---:|
| 100 requests/day | Yes | Yes |
| Standard endpoints | Yes | Yes |
| JSON responses | Yes | Yes |
| Unlimited requests | - | Yes |
| Premium endpoints | - | Yes |
| Batch processing | - | Yes |
| Webhook notifications | - | Yes |
| SLA guarantee | - | Yes |
| Priority support | - | Yes |

### Upgrade to Pro

Get the full version with all premium features, priority support, and lifetime updates.

**[Get Pro Version](https://buy.stripe.com/9B69ATdPp2k43lmeM4cZg3A)**

- [Buy Now (Stripe)](https://buy.stripe.com/9B69ATdPp2k43lmeM4cZg3A)

