# Aerofatiguepro-python-library
pip install aerofatiguepro, A physics-informed fatigue life prediction library combining classical mechanics + machine learning + deployment.

Fatigue failure is still one of the biggest challenges in engineering — especially in aeroengine alloys.

Traditional models like Basquin and Coffin–Manson are powerful, but struggle with complex materials, temperature effects, and microstructure.

So I built something to bridge physics and AI.

🚀 Introducing: **AeroFatiguePro**
A physics-informed fatigue life prediction library combining classical mechanics + machine learning + deployment.

🔧 What it includes:
• Basquin S–N fatigue modeling
• Coffin–Manson low-cycle fatigue
• Paris Law crack growth
• Goodman / Gerber corrections
• Multiaxial fatigue (von Mises)
• FEA stress ingestion (Abaqus / ANSYS CSV)
• ML models (Random Forest, GPR)
• SHAP explainability
• Uncertainty estimation
• Benchmarking vs classical models
• FastAPI REST API + Docker deployment

📊 Key idea:
Instead of replacing physics with AI, this integrates both → better accuracy + interpretability.

⚙️ Built as a production-style system:
• Scalable ML pipeline
• Proprietary data validation
• API deployment



aerofatiguepro/
│
├── README.md
├── pyproject.toml
├── LICENSE
├── requirements.txt
│
├── aerofatiguepro/
│   ├── core.py
│   ├── ml.py
│   ├── fea.py
│   ├── validation.py
│   ├── api.py
│
├── examples/
│   ├── train_demo.py
│   ├── fea_demo.py
│
├── figures/
│   ├── parity.png
│   ├── benchmark.png
│   ├── sensitivity.png
│   ├── architecture.png
│
├── app/
│   └── streamlit_app.py
│
└── .github/workflows/ci.yml



from aerofatiguepro.core import fit_basquin

stress = [760,700,650,600,550]
cycles = [1e4,3e4,8e4,2e5,7e5]

fit = fit_basquin(stress, cycles)
print(fit)
• CI/CD ready


Would love feedback from materials scientists, ML engineers, and industry professionals.

#MaterialsScience #MachineLearning #AI #Fatigue #Aerospace #Engineering #Python #MLOps
