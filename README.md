# Recursive Entropy Calculus

**PREPRINT - Research in Progress**

A mathematical framework extending Shannon entropy to hierarchically partitioned probability spaces, revealing universal bounds and resonance phenomena in structured systems.

## 📋 Quick Start

```bash
# Clone repository
git clone https://github.com/[username]/recursive-entropy-calculus
cd recursive-entropy-calculus

# Install dependencies
pip install -r requirements.txt

# Run basic example
python examples/basic_example.py

# Reproduce paper results
python experiments/reproduce_tables.py

# Generate all figures
python experiments/generate_figures.py
```

## 📖 Paper

**Title:** Recursive Entropy Calculus: Bounds and Resonance in Hierarchically Partitioned Systems  
**Status:** Preprint v0.1 - Under Review  
**PDF:** [paper/recursive_entropy_calculus.pdf](paper/recursive_entropy_calculus.pdf)

### Key Findings

- **Proven Bounds:** S̄(d) ≤ 1 and r̃(d) ≤ 2 for all hierarchical partitions
- **5:4 Resonance:** Empirical convergence to r̃ ≈ 1.25 in structured distributions
- **Universal Scaling:** Information scaling laws in hierarchical systems

## 🔬 Results Reproduction

### Core Theoretical Results
```bash
# Verify entropy bounds (Tables 6.1-6.2)
python experiments/verify_bounds.py

# Demonstrate 5:4 resonance (Table 6.3)  
python experiments/resonance_analysis.py

# Generate convergence plots
python experiments/plot_convergence.py
```

### Expected Output
- Entropy bounds satisfied for all tested distributions
- Resonance convergence within 0.2% of theoretical 5/4 = 1.25
- Convergence plots showing asymptotic behavior
/
```

## 🧮 Core Algorithm

The recursive entropy for depth d with branching factor b:

```python
def recursive_entropy(probabilities, depth, branching_factor):
    """
    Calculate S(d), S̄(d), and r̃(d) for hierarchical partition
    
    Args:
        probabilities: np.array of cell probabilities at depth d
        depth: recursion depth d ≥ 1  
        branching_factor: subdivision factor b ≥ 2
        
    Returns:
        dict: {'S_d': entropy, 'S_bar_d': normalized, 'r_tilde_d': growth}
    """
```

## 📊 Key Results

### Theoretical Bounds (Proven)
- **Normalized Entropy:** S̄(d) ≤ 1 with equality for uniform distributions
- **Growth Factor:** r̃(d) ≤ 2 with maximum at d=1

### Empirical Resonance (Observed)
- **5:4 Ratio:** r̃ → 1.25 for structured distributions
- **Universality:** Robust across power-law, exponential distributions
- **Convergence:** Relative error < 0.2% by depth 20

## Research Status

**Completed:**
- Mathematical proofs for entropy bounds
- Computational verification up to depth d=25
- Resonance demonstration across distribution families

**In Progress:**
- Theoretical derivation of 5:4 resonance
- Large-scale real-world dataset validation
- Extension to continuous distributions

**Needs Validation:**
- Independent verification of computational results
- Peer review of mathematical proofs
- Applications to practical hierarchical systems

## Applications

- **Information Theory:** Multi-scale entropy analysis
- **Algorithm Analysis:** Recursive complexity bounds  
- **Data Mining:** Hierarchical structure detection
- **Complex Systems:** Information scaling in fractals

##  Contributing

This is active research. Contributions welcome:

### How to Help
- **Verify Results:** Run reproduction scripts, report discrepancies
- **Review Mathematics:** Check proofs in `paper/` directory
- **Test Applications:** Apply REC to your hierarchical datasets
- **Theoretical Input:** Help derive the 5:4 resonance theoretically

### Contribution Guidelines
1. Fork repository
2. Create feature branch (`git checkout -b feature/improvement`)
3. Add tests for new functionality
4. Run full test suite (`python -m pytest tests/`)
5. Submit pull request with clear description

##  Citation

```bibtex
@misc{recursive_entropy_2024,
  title={Recursive Entropy Calculus: Bounds and Resonance in Hierarchically Partitioned Systems},
  author={[Author Name]},
  year={2024},
  note={Preprint},
  url={https://github.com/[username]/recursive-entropy-calculus}
}
```

##  License

MIT License - see [LICENSE](LICENSE) file for details.

##  Contact

- **Author:** Steven Reid
- **Email:** [sreid1118@gmail.com]
- **Issues:** Use GitHub Issues for questions/bugs
- **Discussions:** GitHub Discussions for theoretical input

---

**Disclaimer:** This is preliminary research. Mathematical proofs require peer review, computational results need independent verification, and practical applications remain largely untested. Use with appropriate caution.
