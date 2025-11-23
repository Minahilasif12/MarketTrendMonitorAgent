# Deployment Information

## Live Agent URL
**https://minahilasif222.pythonanywhere.com**

## Endpoints
- Health Check: https://minahilasif222.pythonanywhere.com/health
- Agent Info: https://minahilasif222.pythonanywhere.com/info
- Analysis: https://minahilasif222.pythonanywhere.com/analyze (POST)

## Deployment Platform
**PythonAnywhere** - Free Python web hosting

### Why PythonAnywhere?
- ✅ 100% Free (no credit card required)
- ✅ Perfect for Flask applications
- ✅ Easy deployment process
- ✅ Always-on web apps on free tier
- ✅ Built-in Python environment

### Deployment Steps Completed
1. Created free account at pythonanywhere.com
2. Uploaded files: agent.py, requirements.txt, test_agent.py
3. Installed dependencies: `pip3 install --user flask requests`
4. Created Flask web app pointing to /home/minahilasif222/agent.py
5. Configured WSGI file to import the Flask app
6. Reloaded the web app

## Integration with Supervisor
Use this URL in the supervisor integration spreadsheet:
- **Column C (API Testing Link)**: https://minahilasif222.pythonanywhere.com

## Testing the Deployment
```bash
# Health check
curl https://minahilasif222.pythonanywhere.com/health

# Get agent info
curl https://minahilasif222.pythonanywhere.com/info

# Trend analysis
curl -X POST https://minahilasif222.pythonanywhere.com/analyze \
  -H "Content-Type: application/json" \
  -d '{"type":"trend","market":"BTC/USD","prices":[45000,46000,47500],"volumes":[1000000,1200000,1500000]}'
```

## Maintenance
- Free tier requires logging in once every 3 months
- Site will be disabled on: **Monday 23 February 2026** (can be extended by clicking "Run until 3 months from today")
- Email reminders sent 1 week before expiration

## Team
- **Abdul Hannan** (22i-2441) - Project Manager
- **Minahil Asif** (22i-2710) - Lead Developer
- **Agha Ahsan** (22i-1117) - Data & Testing

## GitHub Repository
https://github.com/Minahilasif12/MarketTrendMonitorAgent
