Solar AI Support — Multi-Agent Customer Support System

Solar AI Support is a multi-agent customer support system for solar energy queries, built with CrewAI and Streamlit. Five specialized agents — a Query Analyzer, Assistant, Web Search Verifier, Quality Synthesizer, and Entry Agent — work together to triage, answer, fact-check, and log every question.

Key engineering: the Assistant's answers are grounded in a project knowledge base using TF-IDF retrieval (RAG). A conditional routing layer skips the Web Search and Synthesizer agents for simple questions, roughly halving LLM calls, while always forcing the full verification path for urgent or frustrated queries. Every interaction is logged to a structured SQLite database instead of a flat text file, with a live Database Explorer built into the UI.

The interface includes a live multi-step agent progress tracker, confidence scoring, cited web sources, an auto-escalation banner for urgent queries, session analytics, and a glassmorphic solar-themed design.

Built to demonstrate a production-style multi-agent AI workflow — retrieval, conditional routing, and structured logging — not just a single LLM call wrapped in a UI.

Project Made by - Jesika Shree Sivakumar
Sona College of Technology
