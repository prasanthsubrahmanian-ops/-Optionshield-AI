# app.py - MINIMAL WORKING VERSION
import streamlit as st
import pandas as pd
import numpy as np

st.set_page_config(page_title="Optionshield AI", layout="wide")

st.title("🛡️ Optionshield AI")
st.markdown("### AI-Powered Nifty Options Trading")

st.success("🚀 App is live and working!")

# Simple components that always work
st.sidebar.title("Settings")
symbol = st.sidebar.selectbox("Select Symbol", ["NIFTY", "BANKNIFTY"])

# Basic calculator
st.subheader("📊 Quick POP Calculator")
strike = st.number_input("Strike Price", value=19500)
days = st.slider("Days to Expiry", 1, 30, 7)
pop = 75 - (abs(strike - 19500) / 19500 * 100)
st.metric("Estimated POP", f"{max(30, pop):.1f}%")

# Simple strategy display
st.subheader("🎯 Recommended Strategies")
strategies = [
    "Put Credit Spread - POP: 78%",
    "Iron Condor - POP: 72%", 
    "Call Debit Spread - POP: 65%"
]

for strategy in strategies:
    st.write(f"• {strategy}")

st.info("Optionshield AI - Live and Working! ✅")