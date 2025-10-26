# PhIDO: AI-Powered Photonic Circuit Designer

PhIDO (Photonics Intelligent Design and Optimization) is an intelligent web application that automates the design of photonic integrated circuits using Large Language Models (LLMs). The application provides both automatic guided workflows and step-by-step execution modes for circuit design, from specification to layout generation and Design Rule Checking (DRC).

[Paper preprint](https://arxiv.org/abs/2508.14123)

> **📚 Getting Started**: For hands-on tutorials and detailed step-by-step instructions on using PhIDO, see [GETTING_STARTED.md](GETTING_STARTED.md). This comprehensive guide includes practical examples, troubleshooting tips, and detailed explanations of both workflow modes.

## 🏗️ Project Structure

```
PhIDO/
├── PhotonicsAI/                    # Main application package
│   ├── Photon/                     # Core application modules
│   │   ├── webapp.py              # Streamlit web application (main entry point)
│   │   ├── llm_api.py             # LLM API integrations and model configurations
│   │   ├── utils.py               # Utility functions for circuit processing
│   │   ├── prompts.yaml           # LLM prompts and system instructions
│   │   ├── templates.yaml         # Circuit templates and configurations
│   │   ├── DemoPDK.py             # Demo Process Design Kit
│   │   ├── drc/                   # Design Rule Checking module
│   │   │   ├── drc.py             # DRC execution engine
│   │   │   └── drc_script.drc     # KLayout DRC script
│   │   └── CIRCUIT_wdd0.yaml      # Example circuit configuration
│   ├── KnowledgeBase/             # Design knowledge and components
│   │   ├── DesignLibrary/         # Photonic component library
│   │   │   ├── mzi_1x1_heater_tin_cband.py  # MZI with TiN heaters
│   │   │   ├── mzi_2x2_heater_tin_cband.py  # 2x2 MZI with heaters
│   │   │   └── ...                # Other photonic components
│   │   └── FDTD/                  # Finite Difference Time Domain simulation data
│   └── config.py                  # Application configuration
├── GETTING_STARTED.md             # Comprehensive tutorial and user guide
├── GETTING_STARTED_EXAMPLE_OUTPUTS/  # Example outputs for tutorial prompts
│   ├── Level 1 Prompt/            # Single component example outputs
│   ├── Level 2 Prompt/            # Two components example outputs
│   ├── Level 3 Prompt/            # Multiple components example outputs
│   └── Level 4 Prompt/            # Complex system example outputs
├── requirements.txt               # Complete environment dependencies
├── Makefile                      # Build and run commands
├── Testbench.xlsx                # Contains 102 testbench prompts
└── README.md                     # This file
```

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
