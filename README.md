# XAI PMS by KK Academy — Enterprise Model Bias & Transparency Monitoring

Explainable Artificial Intelligence (XAI) Performance Management System for monitoring model bias, fairness compliance, and transparency across large-scale enterprise machine learning pipelines.

## Razorpay In-Interface Checkout Integration

This updated commercial release resolves the payment gateway flow:
1. **In-Interface Modal Checkout**: Razorpay Standard Checkout opens directly inside the application interface (no new browser tab).
2. **Instant Subscription Redirection**: On payment completion, the callback immediately activates the subscription and redirects the user directly back into the live workspace.
3. **14-Day Free Trial Removed**: The trial countdown and trial badge are automatically replaced upon activation.
4. **Subscription Plan Status**: Shows **You are on "Monthly subscription plan"**.
5. **Renewal Date & Management**: Displays the calculated **Next renewal date** along with an interactive **Cancel Subscription** button.
6. **Interface Access Control**: Enforces that corporate users must have an active subscription or valid trial to access the enterprise pipeline monitoring suite.

## Quick Start

```bash
# 1. Install dependencies
pip install -r requirements.txt

# 2. Configure Streamlit secrets (copy example file)
cp .streamlit/secrets.toml.example .streamlit/secrets.toml

# 3. Run the application
streamlit run app.py
```

## Streamlit Secrets Configuration (`.streamlit/secrets.toml`)

Configure your Razorpay Test or Live API keys in `.streamlit/secrets.toml` or in Streamlit Cloud Dashboard -> Settings -> Secrets:

```toml
RAZORPAY_KEY_ID = "rzp_test_YOUR_KEY_HERE"
RAZORPAY_KEY_SECRET = "YOUR_RAZORPAY_SECRET_HERE"

# Optional Supabase database integration for multi-device persistence
SUPABASE_URL = "https://your-project.supabase.co"
SUPABASE_SECRET_KEY = "your-supabase-service-role-key"

[users.hr_admin]
password = "YOUR_SECURE_HR_PASSWORD"
role = "hr"
```

## Features

- **Pipeline Monitoring**: Monitor 4+ enterprise ML pipelines (Credit Scoring, Healthcare Triage, Talent Acquisition, Fraud Anomaly).
- **Fairness & Bias Audits**: Disparate Impact Ratio (80% four-fifths rule), Demographic Parity Difference, Equalized Odds.
- **Explainability**: Global feature attribution and SHAP/LIME local explanation waterfalls.
- **Human-in-the-Loop**: Contest model decisions with documented audit logs.
- **Commercial Billing**: Razorpay in-interface subscriptions (Monthly, Quarterly, Annual).
