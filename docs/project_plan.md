## Project Structure
implicit-bias-optimizers/
│
├── README.md                          # Project overview, how to run
├── requirements.txt                   # Python dependencies
├── .gitignore                        # What NOT to commit to GitHub
│
├── data/                             # Data handling
│   ├── __init__.py
│   ├── loaders.py                    # Fashion-MNIST, CIFAR-10 loaders
│   └── README.md                     # Dataset documentation
│
├── models/                           # Neural network architectures
│   ├── __init__.py
│   ├── architectures.py              # LinearNet, MLP, CNN
│   └── README.md
│
├── optimizers/                       # Custom optimizer implementations
│   ├── __init__.py
│   ├── custom_optimizers.py          # USAM, SAM
│   └── README.md
│
├── training/                         # Training utilities
│   ├── __init__.py
│   ├── trainer.py                    # Generic training loop
│   ├── metrics.py                    # Accuracy, loss tracking
│   └── utils.py                      # Checkpointing, logging
│
├── visualization/                    # Plotting and analysis
│   ├── __init__.py
│   ├── plots.py                      # All plotting functions
│   ├── loss_landscape.py             # 2D landscape visualization
│   └── analysis.py                   # Statistical analysis tools
│
├── experiments/                      # Actual experiments (Colab notebooks)
│   ├── notebooks/                    # .ipynb files live here
│   │   ├── 01_gunasekar_reproduction.ipynb
│   │   ├── 02_fashion_mnist_linear.ipynb
│   │   ├── 03_fashion_mnist_mlp.ipynb
│   │   └── template.ipynb           # Template for new experiments
│   │
│   └── scripts/                      # .py versions (optional)
│       └── run_experiment.py
│
├── results/                          # Experiment outputs (NOT committed to git)
│   ├── checkpoints/                  # Model checkpoints
│   ├── logs/                         # Training logs
│   ├── figures/                      # Generated plots
│   └── metrics/                      # CSV/JSON metrics
│
├── literature/                       # Papers and notes
│   ├── papers/                       # PDF papers (add to .gitignore if large)
│   ├── notes/                        # Literature review notes
│   └── references.bib                # BibTeX for report
│
├── report/                           # LaTeX report (NeurIPS format)
│   ├── main.tex
│   ├── sections/
│   │   ├── introduction.tex
│   │   ├── background.tex
│   │   ├── experiments.tex
│   │   ├── results.tex
│   │   └── conclusion.tex
│   ├── figures/                      # Figures for report
│   └── neurips_2024.sty             # NeurIPS style files
│
├── presentation/                     # For bonus presentation
│   ├── slides.pptx (or .key or .pdf)
│   ├── figures/                      # Figures for slides
│   └── script.md                     # Speaking notes
│
└── docs/                             # Project documentation
    ├── project_plan.md               # This plan
    ├── meeting_notes.md              # Weekly meeting notes
    ├── contribution_log.md           # Individual contributions
    └── api_contracts.md              # Function signatures