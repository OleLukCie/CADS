# Cognitive Asymmetric Data Science (CADS)

&gt; **Human-interpretable, AI-resistant data systems**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)

## Research Status

⚠️ **This is an experimental research project.** All tools are proof-of-concept and should not be used for critical security applications

## Overview

Cognitive Asymmetric Data Science (CADS) explores the design of data systems that remain fully interpretable to humans while becoming resistant to automated extraction and machine learning. This repository contains theoretical frameworks, experimental tools, and reference implementations for **semantic data protection**.

**<u>*Do not aim for AI-unintelligible systems, but for systems where AI learning costs vastly exceed gains.*</u>**

### Core Insight

&gt; *AI systems learn from statistical patterns. Humans understand through semantic context. CADS exploits this fundamental asymmetry.*

Traditional data protection focuses on **access control** (who can see data). CADS focuses on **learnability control** (who can derive value from data).

## Motivation

- **Generative AI era**: Internal documents, creative works, and proprietary knowledge are increasingly harvested for model training
- **Data sovereignty gap**: Existing tools prevent data *leakage* but not data *exploitation*
- **Asymmetric power**: Individual creators and small organizations lack technical means to protect their cognitive labor from automated extraction

## Key Concepts

| Concept                     | Description                                                                   | Status       |
| --------------------------- | ----------------------------------------------------------------------------- | ------------ |
| **Semantic Obfuscation**    | Context-dependent encoding that humans resolve but machines struggle to learn | Research     |
| **Dynamic Denormalization** | Intentional inconsistency to poison training data quality                     | Experimental |
| **Cognitive Watermarking**  | Human-perceptible, machine-disruptive marking systems                         | Prototype    |
| **Learnability Metrics**    | Quantifying "usefulness to humans" vs. "learnability by AI"                   | Theory       |

## Repository Structure

```markdown
CADS/
├── theory/               # Foundational papers and frameworks
├── tools/                # Reference implementations
│   ├── semantic_obfuscator/     # Text obfuscation tools
│   ├── visual_confusion/        # Image protection utilities
│   └── dynamic_watermarker/     # Document marking system
├── experiments/          # Validation studies
├── applications/         # Domain-specific examples
└── docs/                 # Tutorials and best practices
```

```bash
git clone https://github.com/olelukcie/CADS.git
```

### Basic Usage: Semantic Obfuscation

```python
from cads.text import SemanticObfuscator

# Initialize with domain-specific codebook
obfuscator = SemanticObfuscator(
    domain="financial_reporting",
    consistency_level="high"  # Options: low, medium, high
)

# Obfuscate sensitive strategic content
original = "Q3 revenue declined due to supply chain disruptions"
protected = obfuscator.obfuscate(original)

print(protected)
# Output: "Autumn harvest fell short following logistical headwinds"
# Humans understand via context; ML systems see inconsistent terminology
```

### Visual Document Protection

```python
from cads.visual import CognitiveWatermark

watermarker = CognitiveWatermark(
    method="layout_deception",
    strength=0.7
)

protected_doc = watermarker.apply(
    input_path="sensitive_report.pdf",
    output_path="protected_report.pdf"
)
# Key metadata visually preserved but OCR-resistant
```

## Contributing

We welcome contributions from:

- **Data scientists**

- **ML researchers**

- **Security engineers**

- **Domain experts**

See *CONTRIBUTING.md* for guidelines.

## Ethical Guidelines

CADS is designed for **legitimate protection of intellectual labor**, not for:

- Evading legal discovery or transparency requirements

- Concealing illegal activities

- Malicious disruption of AI safety research

## Related Work

- **Mathematical privacy guarantees**

- **Adversarial Examples**: ML input perturbations

- **Data Poisoning**: Attacking ML training

- **Steganography**: Hidden information encoding

**CADS differs** by focusing on *semantic* rather than *statistical* protection, and prioritizing *human usability* alongside *machine resistance*.

## License

MIT License - See *LICENSE* for details.

**Disclaimer**: This project explores emerging concepts in data protection. The techniques described may not provide legal protection against data scraping or training. Consult legal counsel for compliance with applicable regulations (GDPR, CCPA, etc.).