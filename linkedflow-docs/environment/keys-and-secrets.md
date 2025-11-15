# API Keys and Secrets Management

## Required API Keys

### OpenAI
- **Purpose**: Post generation, content creation
- **Where to get**: https://platform.openai.com/api-keys
- **Environment Variable**: `OPENAI_API_KEY`

### Anthropic (Claude)
- **Purpose**: Alternative AI model, advanced reasoning
- **Where to get**: https://console.anthropic.com/
- **Environment Variable**: `ANTHROPIC_API_KEY`

### LinkedIn API (Future)
- **Purpose**: Direct LinkedIn integration
- **Status**: To be configured
- **Environment Variable**: `LINKEDIN_CLIENT_ID`, `LINKEDIN_CLIENT_SECRET`

## Secrets Management

### Development
- Store keys in `.env` files (not committed to git)
- Use `.env.example` as template

### Production
- environment variable management in hosting platform
- Never commit secrets to version control
- Rotate keys regularly
- Use secret management services (AWS Secrets Manager, etc.)

## Security Best Practices

1. **Never commit** `.env` files
2. Use different keys for development and production
3. Rotate API keys periodically
4. Monitor API usage and set rate limits
5. Use environment-specific configurations

