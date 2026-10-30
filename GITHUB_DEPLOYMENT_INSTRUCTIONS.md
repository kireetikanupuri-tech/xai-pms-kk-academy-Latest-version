# How to Push to your GitHub Repository

1. Extract this ZIP archive into your local project directory.
2. In your app.py, the Razorpay integration snippet provides the in-interface modal checkout.
3. Configure your Razorpay Key ID in .streamlit/secrets.toml:
   RAZORPAY_KEY_ID = "rzp_test_..."
   RAZORPAY_KEY_SECRET = "..."
4. Run locally to test:
   pip install -r requirements.txt
   streamlit run app.py
5. Commit and push to GitHub:
   git add .
   git commit -m "Fix: Razorpay in-interface modal checkout and monthly subscription flow"
   git push origin main
